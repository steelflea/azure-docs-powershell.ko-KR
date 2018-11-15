---
title: Azure PowerShell 제거
description: Azure PowerShell의 전체 제거를 수행하는 방법
ms.date: 09/11/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 3543dbb692a41bd3b417bb3d771e67c52d57c340
ms.sourcegitcommit: ac4b53bb42a25aae013a9d8cd9ae98ada9397274
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/08/2018
ms.locfileid: "51274656"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="da2d5-103">Azure PowerShell 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="da2d5-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="da2d5-104">이 문서에서는 Azure PowerShell의 이전 버전을 제거하거나 시스템에서 완전히 제거하는 방법을 알려줍니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="da2d5-105">Azure PowerShell을 완전히 제거하기로 한 경우 [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet을 통해 몇 가지 피드백을 보내주세요.</span><span class="sxs-lookup"><span data-stu-id="da2d5-105">If you've decided to completely uninstall the Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="da2d5-106">버그가 발생한 경우 [GitHub 문제를 제출](https://github.com/azure/azure-powershell/issues)해주시면 감사하겠습니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="da2d5-107">PowerShell에서 제거하기</span><span class="sxs-lookup"><span data-stu-id="da2d5-107">Uninstall from PowerShell</span></span>

<span data-ttu-id="da2d5-108">PowerShellGet을 사용하여 Azure PowerShell을 설치하는 경우 [Uninstall-module](/powershell/module/powershellget/uninstall-module) cmdlet을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-108">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="da2d5-109">그러나 `Uninstall-Module`은 모듈 중 하나만 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-109">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="da2d5-110">Azure PowerShell을 완전히 제거하려면 각 모듈을 개별적으로 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-110">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="da2d5-111">2개 이상의 Azure PowerShell 버전을 설치한 경우 제거가 복잡할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-111">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="da2d5-112">다음 스크립트는 PowerShell 갤러리를 쿼리하여 종속 하위 모듈의 목록을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-112">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="da2d5-113">그런 다음 스크립트는 올바른 버전의 각 하위 모듈을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-113">Then, the script uninstalls the correct version of each submodule.</span></span>

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

<span data-ttu-id="da2d5-114">이 함수를 사용하려면 코드를 복사하고 PowerShell 세션에 붙여넣습니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-114">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="da2d5-115">다음 예제에서는 이전 버전의 Azure PowerShell을 제거하는 함수를 실행하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-115">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="da2d5-116">이 스크립트를 실행하면 제거하고 있는 각 하위 모듈의 이름 및 버전이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-116">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

<span data-ttu-id="da2d5-117">제거하려는 Azure PowerShell의 모든 버전에 대해 이 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-117">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span> <span data-ttu-id="da2d5-118">편의를 위해, 다음 스크립트는 최신 버전을 __제외한__ 모든 AzureRM 버전을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-118">For convenience, the following script will uninstall all versions of AzureRM __except__ for the latest.</span></span>

```powershell-interactive
$versions = (get-installedmodule AzureRM -AllVersions | Select-Object Version)
$versions[1..($versions.Length-1)]  | foreach { Uninstall-AllModules -TargetModule AzureRM -Version ($_.Version) -Force }
```

## <a name="uninstall-msi"></a><span data-ttu-id="da2d5-119">MSI 제거</span><span class="sxs-lookup"><span data-stu-id="da2d5-119">Uninstall MSI</span></span>

<span data-ttu-id="da2d5-120">MSI 패키지를 사용하여 Azure PowerShell을 설치한 경우 PowerShell이 아닌 Windows 시스템을 통해 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-120">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="da2d5-121">플랫폼</span><span class="sxs-lookup"><span data-stu-id="da2d5-121">Platform</span></span> | <span data-ttu-id="da2d5-122">지침</span><span class="sxs-lookup"><span data-stu-id="da2d5-122">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="da2d5-123">윈도우 10</span><span class="sxs-lookup"><span data-stu-id="da2d5-123">Windows 10</span></span> | <span data-ttu-id="da2d5-124">시작 > 설정 > 앱</span><span class="sxs-lookup"><span data-stu-id="da2d5-124">Start > Settings > Apps</span></span> |
| <span data-ttu-id="da2d5-125">Windows 7</span><span class="sxs-lookup"><span data-stu-id="da2d5-125">Windows 7</span></span> </br><span data-ttu-id="da2d5-126">Windows 8</span><span class="sxs-lookup"><span data-stu-id="da2d5-126">Windows 8</span></span> | <span data-ttu-id="da2d5-127">시작>제어판 > 프로그램 > 프로그램 제거</span><span class="sxs-lookup"><span data-stu-id="da2d5-127">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="da2d5-128">이 화면의 프로그램 목록에서 "Azure PowerShell"이 보여야 여기에서 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da2d5-128">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>