---
title: macOS 또는 Linux에 Azure PowerShell 설치
description: macOS 또는 Linux에 Azure PowerShell 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 17912c155255b6fdfd3cfb9242163b67d405dc03
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323172"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="11493-103">macOS 또는 Linux에 Azure PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="11493-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="11493-104">Windows 이외의 플랫폼에서도 PowerShell Core v6 위에 Azure PowerShell을 실행할 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11493-104">For non-Windows platforms, it's possible to run Azure PowerShell on top of PowerShell Core v6.</span></span> <span data-ttu-id="11493-105">Windows용 .NET Framework 기반 표준 Azure PowerShell 대신, 본 제품은 .NET Core용 기반으로서 .Net Core 런타임을 지원하는 모든 플랫폼에서 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="11493-105">Rather than the standard Azure PowerShell built on .NET Framework for Windows, this product is built for .NET Core and can run on any platform which supports the .Net Core runtime.</span></span>

> [!NOTE]
> <span data-ttu-id="11493-106">이때 PowerShell Core v6과 .NET Core용 Azure PowerShell은 아직 베타 버전입니다.</span><span class="sxs-lookup"><span data-stu-id="11493-106">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="11493-107">이러한 제품에 대한 지원은 제한됩니다.</span><span class="sxs-lookup"><span data-stu-id="11493-107">Support for these products is limited.</span></span> <span data-ttu-id="11493-108">문제가 있거나 버그를 발견한 경우 GitHub에서 문제를 제출하십시오.</span><span class="sxs-lookup"><span data-stu-id="11493-108">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="11493-109">PowerShell Core v6에 대한 문제</span><span class="sxs-lookup"><span data-stu-id="11493-109">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="11493-110">Azure PowerShell에 대한 문제</span><span class="sxs-lookup"><span data-stu-id="11493-110">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core-v6"></a><span data-ttu-id="11493-111">PowerShell Core v6 설치</span><span class="sxs-lookup"><span data-stu-id="11493-111">Install PowerShell Core v6</span></span>

<span data-ttu-id="11493-112">Linux 또는 macOS에 PowerShell Core v6을 설치하는 것은 Linux 배포 및 OS 버전에 따라 달라집니다.</span><span class="sxs-lookup"><span data-stu-id="11493-112">Installing PowerShell Core v6 on Linux or macOS varies depending on the Linux distribution and OS version.</span></span>
<span data-ttu-id="11493-113">자세한 지침은 다음 문서에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="11493-113">Detailed instructions can be found in the following articles:</span></span>

- [<span data-ttu-id="11493-114">macOS에 PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="11493-114">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
- [<span data-ttu-id="11493-115">Linux에 PowerShell Core 설치</span><span class="sxs-lookup"><span data-stu-id="11493-115">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a><span data-ttu-id="11493-116">.NET Core용 Azure PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="11493-116">Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="11493-117">PowerShell Core v6은 PowerShellGet 모듈이 이미 설치되어 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="11493-117">PowerShell Core v6 comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="11493-118">따라서 PowerShell 갤러리에 게시된 어떤 모듈도 쉽게 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="11493-118">This makes it easy to install any module that is published to the PowerShell Gallery.</span></span> <span data-ttu-id="11493-119">Azure PowerShell을 설치하려면 새 PowerShell 세션을 열고 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="11493-119">To install Azure PowerShell, open a new PowerShell session and run the following command:</span></span>

```powershell
Install-Module AzureRM.NetCore
```

## <a name="load-the-azurermnetcore-module"></a><span data-ttu-id="11493-120">AzureRM.Netcore 모듈 로드</span><span class="sxs-lookup"><span data-stu-id="11493-120">Load the AzureRM.Netcore module</span></span>

<span data-ttu-id="11493-121">모듈이 설치되면 PowerShell 세션에 모듈을 로드해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="11493-121">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="11493-122">모듈은 다음과 같이 `Import-Module` cmdlet을 사용하여 로드됩니다.</span><span class="sxs-lookup"><span data-stu-id="11493-122">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

<span data-ttu-id="11493-123">가져오기가 완료되면 다음 명령을 사용하여 Azure에 로그인을 시도하여 새로 설치한 모듈을 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="11493-123">After the import completes, you can test your newly installed and module by attempting to sign into Azure using the following command:</span></span>

```powershell
Connect-AzureRmAccount
```

<span data-ttu-id="11493-124">위의 명령을 실행하면 `https://aka.ms/devicelogin`으로 이동하여 제공된 코드를 입력하라는 메시지가 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="11493-124">The above command should prompt you to go to `https://aka.ms/devicelogin` and enter the provided code.</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="11493-125">사용할 수 있는 cmdlet</span><span class="sxs-lookup"><span data-stu-id="11493-125">Available cmdlets</span></span>

<span data-ttu-id="11493-126">.NET 표준용 Azure PowerShell 모듈은 아직 개발 중입니다.</span><span class="sxs-lookup"><span data-stu-id="11493-126">The Azure PowerShell modules for .NET Standard are still in development.</span></span> <span data-ttu-id="11493-127">이러한 모듈은 모듈의 Windows 버전에 대해 사용할 수 있는 cmdlet의 집합을 모두 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="11493-127">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="11493-128">다음 함수는 AzureRM.Netcore 모듈에서 구현됩니다.</span><span class="sxs-lookup"><span data-stu-id="11493-128">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="11493-129">계정 관리</span><span class="sxs-lookup"><span data-stu-id="11493-129">Account management</span></span>
  - <span data-ttu-id="11493-130">Microsoft 계정, 조직 계정 또는 Azure Active Directory를 통해 서비스 사용자로 로그인</span><span class="sxs-lookup"><span data-stu-id="11493-130">Login with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  - <span data-ttu-id="11493-131">Save-AzureRmContext로 자격 증명을 디스크에 저장하고 Import-AzureRmContext를 사용하여 저장된 자격 증명 로드</span><span class="sxs-lookup"><span data-stu-id="11493-131">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="11493-132">Environment</span><span class="sxs-lookup"><span data-stu-id="11493-132">Environment</span></span>
  - <span data-ttu-id="11493-133">다른 기본 Microsoft Azure 환경 가져오기</span><span class="sxs-lookup"><span data-stu-id="11493-133">Get the different out-of-box Microsoft Azure environments</span></span>
  - <span data-ttu-id="11493-134">사용자 지정 환경 추가/설정/제거(예: Azure Stack 또는 Windows Azure 팩 환경)</span><span class="sxs-lookup"><span data-stu-id="11493-134">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="11493-135">리소스 관리자 및 서비스 관리 인터페이스를 사용하여 Azure 서비스용 평면 cmdlet 관리</span><span class="sxs-lookup"><span data-stu-id="11493-135">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  - <span data-ttu-id="11493-136">Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="11493-136">Virtual Machine</span></span>
  - <span data-ttu-id="11493-137">App Service(웹 사이트)</span><span class="sxs-lookup"><span data-stu-id="11493-137">App Service (Websites)</span></span>
  - <span data-ttu-id="11493-138">SQL Database</span><span class="sxs-lookup"><span data-stu-id="11493-138">SQL Database</span></span>
  - <span data-ttu-id="11493-139">Storage</span><span class="sxs-lookup"><span data-stu-id="11493-139">Storage</span></span>
  - <span data-ttu-id="11493-140">네트워크</span><span class="sxs-lookup"><span data-stu-id="11493-140">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="11493-141">다음 단계</span><span class="sxs-lookup"><span data-stu-id="11493-141">Next Steps</span></span>

<span data-ttu-id="11493-142">Azure PowerShell 사용에 대한 자세한 내용은 [Azure PowerShell 시작](get-started-azureps.md) 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="11493-142">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
