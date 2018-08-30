---
title: Azure PowerShell 제거
description: Azure PowerShell의 전체 제거를 수행하는 방법
ms.date: 06/20/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 92af0fdd8db451e2f0f092d66a3e296ad8d6a09e
ms.sourcegitcommit: 9cb98f055a0525c2061f65149965d5e7c3e03ddc
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/30/2018
ms.locfileid: "43117384"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="4f1a1-103">Azure PowerShell 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="4f1a1-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="4f1a1-104">이 문서에서는 Azure PowerShell의 이전 버전을 제거하거나 시스템에서 완전히 제거하는 방법을 알려줍니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="4f1a1-105">Azure PowerShell을 완전히 제거하기로 한 경우 [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet을 통해 몇 가지 피드백을 보내주세요.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-105">If you've decided to completely uninstall the Azure PowerShell, please give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="4f1a1-106">버그가 발생한 경우 [GitHub 문제를 제출](https://github.com/azure/azure-powershell/issues)해주시면 감사하겠습니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-msi"></a><span data-ttu-id="4f1a1-107">MSI 제거</span><span class="sxs-lookup"><span data-stu-id="4f1a1-107">Uninstall MSI</span></span>

<span data-ttu-id="4f1a1-108">MSI 패키지를 사용하여 Azure PowerShell을 설치한 경우 PowerShell이 아닌 Windows 시스템을 통해 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-108">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="4f1a1-109">플랫폼</span><span class="sxs-lookup"><span data-stu-id="4f1a1-109">Platform</span></span> | <span data-ttu-id="4f1a1-110">지침</span><span class="sxs-lookup"><span data-stu-id="4f1a1-110">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="4f1a1-111">윈도우 10</span><span class="sxs-lookup"><span data-stu-id="4f1a1-111">Windows 10</span></span> | <span data-ttu-id="4f1a1-112">시작 > 설정 > 앱</span><span class="sxs-lookup"><span data-stu-id="4f1a1-112">Start > Settings > Apps</span></span> |
| <span data-ttu-id="4f1a1-113">Windows 7</span><span class="sxs-lookup"><span data-stu-id="4f1a1-113">Windows 7</span></span> </br><span data-ttu-id="4f1a1-114">Windows 8</span><span class="sxs-lookup"><span data-stu-id="4f1a1-114">Windows 8</span></span> | <span data-ttu-id="4f1a1-115">시작>제어판 > 프로그램 > 프로그램 제거</span><span class="sxs-lookup"><span data-stu-id="4f1a1-115">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="4f1a1-116">이 화면의 프로그램 목록에서 "Azure PowerShell"이 보여야 여기에서 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-116">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="4f1a1-117">PowerShell에서 제거하기</span><span class="sxs-lookup"><span data-stu-id="4f1a1-117">Uninstall from PowerShell</span></span>

<span data-ttu-id="4f1a1-118">PowerShellGet을 사용하여 Azure PowerShell을 설치하는 경우 [Uninstall-module](/powershell/module/powershellget/uninstall-module) cmdlet을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-118">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="4f1a1-119">그러나 `Uninstall-Module`은 모듈 중 하나만 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-119">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="4f1a1-120">Azure PowerShell을 완전히 제거하려면 각 모듈을 개별적으로 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-120">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="4f1a1-121">여러 버전의 Azure PowerShell이 설치되어 있는 경우 제거가 복잡할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-121">Uninstallation can be complicated if you have multiple versions of Azure PowerShell installed.</span></span>

<span data-ttu-id="4f1a1-122">다음 스크립트를 사용하면 단일 버전의 Azure PowerShell을 완전히 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-122">The following script can be used to completely remove a single version of Azure PowerShell.</span></span> <span data-ttu-id="4f1a1-123">해당 스크립트는 PowerShell 갤러리를 쿼리하여 종속 하위 모듈의 목록을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-123">The script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="4f1a1-124">그런 다음 스크립트는 올바른 버전의 각 하위 모듈을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-124">Then, the script uninstalls the correct version of each submodule.</span></span>

```powershell
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

<span data-ttu-id="4f1a1-125">이 함수를 사용하려면 코드를 복사하고 PowerShell 세션에 붙여넣습니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-125">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="4f1a1-126">다음 예제에서는 이전 버전의 Azure PowerShell을 제거하는 함수를 실행하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-126">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="4f1a1-127">이 스크립트를 실행하면 제거하고 있는 각 하위 모듈의 이름 및 버전이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-127">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

<span data-ttu-id="4f1a1-128">제거하려는 Azure PowerShell의 모든 버전에 대해 이 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="4f1a1-128">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span>
