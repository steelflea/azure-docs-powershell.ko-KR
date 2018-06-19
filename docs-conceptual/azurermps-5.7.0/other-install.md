---
title: Azure PowerShell을 설치하는 다른 방법
description: MSI 패키지 또는 웹 플랫폼 설치 관리자를 사용하여 Azure PowerShell을 설치하는 방법입니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 0919583d9cb05a75fae3b812eed84109be8b28aa
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323274"
---
# <a name="other-installation-methods"></a><span data-ttu-id="0472f-103">다른 설치 방법</span><span class="sxs-lookup"><span data-stu-id="0472f-103">Other installation methods</span></span>

<span data-ttu-id="0472f-104">이 문서에서는 MSI 또는 웹 플랫폼 설치 관리자 (WebPI)를 사용하여 Azure PowerShell을 설치 하는 방법에 대해 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-104">This article explains how to install Azure PowerShell using an MSI or Web Platform Installer (WebPI).</span></span> <span data-ttu-id="0472f-105">또한 Docker 컨테이너 내부에서 Azure PowerShell을 실행할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-105">You can also run Azure PowerShell from inside of a Docker container.</span></span> <span data-ttu-id="0472f-106">시스템에 필요한 경우에만 이러한 설치 방법을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-106">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="0472f-107">Azure PowerShell을 설치하는 정식 방법은 PowerShellGet을 사용하는 방식입니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-107">The canonical way to install Azure PowerShell is through PowerShellGet.</span></span> <span data-ttu-id="0472f-108">PowerShellGet을 사용하여 Azure PowerShell을 설치하는 방법은 [PowerShellGet으로 Azure PowerShell 설치하기](install-azurerm-ps.md)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-108">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

<span data-ttu-id="0472f-109">Linux 또는 macOS 환경에 설치하려면 [macOS 또는 Linux에 Azure PowerShell 설치](install-azurermps-maclinux.md)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-109">To install on Linux or macOS environments, see [Install Azure PowerShell on macOS or Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a><span data-ttu-id="0472f-110">웹 플랫폼 설치 관리자를 사용하여 Windows에 설치 및 업데이트</span><span class="sxs-lookup"><span data-stu-id="0472f-110">Install or update on Windows using the Web Platform Installer</span></span>

<span data-ttu-id="0472f-111">WebPI에서 최신 Azure PowerShell을 설치하는 것은 이전 버전과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-111">Installing the latest Azure PowerShell from WebPI is the same as it was for previous versions.</span></span>
<span data-ttu-id="0472f-112">[Azure PowerShell WebPI 패키지](http://aka.ms/webpi-azps)를 다운로드하고 설치를 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-112">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span>

> [!NOTE]
> <span data-ttu-id="0472f-113">이전에 PowerShell 갤러리에서 Azure 모듈을 설치한 경우에는 설치 관리자가 해당 모듈을 자동으로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-113">If you have previously installed Azure modules from the PowerShell Gallery, the installer automatically removes them.</span></span> <span data-ttu-id="0472f-114">한 가지 버전의 Azure PowerShell을 설치하여 사용자 환경을 단순화합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-114">This simplifies your environment by ensuring that only one version of Azure PowerShell is installed.</span></span> <span data-ttu-id="0472f-115">그러나 여러 버전이 동시에 설치된 시나리오가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-115">However, there are scenarios where you may need multiple versions installed at the same time.</span></span>
>
> <span data-ttu-id="0472f-116">PowerShell 갤러리 모듈은 `$env:ProgramFiles\WindowsPowerShell\Modules`에서 모듈을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-116">PowerShell Gallery modules install modules in `$env:ProgramFiles\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="0472f-117">반면, WebPI 설치 관리자는 `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`에서 Azure 모듈을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-117">In contrast, the WebPI installer installs the Azure modules in `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span></span>
>
> <span data-ttu-id="0472f-118">설치 중에 오류가 발생하는 경우 `$env:ProgramFiles\WindowsPowerShell\Modules` 폴더에서 `Azure*`폴더를 수동으로 제거한 다음 다시 설치하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-118">If an error occurs during install, you can manually remove the `Azure*` folders in your `$env:ProgramFiles\WindowsPowerShell\Modules` folder, and try the installation again.</span></span>

<span data-ttu-id="0472f-119">설치가 완료되면 `$env:PSModulePath` 설정에는 Azure PowerShell cmdlet이 들어 있는 디렉터리가 포함되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-119">Once the installation completes, your `$env:PSModulePath` setting should include the directories containing the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="0472f-120">다음 명령을 사용하여 Azure PowerShell이 제대로 설치되어 있는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-120">The following command can be used to verify that the Azure PowerShell is installed properly:</span></span>

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> <span data-ttu-id="0472f-121">WebPI에서 설치할 때 발생할 수 있는 알려진 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-121">There is a known issue that can occur when installing from WebPI.</span></span> <span data-ttu-id="0472f-122">시스템 업데이트 또는 다른 설치로 인해 컴퓨터를 다시 시작해야 하는 경우 `$env:PSModulePath` 업데이트 과정에서 Azure PowerShell이 설치된 경로가 포함되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-122">If your computer requires a restart due to system updates or other installations, it may cause updates to `$env:PSModulePath` to fail to include the path where Azure PowerShell is installed.</span></span>

<span data-ttu-id="0472f-123">설치 후에 cmdlet을 로드하거나 실행하려고 할 때 다음과 같은 오류 메시지가 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-123">When attempting to load or execute cmdlets after installation, you can receive the following error message:</span></span>

```
PS C:\> Connect-AzureRmAccount
Connect-AzureRmAccount : The term 'Connect-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Connect-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Connect-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

<span data-ttu-id="0472f-124">컴퓨터를 다시 시작하거나 정규화된 경로를 사용하는 모듈을 가져와서 이 오류를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-124">This error can be corrected by restarting the machine or importing the module using the fully qualified path.</span></span>

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="0472f-125">MSI 패키지를 사용하여 Windows에 설치 및 업데이트</span><span class="sxs-lookup"><span data-stu-id="0472f-125">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="0472f-126">Azure PowerShell은 [GitHub](https://aka.ms/azps-release)에서 사용할 수 있는 MSI 파일을 사용하여 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-126">Azure PowerShell can be installed using the MSI file available from [GitHub](https://aka.ms/azps-release).</span></span> <span data-ttu-id="0472f-127">이전 버전의 Azure 모듈이 설치된 경우 설치 관리자에서 자동으로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-127">If you have installed previous versions of Azure modules, the installer automatically removes them.</span></span> <span data-ttu-id="0472f-128">MSI 패키지는 `$env:ProgramFiles\WindowsPowerShell\Modules`에서 모듈을 설치하지만 특정 버전 폴더를 만들지는 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-128">The MSI package installs modules in `$env:ProgramFiles\WindowsPowerShell\Modules` but does not create version-specific folders.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="0472f-129">Docker 컨테이너에서 실행</span><span class="sxs-lookup"><span data-stu-id="0472f-129">Run in a Docker container</span></span>

<span data-ttu-id="0472f-130">Microsoft는 Azure PowerShell로 미리 구성된 Docker 이미지 집합을 유지합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-130">We maintain a set of Docker images preconfigured with Azure PowerShell.</span></span> <span data-ttu-id="0472f-131">사용할 수 있는 두 가지 유형의 컨테이너: Windows에서 기존의 PowerShell을 실행 중인 컨테이너 및 Windows 또는 Linux에서 PowerShell Core를 실행 중인 컨테이너</span><span class="sxs-lookup"><span data-stu-id="0472f-131">There are two types of containers available: Those running traditional PowerShell on Windows, and a container running PowerShell Core on either Windows or Linux.</span></span>

| <span data-ttu-id="0472f-132">Environment</span><span class="sxs-lookup"><span data-stu-id="0472f-132">Environment</span></span> | <span data-ttu-id="0472f-133">Docker 이미지</span><span class="sxs-lookup"><span data-stu-id="0472f-133">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="0472f-134">PowerShell(Windows)</span><span class="sxs-lookup"><span data-stu-id="0472f-134">PowerShell on Windows</span></span> | [<span data-ttu-id="0472f-135">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="0472f-135">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="0472f-136">PowerShell Core(Windows)</span><span class="sxs-lookup"><span data-stu-id="0472f-136">PowerShell Core on Windows</span></span> | [<span data-ttu-id="0472f-137">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="0472f-137">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="0472f-138">PowerShell Core(Linux)</span><span class="sxs-lookup"><span data-stu-id="0472f-138">PowerShell Core on Linux</span></span> | [<span data-ttu-id="0472f-139">azuresdk/azure-powershell-core:latest</span><span class="sxs-lookup"><span data-stu-id="0472f-139">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="0472f-140">이러한 컨테이너 중 하나를 실행하려면 `docker run -it $ImageName`을(를) 사용하여 대화형 터미널을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-140">To run any of these containers, you use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="0472f-141">예를 들어 Linux 컨테이너에서 PowerShell Core를 실행하려면 다음을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-141">For example, to run the PowerShell Core on Linux container, use:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="0472f-142">Docker에서 Windows 컨테이너를 실행하려면 호스트 OS가 Windows여야 하며 Docker를 Windows 컨테이너를 실행하도록 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-142">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="0472f-143">Docker에서 Windows와 Linux 환경 사이에서 전환하는 방법에 대한 자세한 내용은, Docker 설명서 [Windows 및 Linux 컨테이너 간 전환](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers)을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="0472f-143">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>