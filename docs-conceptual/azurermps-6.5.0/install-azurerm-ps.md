---
title: PowerShellGet으로 Azure PowerShell을 설치
description: PowerShellGet으로 Azure PowerShell을 설치 하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/15/2018
ms.openlocfilehash: 50b05e5f25b6e3e1c815f6b26f1b53b84cd0b7da
ms.sourcegitcommit: 8b882d1c27d9e323447ff85f56d11bbf5e244d7f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/18/2018
ms.locfileid: "39110894"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a><span data-ttu-id="3174c-103">PowerShellGet으로 Azure PowerShell을 설치</span><span class="sxs-lookup"><span data-stu-id="3174c-103">Install Azure PowerShell on Windows with PowerShellGet</span></span>

<span data-ttu-id="3174c-104">이 문서에서는 Windows 환경에서 PowerShellGet을 사용하여 Azure PowerShell 모듈을 설치하는 단계를 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-104">This article explains the steps to install the Azure PowerShell modules in a Windows environment using PowerShellGet.</span></span> <span data-ttu-id="3174c-105">PowerShellGet 및 모듈 관리는 Azure PowerShell을 설치하는 더 좋은 방법이지만 대신 웹 플랫폼 설치 관리자 또는 MSI 패키지로 설치하려는 경우 [다른 설치 방법](other-install.md)을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-105">PowerShellGet and module management is the preferred way to install Azure PowerShell but if you would rather install with the Web Platform Installer or MSI package, see [Other installation methods](other-install.md).</span></span>

<span data-ttu-id="3174c-106">Azure PowerShell을 다른 플랫폼에서 설치하는 지침에 대해서는, [macOS 및 Linux에서 Azure PowerShell 설치 및 구성](install-azurermps-maclinux.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="3174c-106">For instructions to install Azure PowerShell on other platforms, see [Install and configure Azure PowerShell on macOS and Linux](install-azurermps-maclinux.md).</span></span>

<span data-ttu-id="3174c-107">Azure 클래식 배포 모델은 본 버전의 Azure PowerShell에서 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-107">The Azure classic deployment model is not supported by this version of Azure PowerShell.</span></span> <span data-ttu-id="3174c-108">클래식 배포에 대한 지원은 [Azure PowerShell Service Management 모듈 설치](/powershell/azure/servicemanagement/install-azure-ps) 지침을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-108">For support for classic deployments, follow the instructions in [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

## <a name="requirements"></a><span data-ttu-id="3174c-109">요구 사항</span><span class="sxs-lookup"><span data-stu-id="3174c-109">Requirements</span></span>

<span data-ttu-id="3174c-110">Azure PowerShell 버전 6.0부터 Azure PowerShell은 PowerShell 버전 5.0이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-110">Starting with Azure PowerShell version 6.0, Azure PowerShell requires PowerShell version 5.0.</span></span> <span data-ttu-id="3174c-111">시스템의 PowerShell 버전을 확인하려면 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-111">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell
$PSVersionTable.PSVersion
```

<span data-ttu-id="3174c-112">만료된 버전을 사용하는 경우 [기존 Windows PowerShell 업그레이드](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-112">If you have an outdated version, see [Upgrading existing Windows PowerShell](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3174c-113">이 문서에서 설명된 모듈인 AzureRM에서는 .NET Framework를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-113">The module described in this document, AzureRM, uses .NET Framework.</span></span> <span data-ttu-id="3174c-114">이렇게 하면 .NET Core를 사용하는 PowerShell 6.0과 호환되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-114">This makes it incompatible with PowerShell 6.0, which uses .NET Core.</span></span> <span data-ttu-id="3174c-115">PowerShell 6.0을 사용하는 경우, [macOS 및 Linux에 대한 설치 지침](install-azurermps-maclinux.md)을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-115">If you are using PowerShell 6.0, follow the [installation instructions for macOS and Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="3174c-116">Azure PowerShell 모듈 설치</span><span class="sxs-lookup"><span data-stu-id="3174c-116">Install the Azure PowerShell module</span></span>

<span data-ttu-id="3174c-117">PowerShell 갤러리에서 모듈을 설치하려면 상승된 권한이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-117">You need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="3174c-118">Azure PowerShell을 설치하려면 승격된 세션에서 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-118">To install Azure PowerShell, run the following command in an elevated session:</span></span>

```powershell
Install-Module -Name AzureRM
```

> [!NOTE]
> <span data-ttu-id="3174c-119">NuGet 2.8.5.201 이전 버전을 사용하는 경우 최신 버전의 NuGet을 다운로드하여 설치하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-119">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="3174c-120">기본적으로 PowerShell 갤러리는 PowerShellGet에 대한 신뢰할 수 있는 리포지토리로 구성되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-120">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="3174c-121">PSGallery를 처음 사용할 때는 다음과 같은 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-121">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="3174c-122">설치를 계속하려면 `Yes` 또는 `Yes to All`로 답변합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-122">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="3174c-123">`AzureRM` 모듈은 Azure PowerShell cmdlet의 롤업 모듈입니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-123">The `AzureRM` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="3174c-124">설치하면 사용 가능한 모든 Azure Resource Manager 모듈이 다운로드되고 cmdlet을 사용할 수 있게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-124">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="3174c-125">로그인</span><span class="sxs-lookup"><span data-stu-id="3174c-125">Sign in</span></span>

<span data-ttu-id="3174c-126">Azure PowerShell을 사용하여 작업을 시작 하려면 [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet을 사용하여 현재 PowerShell 세션에 `AzureRM`을 로드한 후 Azure 자격 증명으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-126">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="3174c-127">모든 새 PowerShell 세션에 대해 이러한 단계를 반복해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-127">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="3174c-128">`AzureRM` 모듈을 자동으로 가져오려면 PowerShell 프로필을 설정해야 하며, 프로필 설정은 [프로필 정보](/powershell/module/microsoft.powershell.core/about/about_profiles)에서 알아볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-128">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="3174c-129">Azure 로그인을 세션 간에 유지하는 방법을 알아보려면 [PowerShell 세션 간에 사용자 자격 증명 유지](context-persistence.md)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-129">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="3174c-130">Azure PowerShell 모듈 업데이트</span><span class="sxs-lookup"><span data-stu-id="3174c-130">Update the Azure PowerShell module</span></span>

<span data-ttu-id="3174c-131">[Update-Module](/powershell/module/powershellget/update-module)을 실행하여 Azure PowerShell 설치를 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-131">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="3174c-132">이 명령은 이전 버전을 제거하지 __않습니다__.</span><span class="sxs-lookup"><span data-stu-id="3174c-132">This command does __not__ uninstall earlier versions.</span></span>

```powershell
Update-Module -Name AzureRM
```

<span data-ttu-id="3174c-133">Azure PowerShell의 이전 버전을 시스템에서 제거하려면, [Azure PowerShell 모듈 제거](uninstall-azurerm-ps.md)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-133">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="3174c-134">여러 버전의 Azure PowerShell 사용</span><span class="sxs-lookup"><span data-stu-id="3174c-134">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="3174c-135">여러 버전의 Azure PowerShell을 설치하는 것은 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-135">It's possible to install multiple versions of Azure PowerShell.</span></span> <span data-ttu-id="3174c-136">온-프레미스 Azure Stack 리소스로 작업하거나 PowerShell 5.0으로 업데이트할 수 없는 이전 버전의 Windows를 실행하거나 Azure 클래식 배포 모델을 사용하는 경우 둘 이상의 버전이 필요할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-136">You might need more than one version if you work with on-premises Azure Stack resources, run an older version of Windows that you can't update to PowerShell 5.0, or use the Azure classic deployment model.</span></span> <span data-ttu-id="3174c-137">이전 버전을 설치하려면 `-RequiredVersion` 인수를 설치 시 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-137">To install an older version, provide the `-RequiredVersion` argument when installing.</span></span>

```powershell
# Install version 1.2.9 of Azure PowerShell
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

<span data-ttu-id="3174c-138">Azure PowerShell 모듈 로드 시, 기본으로 최신 버전이 로드됩니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-138">When loading the Azure PowerShell module the latest version is loaded by default.</span></span> <span data-ttu-id="3174c-139">다른 버전을 로드하려면 `-RequiredVersion` 인수를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="3174c-139">To load a different version, provide the `-RequiredVersion` argument.</span></span>

```powershell
# Load version 1.2.9 of Azure PowerShell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

## <a name="provide-feedback"></a><span data-ttu-id="3174c-140">피드백 제공</span><span class="sxs-lookup"><span data-stu-id="3174c-140">Provide feedback</span></span>

<span data-ttu-id="3174c-141">Azure Powershell 사용 중 버그 발생 시, [ GitHub에서 문제 제출](https://github.com/Azure/azure-powershell/issues)을 해 주십시오.</span><span class="sxs-lookup"><span data-stu-id="3174c-141">If you find a bug when using Azure Powershell, please [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="3174c-142">명령줄에서 피드백을 제공하려면 [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="3174c-142">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3174c-143">다음 단계</span><span class="sxs-lookup"><span data-stu-id="3174c-143">Next Steps</span></span>

<span data-ttu-id="3174c-144">Azure PowerShell 사용을 시작하려면, [Azure PowerShell 시작](get-started-azureps.md)을 참조하여 모듈 및 모듈의 기능에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="3174c-144">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>