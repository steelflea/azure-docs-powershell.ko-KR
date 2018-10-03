---
title: macOS 또는 Linux에 Azure PowerShell 설치
description: macOS 또는 Linux에 Azure PowerShell 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: f014d62e898da195a38052db6b7e37a2cd96dfdd
ms.sourcegitcommit: 3a02e0c85c83de873981dd392500bc82c1cf9286
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/24/2018
ms.locfileid: "46560119"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="a3820-103">macOS 또는 Linux에 Azure PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="a3820-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="a3820-104">Windows 이외의 플랫폼에서도 PowerShell Core v6에서 Azure PowerShell을 실행할 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="a3820-105">본 버전의 PowerShell은 .NET Core를 지원하는 모든 플랫폼에서 사용할 수 있도록 빌드되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="a3820-106">이러한 플랫폼에서 작동하기 위해, Azure PowerShell의 .NET 표준 버전이 사용 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-106">To work with these platforms, there's a .NET Standard version of Azure PowerShell available.</span></span>

> [!NOTE]
> <span data-ttu-id="a3820-107">이때 PowerShell Core v6과 .NET Core용 Azure PowerShell은 아직 베타 버전입니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-107">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="a3820-108">이러한 제품에 대한 지원은 제한됩니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-108">Support for these products is limited.</span></span> <span data-ttu-id="a3820-109">문제가 있거나 버그를 발견한 경우 GitHub에서 문제를 제출하십시오.</span><span class="sxs-lookup"><span data-stu-id="a3820-109">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="a3820-110">PowerShell Core v6에 대한 문제</span><span class="sxs-lookup"><span data-stu-id="a3820-110">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="a3820-111">Azure PowerShell에 대한 문제</span><span class="sxs-lookup"><span data-stu-id="a3820-111">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a><span data-ttu-id="a3820-112">PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="a3820-112">Install PowerShell Core</span></span>

<span data-ttu-id="a3820-113">PowerShell Core를 위한 설치 지침은 macOS나 대부분의 Linux 배포와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-113">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="a3820-114">자세한 지침은 다음 문서에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-114">Detailed instructions can be found in the following articles:</span></span>

* [<span data-ttu-id="a3820-115">macOS에 PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="a3820-115">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [<span data-ttu-id="a3820-116">Linux에 PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="a3820-116">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a><span data-ttu-id="a3820-117">.NET Core용 Azure PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="a3820-117">Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="a3820-118">PowerShell Core는 PowerShellGet 모듈이 이미 설치되어 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-118">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="a3820-119">PowerShell에서 모듈을 설치하려면 상승된 권한이 필요하므로 세션을 슈퍼 사용자로 시작해야 합니다:</span><span class="sxs-lookup"><span data-stu-id="a3820-119">Installation of modules in PowerShell requires elevated privileges, so you'll need to start your session as superuser:</span></span>

```bash
sudo pwsh
```

<span data-ttu-id="a3820-120">Azure PowerShell을 설치하려면 다음 명령을 실행합니다:</span><span class="sxs-lookup"><span data-stu-id="a3820-120">To install Azure PowerShell, run the following command:</span></span>

```powershell
Install-Module Az
```

> [!IMPORTANT]
> <span data-ttu-id="a3820-121">다른 아티클에서 설명된 `AzureRM` 모듈은 .NET Core용으로 빌드된 것이 아니며 PowerShell Core와 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-121">The `AzureRM` module detailed in other articles is not built for .NET Core and will not work with PowerShell Core.</span></span> <span data-ttu-id="a3820-122">`Az` 모듈에는 모든 `AzureRM` cmdlet에 대한 명령 별칭이 포함되어 있으므로 `AzureRM`의 모든 설명서가 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-122">The `Az` modules contain command aliases for all `AzureRM` cmdlets, so all of the documentation for `AzureRM` applies.</span></span>

<span data-ttu-id="a3820-123">기본적으로 PowerShell 갤러리는 PowerShellGet에 대한 신뢰할 수 있는 리포지토리로 구성되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-123">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="a3820-124">PSGallery를 처음 사용할 때는 다음과 같은 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-124">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="a3820-125">설치를 계속하려면 `Yes` 또는 `Yes to All`로 답변합니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-125">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="sign-in"></a><span data-ttu-id="a3820-126">로그인</span><span class="sxs-lookup"><span data-stu-id="a3820-126">Sign in</span></span>

<span data-ttu-id="a3820-127">Azure PowerShell을 사용하여 작업을 시작 하려면 [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet을 사용하여 PowerShell 세션에 `Az`을 로드한 후 Azure 자격 증명으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-127">To start working with Azure PowerShell, you need to load `Az` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="a3820-128">모듈 가져오기는 상승된 권한이 필요하지 __않습니다__.</span><span class="sxs-lookup"><span data-stu-id="a3820-128">Importing a module does __not__ require elevated privileges.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="a3820-129">모든 새 PowerShell 세션에 대해 이러한 단계를 반복해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-129">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="a3820-130">`Az` 모듈을 자동으로 가져오려면 PowerShell 프로필을 설정해야 하며, 프로필 설정은 [프로필 정보](/powershell/module/microsoft.powershell.core/about/about_profiles)에서 알아볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-130">Automatically importing the `Az` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="a3820-131">macOS 및 Linux에서, `$Profile` 환경 변수를 통해 프로필 작업을 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a3820-131">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="a3820-132">세션 간에 Azure 로그인을 유지하는 방법을 보려면 [PowerShell 세션간에 사용자 자격 증명 유지](context-persistence.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a3820-132">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="a3820-133">다음 단계</span><span class="sxs-lookup"><span data-stu-id="a3820-133">Next Steps</span></span>

<span data-ttu-id="a3820-134">Azure PowerShell 사용에 대한 자세한 내용은 [Azure PowerShell 시작](get-started-azureps.md) 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a3820-134">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
