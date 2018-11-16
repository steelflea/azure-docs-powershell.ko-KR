---
title: PowerShellGet으로 Azure PowerShell 설치
description: PowerShellGet으로 Azure PowerShell을 설치 하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: c4af07816aaa6713d67e3349a45880f8cc22c80a
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/15/2018
ms.locfileid: "51574501"
---
# <a name="install-azure-powershell-with-powershellget"></a><span data-ttu-id="d3161-103">PowerShellGet으로 Azure PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="d3161-103">Install Azure PowerShell with PowerShellGet</span></span>

<span data-ttu-id="d3161-104">이 문서에서는 PowerShellGet을 사용하여 Azure PowerShell 모듈을 설치하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="d3161-105">Az의 미리보기 릴리스에서는 다른 설치 방법이 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-105">For the preview release of Az, no other install methods are supported.</span></span> 

## <a name="requirements"></a><span data-ttu-id="d3161-106">요구 사항</span><span class="sxs-lookup"><span data-stu-id="d3161-106">Requirements</span></span>

<span data-ttu-id="d3161-107">Azure PowerShell은 Windows의 PowerShell 5.x 또는 모든 플랫폼의 PowerShell 6.x에서 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-107">Azure PowerShell works with either PowerShell 5.x on Windows, or PowerShell 6.x on any platform.</span></span> <span data-ttu-id="d3161-108">시스템의 PowerShell 버전을 확인하려면 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-108">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="d3161-109">오래된 버전이 있거나 PowerShell을 설치해야 하는 경우 [다양한 버전의 PowerShell 설치](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d3161-109">If you have an outdated version or need to install PowerShell, see [Installing various versions of PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span></span> <span data-ttu-id="d3161-110">플랫폼에 대한 설치 정보는 해당 페이지에 링크되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-110">Install information for your platform is linked from that page.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="d3161-111">Azure PowerShell 모듈 설치</span><span class="sxs-lookup"><span data-stu-id="d3161-111">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="d3161-112">한 시스템에 `AzureRM` 및 `Az` 모듈을 동시에 설치하지 않아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-112">You shouldn't have both the `AzureRM` and `Az` modules installed on a system at the same time.</span></span> <span data-ttu-id="d3161-113">`Az` 모듈을 설치하려면 `AzureRM`을 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-113">In order to install the `Az` module, `AzureRM` must be uninstalled.</span></span> <span data-ttu-id="d3161-114">이를 수행하는 방법에 대한 지침은 [Azure PowerShell 모듈(AzureRM) 제거](uninstall-azurerm-ps.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d3161-114">For instructions on how to do that, see [Uninstall the Azure PowerShell module (AzureRM)](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="d3161-115">모듈을 전역 범위에 설치하려면 상승된 권한으로 PowerShell 갤러리에서 모듈을 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-115">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="d3161-116">Azure PowerShell을 설치하려면 상승된 세션에서 다음 명령을 실행합니다(Windows에서는 "관리자 권한으로 실행", macOS 또는 Linux에서는 슈퍼 사용자 권한으로 실행).</span><span class="sxs-lookup"><span data-stu-id="d3161-116">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="d3161-117">관리자 권한에 대한 액세스 권한이 없으면 `-Scope` 인수를 추가하여 현재 사용자를 위해 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-117">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="d3161-118">기본적으로 PowerShell 갤러리는 PowerShellGet에 대한 신뢰할 수 있는 리포지토리로 구성되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-118">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="d3161-119">PSGallery를 처음 사용할 때는 다음과 같은 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-119">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="d3161-120">설치를 계속하려면 `Yes` 또는 `Yes to All`로 답변합니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-120">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="d3161-121">`Az` 모듈은 Azure PowerShell cmdlet의 롤업 모듈입니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-121">The `Az` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="d3161-122">설치하면 사용 가능한 모든 Azure Resource Manager 모듈이 다운로드되고 cmdlet을 사용할 수 있게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-122">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="d3161-123">로그인</span><span class="sxs-lookup"><span data-stu-id="d3161-123">Sign in</span></span>

<span data-ttu-id="d3161-124">Azure PowerShell을 사용하여 작업을 시작 하려면 [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet을 사용하여 현재 PowerShell 세션에 `Az`을 로드한 후 Azure 자격 증명으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-124">To start working with Azure PowerShell, you need to load `Az` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

<span data-ttu-id="d3161-125">모든 새 PowerShell 세션에 대해 이러한 단계를 반복해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-125">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="d3161-126">`Az` 모듈을 자동으로 가져오려면 PowerShell 프로필을 설정해야 하며, 프로필 설정은 [프로필 정보](/powershell/module/microsoft.powershell.core/about/about_profiles)에서 알아볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-126">Automatically importing the `Az` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="d3161-127">세션 간에 Azure 로그인을 유지하는 방법을 보려면 [PowerShell 세션간에 사용자 자격 증명 유지](context-persistence.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d3161-127">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="d3161-128">Azure PowerShell 모듈 업데이트</span><span class="sxs-lookup"><span data-stu-id="d3161-128">Update the Azure PowerShell module</span></span>

<span data-ttu-id="d3161-129">[Update-Module](/powershell/module/powershellget/update-module)을 실행하여 Azure PowerShell 설치를 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-129">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="d3161-130">이 명령은 이전 버전을 제거하지 __않습니다__.</span><span class="sxs-lookup"><span data-stu-id="d3161-130">This command does __not__ uninstall earlier versions.</span></span>

```powershell-interactive
Update-Module -Name Az
```

<span data-ttu-id="d3161-131">Azure PowerShell의 이전 버전을 시스템에서 제거하려면, [Azure PowerShell 모듈 제거](uninstall-azurerm-ps.md)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-131">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="d3161-132">여러 버전의 Azure PowerShell 사용</span><span class="sxs-lookup"><span data-stu-id="d3161-132">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="d3161-133">Azure PowerShell은 버전을 2개 이상 설치할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-133">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="d3161-134">여러 버전의 Azure PowerShell이 설치되어 있는지 확인하려면 다음 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-134">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-Module -Name Az -List | select Name,Version
```

<span data-ttu-id="d3161-135">Azure PowerShell의 버전을 제거하려면 [Azure PowerShell 모듈 제거](uninstall-azurerm-ps.md)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-135">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="d3161-136">`Install-Module` 또는 `Import-Module`과 함께 `-RequiredVersion` 인수를 사용하여 `Az` 모듈의 특정 버전을 로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-136">You can load a specific version of the `Az` module by using the `-RequiredVersion` argument with `Install-Module` or `Import-Module`:</span></span>

```powershell-interactive
Install-Module -Name Az -RequiredVersion 0.4.0
Import-Module -Name Az -RequiredVersion 0.4.0
```

<span data-ttu-id="d3161-137">두 개 이상의 모듈 버전이 설치되어 있는 경우, 가져올 때 기본적으로 최신 버전이 로드됩니다.</span><span class="sxs-lookup"><span data-stu-id="d3161-137">If you have more than one version of the module installed, the latest version is loaded by default when importing.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="d3161-138">피드백 제공</span><span class="sxs-lookup"><span data-stu-id="d3161-138">Provide feedback</span></span>

<span data-ttu-id="d3161-139">Azure Powershell 사용 중 버그 발생 시, [ GitHub에서 문제를 제출](https://github.com/Azure/azure-powershell/issues)하세요.</span><span class="sxs-lookup"><span data-stu-id="d3161-139">If you find a bug when using Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="d3161-140">명령줄에서 피드백을 제공하려면 [Send-Feedback](/powershell/module/az.profile/send-feedback) cmdlet을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="d3161-140">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d3161-141">다음 단계</span><span class="sxs-lookup"><span data-stu-id="d3161-141">Next Steps</span></span>

<span data-ttu-id="d3161-142">Azure PowerShell 사용을 시작하려면, [Azure PowerShell 시작](get-started-azureps.md)을 참조하여 모듈 및 모듈의 기능에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="d3161-142">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>