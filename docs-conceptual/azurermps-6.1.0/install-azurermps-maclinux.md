---
title: macOS 및 Linux에서 Azure PowerShell 설치 및 구성 | Microsoft Docs
description: macOS 및 Linux에서 Azure PowerShell을 처음으로 설치하고 구성하는 방법입니다.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/12/2018
ms.openlocfilehash: e2d73f78563b550403e9fd8b66beeef431a384b6
ms.sourcegitcommit: 5971c92cb023bdd1d71fa2ad0a3b378abfbd092a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/23/2018
ms.locfileid: "34461922"
---
# <a name="install-and-configure-azure-powershell-on-macos-and-linux"></a><span data-ttu-id="927bc-103">macOS 및 Linux에서 Azure PowerShell 설치 및 구성</span><span class="sxs-lookup"><span data-stu-id="927bc-103">Install and configure Azure PowerShell on macOS and Linux</span></span>

<span data-ttu-id="927bc-104">이제 Windows 이외의 플랫폼에서도 PowerShell Core v6 및 Azure PowerShell을 설치할 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-104">It is now possible to install PowerShell Core v6 and Azure PowerShell on non-Windows platforms.</span></span>
<span data-ttu-id="927bc-105">macOS 및 Linux에 Azure PowerShell 설치 프로세스는 Windows와 다르지 않지만, PowerShell Core v6을 먼저 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-105">The process of installing Azure PowerShell on macOS and Linux is not that different from Windows, however, you must first install PowerShell Core v6.</span></span>

> [!NOTE]

> <span data-ttu-id="927bc-106">이때 PowerShell Core v6과 .NET Core용 Azure PowerShell은 아직 베타 버전입니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-106">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="927bc-107">이러한 제품에 대한 지원은 제한됩니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-107">Support for these products is limited.</span></span> <span data-ttu-id="927bc-108">문제가 있거나 버그를 발견한 경우 GitHub에서 문제를 제출하십시오.</span><span class="sxs-lookup"><span data-stu-id="927bc-108">If you have problems or discover bugs, please file Issues in GitHub.</span></span>
>
> * [<span data-ttu-id="927bc-109">PowerShell Core v6에 대한 문제</span><span class="sxs-lookup"><span data-stu-id="927bc-109">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="927bc-110">Azure PowerShell에 대한 문제</span><span class="sxs-lookup"><span data-stu-id="927bc-110">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="step-1-install-powershell-core-v6"></a><span data-ttu-id="927bc-111">1단계: PowerShell Core v6 설치</span><span class="sxs-lookup"><span data-stu-id="927bc-111">Step 1: Install PowerShell Core v6</span></span>

<span data-ttu-id="927bc-112">PowerShell Core v6 설치 프로세스는 대상 운영 체제에 따라 달라집니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-112">The process of installing PowerShell Core v6 varies depending on the target operating system.</span></span>
<span data-ttu-id="927bc-113">Windows에 PowerShell Core v6을 설치할 수 있지만 이 문서에서는 macOS 및 Linux에 설치하는 것에 초점을 둡니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-113">While it is possible to install PowerShell Core v6 on Windows, this article focuses on macOS and Linux.</span></span> <span data-ttu-id="927bc-114">Windows에서 Azure PowerShell을 사용하려는 경우 Windows용 [설치](./install-azurerm-ps.md) 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="927bc-114">If you want to use Azure PowerShell on Windows, see the [install](./install-azurerm-ps.md) article for Windows.</span></span>

<span data-ttu-id="927bc-115">Linux 또는 macOS에 **PowerShell Core v6**을 설치하는 것은 Linux 배포 및 OS 버전에 따라 달라집니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-115">Installing **PowerShell Core v6** on Linux or macOS varies depending on the Linux distribution and OS version.</span></span>
<span data-ttu-id="927bc-116">자세한 지침은 다음 문서에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-116">Detailed instructions can be found in the following articles:</span></span>

- [<span data-ttu-id="927bc-117">macOS에 PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="927bc-117">Installing PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
- [<span data-ttu-id="927bc-118">Linux에 PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="927bc-118">Installing PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="step-2-install-azure-powershell-for-net-core"></a><span data-ttu-id="927bc-119">2단계: .NET Core용 Azure PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="927bc-119">Step 2: Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="927bc-120">PowerShell Core v6은 PowerShellGet 모듈이 이미 설치되어 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-120">PowerShell Core v6 comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="927bc-121">따라서 PowerShell 갤러리에 게시된 어떤 모듈도 쉽게 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-121">This makes it easy to install any module that is published to the PowerShell Gallery.</span></span> <span data-ttu-id="927bc-122">Azure PowerShell을 설치하려면 새 PowerShell 세션을 열고 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-122">To install Azure PowerShell, open a new PowerShell session and run the following command:</span></span>

```powershell
Install-Module AzureRM.NetCore
```

## <a name="step-3-load-the-azurermnetcore-module"></a><span data-ttu-id="927bc-123">3단계: AzureRM.Netcore 모듈 로드</span><span class="sxs-lookup"><span data-stu-id="927bc-123">Step 3: Load the AzureRM.Netcore module</span></span>

<span data-ttu-id="927bc-124">모듈이 설치되면 PowerShell 세션에 모듈을 로드해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-124">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="927bc-125">모듈은 다음과 같이 `Import-Module` cmdlet을 사용하여 로드됩니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-125">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

<span data-ttu-id="927bc-126">가져오기가 완료되면 다음 명령을 사용하여 Azure에 로그인을 시도하여 새로 설치한 모듈을 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-126">After the import completes, you can test your newly installed and module by attempting to sign into Azure using the following command:</span></span>

```powershell
Connect-AzureRmAccount
```

<span data-ttu-id="927bc-127">위의 명령을 실행하면 `https://aka.ms/devicelogin`으로 이동하여 제공된 코드를 입력하라는 메시지가 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-127">The above command should prompt you to go to `https://aka.ms/devicelogin` and enter the provided code.</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="927bc-128">사용할 수 있는 cmdlet</span><span class="sxs-lookup"><span data-stu-id="927bc-128">Available cmdlets</span></span>

<span data-ttu-id="927bc-129">.NET 표준용 Azure PowerShell 모듈은 아직 개발 중입니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-129">The Azure PowerShell modules for .NET Standard are still in development.</span></span> <span data-ttu-id="927bc-130">이러한 모듈은 모듈의 Windows 버전에 대해 사용할 수 있는 cmdlet의 집합을 모두 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-130">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="927bc-131">다음 함수는 AzureRM.Netcore 모듈에서 구현됩니다.</span><span class="sxs-lookup"><span data-stu-id="927bc-131">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="927bc-132">계정 관리</span><span class="sxs-lookup"><span data-stu-id="927bc-132">Account management</span></span>
  - <span data-ttu-id="927bc-133">Microsoft 계정, 조직 계정 또는 Azure Active Directory를 통해 서비스 사용자로 로그인</span><span class="sxs-lookup"><span data-stu-id="927bc-133">Login with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  - <span data-ttu-id="927bc-134">Save-AzureRmContext로 자격 증명을 디스크에 저장하고 Import-AzureRmContext를 사용하여 저장된 자격 증명 로드</span><span class="sxs-lookup"><span data-stu-id="927bc-134">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="927bc-135">Environment</span><span class="sxs-lookup"><span data-stu-id="927bc-135">Environment</span></span>
  - <span data-ttu-id="927bc-136">다른 기본 Microsoft Azure 환경 가져오기</span><span class="sxs-lookup"><span data-stu-id="927bc-136">Get the different out-of-box Microsoft Azure environments</span></span>
  - <span data-ttu-id="927bc-137">사용자 지정 환경 추가/설정/제거(예: Azure Stack 또는 Windows Azure 팩 환경)</span><span class="sxs-lookup"><span data-stu-id="927bc-137">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="927bc-138">리소스 관리자 및 서비스 관리 인터페이스를 사용하여 Azure 서비스용 평면 cmdlet 관리</span><span class="sxs-lookup"><span data-stu-id="927bc-138">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  - <span data-ttu-id="927bc-139">Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="927bc-139">Virtual Machine</span></span>
  - <span data-ttu-id="927bc-140">App Service(웹 사이트)</span><span class="sxs-lookup"><span data-stu-id="927bc-140">App Service (Websites)</span></span>
  - <span data-ttu-id="927bc-141">SQL Database</span><span class="sxs-lookup"><span data-stu-id="927bc-141">SQL Database</span></span>
  - <span data-ttu-id="927bc-142">Storage</span><span class="sxs-lookup"><span data-stu-id="927bc-142">Storage</span></span>
  - <span data-ttu-id="927bc-143">네트워크</span><span class="sxs-lookup"><span data-stu-id="927bc-143">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="927bc-144">다음 단계</span><span class="sxs-lookup"><span data-stu-id="927bc-144">Next Steps</span></span>

<span data-ttu-id="927bc-145">Azure PowerShell 사용에 대한 자세한 내용은 [Azure PowerShell 시작](get-started-azureps.md) 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="927bc-145">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
