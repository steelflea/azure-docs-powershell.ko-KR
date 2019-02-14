---
title: Azure PowerShell 제거
description: Azure PowerShell의 전체 제거를 수행하는 방법
ms.date: 06/20/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 3828a6f9d60a68c2837cc201a50d8707324f4f0a
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/13/2018
ms.locfileid: "53217238"
---
# <a name="uninstall-the-azure-powershell-module"></a>Azure PowerShell 모듈 제거

이 문서에서는 Azure PowerShell의 이전 버전을 제거하거나 시스템에서 완전히 제거하는 방법을 알려줍니다. Azure PowerShell을 완전히 제거하기로 한 경우 [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet을 통해 몇 가지 피드백을 보내주세요.
버그가 발생한 경우 [GitHub 문제를 제출](https://github.com/azure/azure-powershell/issues)해주시면 감사하겠습니다.

## <a name="uninstall-msi-or-web-platform-installer"></a>MSI 또는 웹 플랫폼 설치 관리자 제거

MSI 패키지 또는 웹 플랫폼 설치 관리자를 사용 하여 Azure PowerShell을 설치한 경우 PowerShell이 아닌 Windows 시스템을 통해 제거 해야 합니다.

| 플랫폼 | 지침 |
|----------|--------------|
| 윈도우 10 | 시작 > 설정 > 앱 |
| Windows 7 </br>Windows 8 | 시작>제어판 > 프로그램 > 프로그램 제거 |

이 화면의 프로그램 목록에서 "Azure PowerShell"이 보여야 여기에서 제거할 수 있습니다.

## <a name="uninstall-from-powershell"></a>PowerShell에서 제거하기

PowerShellGet을 사용하여 Azure PowerShell을 설치하는 경우 [Uninstall-module](/powershell/module/powershellget/uninstall-module) cmdlet을 사용할 수 있습니다. 그러나 `Uninstall-Module`은 모듈 중 하나만 제거합니다. Azure PowerShell을 완전히 제거하려면 각 모듈을 개별적으로 제거해야 합니다. 여러 버전의 Azure PowerShell이 설치되어 있는 경우 제거가 복잡할 수 있습니다.

다음 스크립트를 사용하면 단일 버전의 Azure PowerShell을 완전히 제거할 수 있습니다. 해당 스크립트는 PowerShell 갤러리를 쿼리하여 종속 하위 모듈의 목록을 가져옵니다. 그런 다음 스크립트는 올바른 버전의 각 하위 모듈을 제거합니다.

```powershell-interactive
function Uninstall-AllModules {
  param(
    [Parameter(Mandatory=$true)]
    [string]$TargetModule,

    [Parameter(Mandatory=$true)]
    [string]$Version,

    [switch]$Force
  )

  $AllModules = @()

  'Creating list of dependencies...'
  $target = Find-Module $TargetModule -RequiredVersion $version
  $target.Dependencies | ForEach-Object {
    $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.requiredversion}
  }
  $AllModules += New-Object -TypeName psobject -Property @{name=$TargetModule; version=$Version}

  foreach ($module in $AllModules) {
    Write-Host ('Uninstalling {0} version {1}' -f $module.name,$module.version)
    try {
      Uninstall-Module -Name $module.name -RequiredVersion $module.version -Force:$Force -ErrorAction Stop
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

이 스크립트를 실행하면 제거하고 있는 각 하위 모듈의 이름 및 버전이 표시됩니다.

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

제거하려는 Azure PowerShell의 모든 버전에 대해 이 명령을 실행합니다.