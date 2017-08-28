---
title: "Azure PowerShell을 설치하는 다른 방법 | Microsoft Docs"
description: "MSI 패키지 또는 웹 플랫폼 설치 관리자를 사용하여 Azure PowerShell을 설치하는 방법입니다."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: 9cee582f74b7f3260c6ae167a8ac358d360ad8ab
ms.sourcegitcommit: 45587b5091293288e16cfae8ac412e0d42f8f450
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/15/2017
---
# <a name="other-installation-methods"></a><span data-ttu-id="9cdb1-103">다른 설치 방법</span><span class="sxs-lookup"><span data-stu-id="9cdb1-103">Other installation methods</span></span>

<span data-ttu-id="9cdb1-104">Azure PowerShell에는 여러 설치 방법이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-104">Azure PowerShell has multiple installation methods.</span></span> <span data-ttu-id="9cdb1-105">PowerShell 갤러리와 PowerShellGet을 사용하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-105">Using PowerShellGet with the PowerShell Gallery is the preferred method.</span></span> <span data-ttu-id="9cdb1-106">Azure PowerShell은 웹 플랫폼 설치 관리자(WebPI)를 사용하거나 [GitHub](https://github.com/Azure/azure-powershell/releases/latest)에서 사용할 수 있는 MSI 파일을 사용하여 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-106">Azure PowerShell can be installed using the Web Platform Installer (WebPI) or by using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span>

## <a name="docker"></a><span data-ttu-id="9cdb1-107">Docker</span><span class="sxs-lookup"><span data-stu-id="9cdb1-107">Docker</span></span>

<span data-ttu-id="9cdb1-108">Microsoft는 Azure PowerShell로 미리 구성된 Docker 이미지를 유지합니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-108">We maintain a Docker image preconfigured with Azure PowerShell.</span></span>

<span data-ttu-id="9cdb1-109">`docker run`으로 컨테이너를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-109">Run the container with `docker run`.</span></span>

```powershell
docker run azuresdk/azure-powershell
```

<span data-ttu-id="9cdb1-110">또한 Microsoft는 PowerShell Core 컨테이너로 cmdlet의 하위 집합을 유지합니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-110">In addition, we maintain a subset of cmdlets as a PowerShell Core container.</span></span>

<span data-ttu-id="9cdb1-111">Mac/Linux의 경우 `latest` 이미지를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-111">For Mac/Linux, use the `latest` image.</span></span>

```bash
docker run azuresdk/azure-powershell-core:latest
```

<span data-ttu-id="9cdb1-112">Windows의 경우 `nanoserver` 이미지를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-112">For Windows, use the `nanoserver` image.</span></span>

```powershell
docker run azuresdk/azure-powershell-core:nanoserver
```

<span data-ttu-id="9cdb1-113">Azure PowerShell은 [PowerShell 갤러리](https://www.powershellgallery.com/)에서 `Install-Module`을 통해 이미지에 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-113">Azure PowerShell is installed on the image via `Install-Module` from the [PowerShell Gallery](https://www.powershellgallery.com/).</span></span>

## <a name="install-using-the-web-platform-installer"></a><span data-ttu-id="9cdb1-114">웹 플랫폼 설치 관리자를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="9cdb1-114">Install using the Web Platform Installer</span></span>

<span data-ttu-id="9cdb1-115">WebPI에서 최신 Azure PowerShell을 설치하는 것은 이전 버전과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-115">Installing the latest Azure PowerShell from WebPI is the same as it was for previous versions.</span></span>
<span data-ttu-id="9cdb1-116">[Azure PowerShell WebPI 패키지](http://aka.ms/webpi-azps)를 다운로드하고 설치를 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-116">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span>

> [!NOTE]
> <span data-ttu-id="9cdb1-117">이전에 PowerShell 갤러리에서 Azure 모듈을 설치한 경우에는 설치 관리자가 해당 모듈을 자동으로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-117">If you have previously installed Azure modules from the PowerShell Gallery, the installer automatically removes them.</span></span> <span data-ttu-id="9cdb1-118">한 가지 버전의 Azure PowerShell을 설치하여 사용자 환경을 단순화합니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-118">This simplifies your environment by ensuring that only one version of Azure PowerShell is installed.</span></span> <span data-ttu-id="9cdb1-119">그러나 여러 버전이 동시에 설치된 시나리오가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-119">However, there are scenarios where you may need multiple versions installed at the same time.</span></span>
>
> <span data-ttu-id="9cdb1-120">PowerShell 갤러리 모듈은 `$env:ProgramFiles\WindowsPowerShell\Modules`에서 모듈을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-120">PowerShell Gallery modules install modules in `$env:ProgramFiles\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="9cdb1-121">반면, WebPI 설치 관리자는 `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`에서 Azure 모듈을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-121">In contrast, the WebPI installer installs the Azure modules in `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span></span>
>
> <span data-ttu-id="9cdb1-122">설치 중에 오류가 발생하는 경우 `$env:ProgramFiles\WindowsPowerShell\Modules` 폴더에서 Azure* 폴더를 수동으로 제거한 다음 다시 설치하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-122">If an error occurs during install, you can manually remove the Azure* folders in your `$env:ProgramFiles\WindowsPowerShell\Modules` folder, and try the installation again.</span></span>

<span data-ttu-id="9cdb1-123">설치가 완료되면 `$env:PSModulePath` 설정에는 Azure PowerShell cmdlet이 들어 있는 디렉터리가 포함되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-123">Once the installation completes, your `$env:PSModulePath` setting should include the directories containing the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="9cdb1-124">다음 명령을 사용하여 Azure PowerShell이 제대로 설치되어 있는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-124">The following command can be used to verify that the Azure PowerShell is installed properly.</span></span>

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> <span data-ttu-id="9cdb1-125">WebPI에서 설치할 때 발생할 수 있는 알려진 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-125">There is a known issue that can occur when installing from WebPI.</span></span> <span data-ttu-id="9cdb1-126">시스템 업데이트 또는 다른 설치로 인해 컴퓨터를 다시 시작해야 하는 경우 `$env:PSModulePath` 업데이트 과정에서 Azure PowerShell이 설치된 경로가 포함되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-126">If your computer requires a restart due to system updates or other installations, it may cause updates to `$env:PSModulePath` to fail to include the path where Azure PowerShell is installed.</span></span>

<span data-ttu-id="9cdb1-127">설치 후에 cmdlet을 로드하거나 실행하려고 할 때 다음과 같은 오류 메시지가 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-127">When attempting to load or execute cmdlets after installation, you can receive the following error message:</span></span>

```
PS C:\> Login-AzureRmAccount
Login-AzureRmAccount : The term 'Login-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Login-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Login-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

<span data-ttu-id="9cdb1-128">컴퓨터를 다시 시작하거나 정규화된 경로를 사용하는 모듈을 가져와서 이 오류를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-128">This error can be corrected by restarting the machine or importing the module using the fully qualified path.</span></span> <span data-ttu-id="9cdb1-129">예:</span><span class="sxs-lookup"><span data-stu-id="9cdb1-129">For example:</span></span>

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-using-the-msi-package"></a><span data-ttu-id="9cdb1-130">MSI 패키지를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="9cdb1-130">Install using the MSI Package</span></span>

<span data-ttu-id="9cdb1-131">Azure PowerShell은 [GitHub](https://github.com/Azure/azure-powershell/releases/latest)에서 사용할 수 있는 MSI 파일을 사용하여 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-131">Azure PowerShell can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span> <span data-ttu-id="9cdb1-132">이전 버전의 Azure 모듈이 설치된 경우 설치 관리자에서 자동으로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-132">If you have installed previous versions of Azure modules, the installer automatically removes them.</span></span> <span data-ttu-id="9cdb1-133">MSI 패키지는 `$env:ProgramFiles\WindowsPowerShell\Modules`에서 모듈을 설치하지만 특정 버전 폴더를 만들지는 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9cdb1-133">The MSI package installs modules in `$env:ProgramFiles\WindowsPowerShell\Modules` but does not create version-specific folders.</span></span>
