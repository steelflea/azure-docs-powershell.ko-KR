---
title: Azure PowerShell 제거
description: Azure PowerShell의 전체 제거를 수행하는 방법
ms.date: 11/30/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: a35814f4411dd9cab75fa36bd13ff087cdec8f9b
ms.sourcegitcommit: 93f93b90ef88c2659be95f3acaba514fe9639169
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/05/2018
ms.locfileid: "52826700"
---
# <a name="uninstall-the-azure-powershell-module"></a>Azure PowerShell 모듈 제거

이 문서에서는 Azure PowerShell의 이전 버전을 제거하거나 시스템에서 완전히 제거하는 방법을 알려줍니다. Azure PowerShell을 완전히 제거하기로 한 경우 [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet을 통해 몇 가지 피드백을 보내주세요.
버그가 발생한 경우 [GitHub 문제를 제출](https://github.com/azure/azure-powershell/issues)해주시면 감사하겠습니다.

## <a name="uninstall-from-powershell"></a>PowerShell에서 제거하기

PowerShellGet을 사용하여 Azure PowerShell을 설치하는 경우 [Uninstall-module](/powershell/module/powershellget/uninstall-module) cmdlet을 사용할 수 있습니다. 그러나 `Uninstall-Module`은 모듈 중 하나만 제거합니다. Azure PowerShell을 완전히 제거하려면 각 모듈을 개별적으로 제거해야 합니다. 2개 이상의 Azure PowerShell 버전을 설치한 경우 제거가 복잡할 수 있습니다.

현재 설치한 Azure PowerShell 버전을 확인하려면 다음 명령을 실행합니다.

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

```output
Version              Name                                Repository           Description
-------              ----                                ----------           -----------
6.11.0               AzureRM                             PSGallery            Azure Resource Manager Module
6.13.1               AzureRM                             PSGallery            Azure Resource Manager Module
```

다음 스크립트는 PowerShell 갤러리를 쿼리하여 종속 하위 모듈의 목록을 가져옵니다. 그런 다음 스크립트는 올바른 버전의 각 하위 모듈을 제거합니다. `Process` 또는 `CurrentUser`외의 범위에서 이 스크립트를 실행하려면 관리자 권한이 필요합니다.

```powershell-interactive
function Uninstall-AllModules {
  param(
    [Parameter(Mandatory=$true)]
    [string]$TargetModule,

    [Parameter(Mandatory=$true)]
    [string]$Version,

    [switch]$Force,

    [switch]$WhatIf
  )
  
  $AllModules = @()
  
  'Creating list of dependencies...'
  $target = Find-Module $TargetModule -RequiredVersion $version
  $target.Dependencies | ForEach-Object {
    if ($_.requiredVersion) {
      $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.requiredVersion}
    }
    else { # Assume minimum version
      # Minimum version actually reports the installed dependency
      # which is used, not the actual "minimum dependency." Check to
      # see if the requested version was installed as a dependency earlier.
      $candidate = Get-InstalledModule $_.name -RequiredVersion $version
      if ($candidate) {
        $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$version}
      }
      else {
        Write-Warning ("Could not find uninstall candidate for {0}:{1} - module may require manual uninstall" -f $_.name,$version)
      }
    }
  }
  $AllModules += New-Object -TypeName psobject -Property @{name=$TargetModule; version=$Version}

  foreach ($module in $AllModules) {
    Write-Host ('Uninstalling {0} version {1}...' -f $module.name,$module.version)
    try {
      Uninstall-Module -Name $module.name -RequiredVersion $module.version -Force:$Force -ErrorAction Stop -WhatIf:$WhatIf
    } catch {
      Write-Host ("`t" + $_.Exception.Message)
    }
  }
}
```

이 함수를 사용하려면 코드를 복사하고 PowerShell 세션에 붙여넣습니다. 다음 예제에서는 이전 버전의 Azure PowerShell을 제거하는 함수를 실행하는 방법을 보여 줍니다.

```powershell-interactive
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

이 스크립트를 실행하면 제거하고 있는 각 하위 모듈의 이름 및 버전이 표시됩니다. 제거하지는 안되, 삭제할 것을 표시만 하도록 스크립트를 실행하려면 `-WhatIf` 옵션을 사용합니다.

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

제거하려는 Azure PowerShell의 모든 버전에 대해 이 명령을 실행합니다. 편의를 위해, 다음 스크립트는 최신 버전을 __제외한__ 모든 AzureRM 버전을 제거합니다.

```powershell-interactive
$versions = (get-installedmodule AzureRM -AllVersions | Select-Object Version)
$versions[1..($versions.Length-1)]  | foreach { Uninstall-AllModules -TargetModule AzureRM -Version ($_.Version) -Force }
```

## <a name="uninstall-msi"></a>MSI 제거

MSI 패키지를 사용하여 Azure PowerShell을 설치한 경우 PowerShell이 아닌 Windows 시스템을 통해 제거해야 합니다.

| 플랫폼 | 지침 |
|----------|--------------|
| 윈도우 10 | 시작 > 설정 > 앱 |
| Windows 7 </br>Windows 8 | 시작>제어판 > 프로그램 > 프로그램 제거 |

이 화면의 프로그램 목록에서 "Azure PowerShell"이 보여야 여기에서 제거할 수 있습니다.
