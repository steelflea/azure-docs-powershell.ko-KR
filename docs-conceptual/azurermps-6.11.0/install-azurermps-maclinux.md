---
title: macOS 또는 Linux에 Azure PowerShell 설치
description: macOS 또는 Linux에 Azure PowerShell 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/05/2018
ms.openlocfilehash: e7d27c6f6d980c54e45620b179cf2e26ffed17f0
ms.sourcegitcommit: 1f699b72bf544d92459da9d888cc0091f9415b65
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/06/2018
ms.locfileid: "50972658"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="303d5-103">macOS 또는 Linux에 Azure PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="303d5-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="303d5-104">Windows 이외의 플랫폼에서도 PowerShell Core v6에서 Azure PowerShell을 실행할 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="303d5-105">본 버전의 PowerShell은 .NET Core를 지원하는 모든 플랫폼에서 사용할 수 있도록 빌드되었습니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="303d5-106">이러한 플랫폼에서 작동하기 위해, Azure PowerShell의 .NET 표준 버전이 사용 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-106">To work with these platforms, there's a .NET Standard version of Azure PowerShell available.</span></span>

> [!NOTE]
> <span data-ttu-id="303d5-107">이때 .NET Standard에 대한 Azure PowerShell은 아직 베타입니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-107">At this time, Azure PowerShell for .NET Standard is still in beta.</span></span>
> <span data-ttu-id="303d5-108">문제가 있거나 버그를 발견한 경우 GitHub에서 문제를 제출하십시오.</span><span class="sxs-lookup"><span data-stu-id="303d5-108">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="303d5-109">Azure PowerShell에 대한 문제</span><span class="sxs-lookup"><span data-stu-id="303d5-109">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a><span data-ttu-id="303d5-110">PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="303d5-110">Install PowerShell Core</span></span>

<span data-ttu-id="303d5-111">PowerShell Core를 위한 설치 지침은 macOS나 대부분의 Linux 배포와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-111">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="303d5-112">자세한 지침은 다음 문서에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-112">Detailed instructions can be found in the following articles:</span></span>

* [<span data-ttu-id="303d5-113">macOS에 PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="303d5-113">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [<span data-ttu-id="303d5-114">Linux에 PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="303d5-114">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-standard"></a><span data-ttu-id="303d5-115">.NET 표준용 Azure PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="303d5-115">Install Azure PowerShell for .NET Standard</span></span>

> [!IMPORTANT]
> <span data-ttu-id="303d5-116">다른 아티클에서 설명된 `AzureRM` 모듈은 PowerShell Core와 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-116">The `AzureRM` module detailed in other articles does not work with PowerShell Core.</span></span>
> <span data-ttu-id="303d5-117">PowerShell Core에서 Azure PowerShell 기능을 활용하려면 `Az` 모듈을 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-117">You must install the `Az` module to get Azure PowerShell functionality in PowerShell Core.</span></span>

<span data-ttu-id="303d5-118">PowerShell Core는 PowerShellGet 모듈이 이미 설치되어 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-118">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="303d5-119">해당 명령을 사용하여 PowerShell을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-119">Start PowerShell with the command:</span></span>

```bash
pwsh
```

<span data-ttu-id="303d5-120">Azure PowerShell을 설치하려면 다음 명령을 실행합니다:</span><span class="sxs-lookup"><span data-stu-id="303d5-120">To install Azure PowerShell, run the following command:</span></span>

```powershell
Install-Module Az
```

> [!NOTE]
> <span data-ttu-id="303d5-121">모듈을 설치할 때 사용 권한 오류가 발생하면 모듈을 설치하기 위해 수퍼 사용자 모드로 PowerShell을 실행해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-121">If you encounter a permissions error when attempting to install the module, you may need to run PowerShell in superuser mode to install modules.</span></span>
>
> ```bash
> sudo pwsh
> ```

<span data-ttu-id="303d5-122">기본적으로 PowerShell 갤러리는 PowerShellGet에 대한 신뢰할 수 있는 리포지토리로 구성되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-122">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="303d5-123">PSGallery를 처음 사용할 때는 다음과 같은 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-123">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="303d5-124">설치를 계속하려면 `Yes` 또는 `Yes to All`로 답변합니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-124">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="enable-aliases"></a><span data-ttu-id="303d5-125">별칭을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="303d5-125">Enable aliases</span></span>

<span data-ttu-id="303d5-126">기존 `AzureRM` 모듈과의 호환성을 위해, 새 `Az` 모듈은 `AzureRM` cmdlet에 대해 이전 버전과 호환되는 별칭을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-126">For compatibility with the existing `AzureRM` module, the new `Az` module has the ability to create backwards compatible aliases for the `AzureRM` cmdlets.</span></span> <span data-ttu-id="303d5-127">처음으로 모듈을 사용하기 전에 다음 명령 사용하여 이러한 별칭을 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-127">Before using the module for the first time, set up these aliases with the following command:</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module Az
# Enable AzureRM aliases for the user
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="303d5-128">이 별칭은 현재 사용자에 대해서만 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-128">This sets up aliases for the current user only.</span></span> <span data-ttu-id="303d5-129">별칭을 설정하려면 `-Scope`에 제공할 수 있는 다른 값에 대한 cmdlet 도움말을 확인하십시오.</span><span class="sxs-lookup"><span data-stu-id="303d5-129">Check the cmdlet help for other values that can be provided to `-Scope` to set up the aliases.</span></span>

> [!NOTE]
> <span data-ttu-id="303d5-130">경로 위치에 대한 오류가 발생하면 로컬 시스템에 경로 위치가 있는지 확인하십시오.</span><span class="sxs-lookup"><span data-stu-id="303d5-130">If you encounter an error about a path location, make sure that it exists on your local system.</span></span> <span data-ttu-id="303d5-131">`CurrentUser` 범위에 대해, `bash`에서 다음 명령을 실행하여 이 오류를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-131">For the `CurrentUser` scope, this error can be resolved by running the following command in `bash`:</span></span>
>
> ```bash
> mkdir -p $HOME/.config/powershell
> ```

## <a name="sign-in"></a><span data-ttu-id="303d5-132">로그인</span><span class="sxs-lookup"><span data-stu-id="303d5-132">Sign in</span></span>

<span data-ttu-id="303d5-133">Azure PowerShell을 사용하여 작업을 시작 하려면 [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet을 사용하여 PowerShell 세션에 `Az`을 로드한 후 Azure 자격 증명으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-133">To start working with Azure PowerShell, you need to load `Az` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="303d5-134">모듈 가져오기는 상승된 권한이 필요하지 __않습니다__.</span><span class="sxs-lookup"><span data-stu-id="303d5-134">Importing a module does __not__ require elevated privileges.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="303d5-135">모든 새 PowerShell 세션에 대해 이러한 단계를 반복해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-135">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="303d5-136">`Az` 모듈을 자동으로 가져오려면 PowerShell 프로필을 설정해야 하며, 프로필 설정은 [프로필 정보](/powershell/module/microsoft.powershell.core/about/about_profiles)에서 알아볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-136">Automatically importing the `Az` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="303d5-137">macOS 및 Linux에서, `$Profile` 환경 변수를 통해 프로필 작업을 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="303d5-137">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="303d5-138">세션 간에 Azure 로그인을 유지하는 방법을 보려면 [PowerShell 세션간에 사용자 자격 증명 유지](context-persistence.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="303d5-138">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="303d5-139">다음 단계</span><span class="sxs-lookup"><span data-stu-id="303d5-139">Next Steps</span></span>

<span data-ttu-id="303d5-140">Azure PowerShell 사용에 대한 자세한 내용은 [Azure PowerShell 시작](get-started-azureps.md) 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="303d5-140">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
