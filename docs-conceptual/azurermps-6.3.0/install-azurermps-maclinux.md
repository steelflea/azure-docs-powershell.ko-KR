---
title: macOS 또는 Linux에 Azure PowerShell 설치
description: macOS 또는 Linux에 Azure PowerShell 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: a54af4b28642fe7b8623550fb05dff33e5c4a7f6
ms.sourcegitcommit: 4c775721461210431bd913f28d1f1e6f1976880a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/28/2018
ms.locfileid: "37091336"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="c7723-103">macOS 또는 Linux에 Azure PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="c7723-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="c7723-104">Windows 이외의 플랫폼에서도 PowerShell Core v6에서 Azure PowerShell을 실행할 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="c7723-105">본 버전의 PowerShell은 .NET Core를 지원하는 모든 플랫폼에서 사용할 수 있도록 빌드되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="c7723-106">이러한 플랫폼에서 작동하기 위해, Azure PowerShell의 특별 .NET Core 버전이 사용 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-106">To work with these platforms, there's a special .NET Core version of Azure PowerShell available.</span></span>

> [!NOTE]
> <span data-ttu-id="c7723-107">이때 PowerShell Core v6과 .NET Core용 Azure PowerShell은 아직 베타 버전입니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-107">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="c7723-108">이러한 제품에 대한 지원은 제한됩니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-108">Support for these products is limited.</span></span> <span data-ttu-id="c7723-109">문제가 있거나 버그를 발견한 경우 GitHub에서 문제를 제출하십시오.</span><span class="sxs-lookup"><span data-stu-id="c7723-109">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="c7723-110">PowerShell Core v6에 대한 문제</span><span class="sxs-lookup"><span data-stu-id="c7723-110">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="c7723-111">Azure PowerShell에 대한 문제</span><span class="sxs-lookup"><span data-stu-id="c7723-111">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a><span data-ttu-id="c7723-112">PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="c7723-112">Install PowerShell Core</span></span>

<span data-ttu-id="c7723-113">PowerShell Core를 위한 설치 지침은 macOS나 대부분의 Linux 배포와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-113">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="c7723-114">자세한 지침은 다음 문서에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-114">Detailed instructions can be found in the following articles:</span></span>

- [<span data-ttu-id="c7723-115">macOS에 PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="c7723-115">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
- [<span data-ttu-id="c7723-116">Linux에 PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="c7723-116">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a><span data-ttu-id="c7723-117">.NET Core용 Azure PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="c7723-117">Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="c7723-118">PowerShell Core는 PowerShellGet 모듈이 이미 설치되어 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-118">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="c7723-119">PowerShell에서 모듈을 설치하려면 상승된 권한이 필요하므로 세션을 슈퍼 사용자로 시작해야 합니다:</span><span class="sxs-lookup"><span data-stu-id="c7723-119">Installation of modules in PowerShell requires elevated privileges, so you'll need to start your session as superuser:</span></span>

```bash
sudo pwsh
```

<span data-ttu-id="c7723-120">Azure PowerShell을 설치하려면 다음 명령을 실행합니다:</span><span class="sxs-lookup"><span data-stu-id="c7723-120">To install Azure PowerShell, run the following command:</span></span>

```powershell
Install-Module AzureRM.NetCore
```

> [!IMPORTANT]
> <span data-ttu-id="c7723-121">다른 아티클에서 설명된 `AzureRM` 모듈은 .NET Core용으로 빌드된 것이 아니며 PowerShell Core와 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-121">The `AzureRM` module detailed in other articles is not built for .NET Core and will not work with PowerShell Core.</span></span> <span data-ttu-id="c7723-122">`AzureRM`, `AzureRM.NetCore` 둘 다 동일한 cmdlet 이름을 사용하므로 롤업 모듈의 이름과 빌드되는 .NET 버전에 따라 달라집니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-122">Both `AzureRM` and `AzureRM.NetCore` use the same cmdlet names, so the only difference is the name of the rollup module and which .NET version they are built against.</span></span>

<span data-ttu-id="c7723-123">기본적으로 PowerShell 갤러리는 PowerShellGet에 대한 신뢰할 수 있는 리포지토리로 구성되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-123">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="c7723-124">PSGallery를 처음 사용할 때는 다음과 같은 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-124">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="c7723-125">설치를 계속하려면 `Yes` 또는 `Yes to All`로 답변합니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-125">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="sign-in"></a><span data-ttu-id="c7723-126">로그인</span><span class="sxs-lookup"><span data-stu-id="c7723-126">Sign in</span></span>

<span data-ttu-id="c7723-127">Azure PowerShell을 사용하여 작업을 시작 하려면 [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet을 사용하여 PowerShell 세션에 `AzureRM.Netcore`을 로드한 후 Azure 자격 증명으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-127">To start working with Azure PowerShell, you need to load `AzureRM.Netcore` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="c7723-128">모듈 가져오기는 상승된 권한이 필요하지 __않습니다__.</span><span class="sxs-lookup"><span data-stu-id="c7723-128">Importing a module does __not__ require elevated privileges.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM.Netcore
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="c7723-129">모든 새 PowerShell 세션에 대해 이러한 단계를 반복해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-129">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="c7723-130">`AzureRM` 모듈을 자동으로 가져오려면 PowerShell 프로필을 설정해야 하며, 프로필 설정은 [프로필 정보](/powershell/module/microsoft.powershell.core/about/about_profiles)에서 알아볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-130">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="c7723-131">macOS 및 Linux에서, `$Profile` 환경 변수를 통해 프로필 작업을 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-131">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="c7723-132">Azure 로그인을 세션 간에 유지하는 방법을 알아보려면 [PowerShell 세션 간에 사용자 자격 증명 유지](context-persistence.md)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-132">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="c7723-133">사용할 수 있는 cmdlet</span><span class="sxs-lookup"><span data-stu-id="c7723-133">Available cmdlets</span></span>

<span data-ttu-id="c7723-134">.NET Core용 Azure PowerShell 모듈은 아직 개발 중입니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-134">The Azure PowerShell modules for .NET Core are still in development.</span></span> <span data-ttu-id="c7723-135">이러한 모듈은 모듈의 Windows 버전에 대해 사용할 수 있는 cmdlet의 집합을 모두 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-135">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="c7723-136">다음 함수는 AzureRM.Netcore 모듈에서 구현됩니다.</span><span class="sxs-lookup"><span data-stu-id="c7723-136">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="c7723-137">계정 관리</span><span class="sxs-lookup"><span data-stu-id="c7723-137">Account management</span></span>
  - <span data-ttu-id="c7723-138">Microsoft 계정, 조직 계정 또는 Microsoft Azure Active Directory를 통해 서비스 사용자로 로그인</span><span class="sxs-lookup"><span data-stu-id="c7723-138">Sign in with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  - <span data-ttu-id="c7723-139">Save-AzureRmContext로 자격 증명을 디스크에 저장하고 Import-AzureRmContext를 사용하여 저장된 자격 증명 로드</span><span class="sxs-lookup"><span data-stu-id="c7723-139">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="c7723-140">Environment</span><span class="sxs-lookup"><span data-stu-id="c7723-140">Environment</span></span>
  - <span data-ttu-id="c7723-141">다른 기본 Microsoft Azure 환경 가져오기</span><span class="sxs-lookup"><span data-stu-id="c7723-141">Get the different out-of-box Microsoft Azure environments</span></span>
  - <span data-ttu-id="c7723-142">사용자 지정 환경 추가/설정/제거(예: Azure Stack 또는 Windows Azure 팩 환경)</span><span class="sxs-lookup"><span data-stu-id="c7723-142">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="c7723-143">리소스 관리자 및 서비스 관리 인터페이스를 사용하여 Azure 서비스용 평면 cmdlet 관리</span><span class="sxs-lookup"><span data-stu-id="c7723-143">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  - <span data-ttu-id="c7723-144">Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="c7723-144">Virtual Machine</span></span>
  - <span data-ttu-id="c7723-145">App Service(웹 사이트)</span><span class="sxs-lookup"><span data-stu-id="c7723-145">App Service (Websites)</span></span>
  - <span data-ttu-id="c7723-146">SQL Database</span><span class="sxs-lookup"><span data-stu-id="c7723-146">SQL Database</span></span>
  - <span data-ttu-id="c7723-147">Storage</span><span class="sxs-lookup"><span data-stu-id="c7723-147">Storage</span></span>
  - <span data-ttu-id="c7723-148">네트워크</span><span class="sxs-lookup"><span data-stu-id="c7723-148">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="c7723-149">다음 단계</span><span class="sxs-lookup"><span data-stu-id="c7723-149">Next Steps</span></span>

<span data-ttu-id="c7723-150">Azure PowerShell 사용에 대한 자세한 내용은 [Azure PowerShell 시작](get-started-azureps.md) 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c7723-150">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
