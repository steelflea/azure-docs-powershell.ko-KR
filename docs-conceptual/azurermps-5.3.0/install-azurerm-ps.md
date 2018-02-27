---
title: "Azure PowerShell 설치 및 구성 | Microsoft Docs"
description: "Azure PowerShell을 처음으로 설치하고 구성하는 방법입니다."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 08/31/2017
ms.openlocfilehash: 1a1a2e3d69252c8461284e6ec8e26fa838e773f7
ms.sourcegitcommit: 7e77fe7ecd2112d6b4515517509c5c723e750e27
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/19/2018
---
# <a name="install-and-configure-azure-powershell"></a><span data-ttu-id="340ff-103">Azure PowerShell 설치 및 구성</span><span class="sxs-lookup"><span data-stu-id="340ff-103">Install and configure Azure PowerShell</span></span>

<span data-ttu-id="340ff-104">이 문서에서는 Windows 환경에서 Azure PowerShell 모듈을 설치하는 단계를 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-104">This article explains the steps to install the Azure PowerShell modules in a Windows environment.</span></span>  
<span data-ttu-id="340ff-105">macOS 또는 Linux에서 Azure PowerShell을 사용하려는 경우 다음 아티클을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="340ff-105">If you want to use Azure PowerShell on macOS or Linux, see the following article:</span></span>  
<span data-ttu-id="340ff-106">[macOS 및 Linux에서 Azure PowerShell 설치 및 구성](install-azurermps-maclinux.md)</span><span class="sxs-lookup"><span data-stu-id="340ff-106">[Install and configure Azure PowerShell on macOS and Linux](install-azurermps-maclinux.md).</span></span>

<span data-ttu-id="340ff-107">PowerShell 갤러리에서 Azure PowerShell을 설치하는 것이 기본적인 설치 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-107">Installing Azure PowerShell from the PowerShell Gallery is the preferred method of installation.</span></span>

## <a name="step-1-install-powershellget"></a><span data-ttu-id="340ff-108">1단계: PowerShellGet 설치</span><span class="sxs-lookup"><span data-stu-id="340ff-108">Step 1: Install PowerShellGet</span></span>

<span data-ttu-id="340ff-109">PowerShell 갤러리에서 항목을 설치하려면 PowerShellGet 모듈이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-109">Installing items from the PowerShell Gallery requires the PowerShellGet module.</span></span> <span data-ttu-id="340ff-110">적절한 버전의 PowerShellGet 및 다른 시스템 요구 사항이 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-110">Make sure you have the appropriate version of PowerShellGet and other system requirements.</span></span> <span data-ttu-id="340ff-111">PowerShellGet이 시스템에 설치되어 있는지 확인하려면 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-111">Run the following command to see if you have PowerShellGet installed on your system.</span></span>

```powershell
Get-Module -Name PowerShellGet -ListAvailable | Select-Object -Property Name,Version,Path
```

<span data-ttu-id="340ff-112">다음과 비슷하게 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-112">You should see something similar to the following output:</span></span>

```Output
Name          Version Path
----          ------- ----
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```
<span data-ttu-id="340ff-113">또한 다음 아래 명령을 사용하여 PowerShellGet을 업데이트하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-113">In addition you may want to update PowerShellGet with the command below:</span></span>
```powershell
Install-Module PowerShellGet -Force
```

<span data-ttu-id="340ff-114">PowerShellGet을 설치하지 않은 경우 이 문서의 [PowerShellGet을 가져오는 방법](#how-to-get-powershellget) 섹션을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="340ff-114">If you do not have PowerShellGet installed, see the [How to get PowerShellGet](#how-to-get-powershellget) section of this article.</span></span>

> [!NOTE]
> <span data-ttu-id="340ff-115">PowerShellGet을 사용하려면 스크립트를 실행할 수 있게 하는 실행 정책이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-115">Using PowerShellGet requires an Execution Policy that allows you to run scripts.</span></span> <span data-ttu-id="340ff-116">PowerShell의 실행 정책에 대한 자세한 내용은 [실행 정책 정보](/powershell/module/microsoft.powershell.core/about/about_execution_policies)(영문)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="340ff-116">For more information about PowerShell's Execution Policy, see [About Execution Policies](/powershell/module/microsoft.powershell.core/about/about_execution_policies).</span></span>

## <a name="step-2-install-azure-powershell"></a><span data-ttu-id="340ff-117">2단계: Azure PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="340ff-117">Step 2: Install Azure PowerShell</span></span>

<span data-ttu-id="340ff-118">PowerShell 갤러리에서 Azure PowerShell을 설치하려면 상승된 권한이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-118">Installing Azure PowerShell from the PowerShell Gallery requires elevated privileges.</span></span> <span data-ttu-id="340ff-119">상승된 PowerShell 세션에서 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-119">Run the following command from an elevated PowerShell session:</span></span>

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

<span data-ttu-id="340ff-120">기본적으로 PowerShell 갤러리는 PowerShellGet에 대한 신뢰할 수 있는 리포지토리로 구성되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-120">By default, the PowerShell gallery is not configured as a Trusted repository for PowerShellGet.</span></span> <span data-ttu-id="340ff-121">PSGallery를 처음 사용할 때는 다음과 같은 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-121">The first time you use the PSGallery you see the following prompt:</span></span>

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"): Y
```

<span data-ttu-id="340ff-122">설치를 계속하려면 'Yes' 또는 'Yes to All'로 답변합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-122">Answer 'Yes' or 'Yes to All' to continue with the installation.</span></span>

> [!NOTE]
> <span data-ttu-id="340ff-123">NuGet 2.8.5.201 이전 버전을 사용하는 경우 최신 버전의 NuGet을 다운로드하여 설치하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-123">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="340ff-124">AzureRM 모듈은 Azure Resource Manager cmdlet의 롤업 모듈입니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-124">The AzureRM module is a rollup module for the Azure Resource Manager cmdlets.</span></span> <span data-ttu-id="340ff-125">AzureRM 모듈을 설치하는 경우 이전에 설치되지 않은 Azure PowerShell 모듈이 PowerShell 갤러리에서 다운로드되고 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-125">When you install the AzureRM module, any Azure PowerShell module not previously installed is downloaded and from the PowerShell Gallery.</span></span>

<span data-ttu-id="340ff-126">이전 버전의 Azure PowerShell이 설치된 경우 오류가 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-126">If you have a previous version of Azure PowerShell installed you may receive an error.</span></span> <span data-ttu-id="340ff-127">이 문제를 해결하려면 이 문서의 [새 Azure PowerShell 버전으로 업데이트](#update-azps) 섹션을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="340ff-127">To resolve this issue, see the [Updating to a new version of Azure PowerShell](#update-azps) section of this article.</span></span>

## <a name="step-3-load-the-azurerm-module"></a><span data-ttu-id="340ff-128">3단계: AzureRM 모듈 로드</span><span class="sxs-lookup"><span data-stu-id="340ff-128">Step 3: Load the AzureRM module</span></span>
<span data-ttu-id="340ff-129">모듈이 설치되면 PowerShell 세션에 모듈을 로드해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-129">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="340ff-130">이 작업은 일반(권한이 상승되지 않은) PowerShell 세션에서 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-130">You should do this in a normal (non-elevated) PowerShell session.</span></span> <span data-ttu-id="340ff-131">모듈은 다음과 같이 `Import-Module` cmdlet을 사용하여 로드됩니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-131">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module -Name AzureRM
```

## <a name="next-steps"></a><span data-ttu-id="340ff-132">다음 단계</span><span class="sxs-lookup"><span data-stu-id="340ff-132">Next Steps</span></span>

<span data-ttu-id="340ff-133">Azure PowerShell을 사용하는 방법에 대한 자세한 내용은 다음 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="340ff-133">For more information about using Azure PowerShell, see the following articles:</span></span>

* [<span data-ttu-id="340ff-134">Azure PowerShell 시작</span><span class="sxs-lookup"><span data-stu-id="340ff-134">Get started with Azure PowerShell</span></span>](get-started-azureps.md)

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="340ff-135">문제 보고 및 피드백</span><span class="sxs-lookup"><span data-stu-id="340ff-135">Reporting issues and feedback</span></span>

<span data-ttu-id="340ff-136">도구에서 버그가 발견되면 GitHub 리포지토리의 [문제](https://github.com/Azure/azure-powershell/issues) 섹션에 문제를 기록해 주세요.</span><span class="sxs-lookup"><span data-stu-id="340ff-136">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-powershell/issues) section of our GitHub repo.</span></span> <span data-ttu-id="340ff-137">명령줄에서 피드백을 제공하려면 `Send-Feedback` cmdlet을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="340ff-137">To provide feedback from the command line, use the `Send-Feedback` cmdlet.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="340ff-138">질문과 대답</span><span class="sxs-lookup"><span data-stu-id="340ff-138">Frequently asked questions</span></span>

### <a name="how-to-get-powershellget"></a><span data-ttu-id="340ff-139">PowerShellGet을 가져오는 방법</span><span class="sxs-lookup"><span data-stu-id="340ff-139">How to get PowerShellGet</span></span>

|<span data-ttu-id="340ff-140">시나리오</span><span class="sxs-lookup"><span data-stu-id="340ff-140">Scenario</span></span>|<span data-ttu-id="340ff-141">설치 지침</span><span class="sxs-lookup"><span data-stu-id="340ff-141">Install instructions</span></span>|
|---|---|
|<span data-ttu-id="340ff-142">윈도우 10</span><span class="sxs-lookup"><span data-stu-id="340ff-142">Windows 10</span></span><br/><span data-ttu-id="340ff-143">Windows Server 2016</span><span class="sxs-lookup"><span data-stu-id="340ff-143">Windows Server 2016</span></span>|<span data-ttu-id="340ff-144">OS에 포함된 WMF(Windows Management Framework) 5.0으로 빌드됩니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-144">Built into Windows Management Framework (WMF) 5.0 included in the OS</span></span>|
|<span data-ttu-id="340ff-145">PowerShell 5로 업그레이드하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-145">I want to upgrade to PowerShell 5</span></span>|<ol><li>[<span data-ttu-id="340ff-146">최신 버전의 WMF 설치</span><span class="sxs-lookup"><span data-stu-id="340ff-146">Install the latest version of WMF</span></span>](https://www.microsoft.com/en-us/download/details.aspx?id=54616)</li><li><span data-ttu-id="340ff-147">다음 명령 실행:</span><span class="sxs-lookup"><span data-stu-id="340ff-147">Run the following command:</span></span><br/>```Install-Module PowerShellGet -Force```</li></ol>|
|<span data-ttu-id="340ff-148">PowerShell 3 또는 PowerShell 4를 사용하는 Windows 버전에서 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-148">I am running on a version of Windows with PowerShell 3 or PowerShell 4</span></span>|<ol><span data-ttu-id="340ff-149"><il>[PackageManagement 모듈 가져오기](http://go.microsoft.com/fwlink/?LinkID=746217)</il></span><span class="sxs-lookup"><span data-stu-id="340ff-149"><il>[Get the PackageManagement modules](http://go.microsoft.com/fwlink/?LinkID=746217)</il></span></span><li><span data-ttu-id="340ff-150">다음 명령 실행:</span><span class="sxs-lookup"><span data-stu-id="340ff-150">Run the following command:</span></span><br/>```Install-Module PowerShellGet -Force```</li></ol>|

<a id="helpmechoose"></a>
### <a name="checking-the-version-of-azure-powershell"></a><span data-ttu-id="340ff-151">Azure PowerShell 버전 확인</span><span class="sxs-lookup"><span data-stu-id="340ff-151">Checking the version of Azure PowerShell</span></span>

<span data-ttu-id="340ff-152">가능한 한 빨리 최신 버전으로 업그레이드하는 것이 좋지만 여러 버전의 Azure PowerShell이 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-152">Although we encourage you to upgrade to the latest version as early as possible, several versions of Azure PowerShell are supported.</span></span> <span data-ttu-id="340ff-153">설치한 Azure PowerShell의 버전을 확인하려면 명령줄에서 `Get-Module AzureRM`을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-153">To determine the version of Azure PowerShell you have installed, run `Get-Module AzureRM` from your command line.</span></span>

```powershell
Get-Module AzureRM -ListAvailable | Select-Object -Property Name,Version,Path
```

### <a name="support-for-classic-deployment-methods"></a><span data-ttu-id="340ff-154">클래식 배포 방법에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="340ff-154">Support for classic deployment methods</span></span>

<span data-ttu-id="340ff-155">클래식 배포 모델을 사용하는 배포가 있는 경우 Azure PowerShell의 Service Management 버전을 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-155">If you have deployments that use the classic deployment model you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="340ff-156">자세한 내용은 [Azure PowerShell Service Management 모듈 설치](/powershell/azure/servicemanagement/install-azure-ps)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="340ff-156">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span> <span data-ttu-id="340ff-157">Azure 모듈과 AzureRM 모듈은 공통 종속성을 공유합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-157">The Azure and AzureRM modules share common dependencies.</span></span> <span data-ttu-id="340ff-158">Azure와 AzureRM 모듈을 둘 다 사용하는 경우 각 패키지의 동일한 버전을 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-158">If you use both the Azure and AzureRM modules, you should install the same version of each package.</span></span>

### <a id="update-azps"></a><span data-ttu-id="340ff-159">새 Azure PowerShell 버전으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="340ff-159">Updating to a new version of Azure PowerShell</span></span>

<span data-ttu-id="340ff-160">서비스 관리 모듈을 포함하는 이전 버전의 Azure PowerShell이 설치되어 있는 경우 다음과 같은 오류가 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-160">If you have a previous version of Azure PowerShell installed that includes the Service Management module, you may receive the following error:</span></span>

```Output
PackageManagement\Install-Package : A command with name 'Get-AzureStorageContainerAcl' is already
available on this system. This module 'Azure.Storage' may override the existing commands. If you
still want to install this module 'Azure.Storage', use -AllowClobber parameter.

At C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PSModule.psm1:1772 char:21
+ ...          $null = PackageManagement\Install-Package @PSBoundParameters
+                      ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidOperation: (Microsoft.Power....InstallPackage:InstallPackage) [Install-Package], Exception
    + FullyQualifiedErrorId : CommandAlreadyAvailable,Validate-ModuleCommandAlreadyAvailable,Microsoft.PowerShell.PackageManagement.Cmdlets.InstallPackage
```

<span data-ttu-id="340ff-161">이 오류 메시지에 나오는 것처럼 -AllowClobber 매개 변수를 사용해서 모듈을 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-161">As the error message states, you need to use the -AllowClobber parameter to install the module.</span></span> <span data-ttu-id="340ff-162">다음 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-162">Use the following command:</span></span>

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

<span data-ttu-id="340ff-163">자세한 내용은 [Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module)에 대한 도움말 항목을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="340ff-163">For more information, see the help topic for [Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module).</span></span>

### <a name="installing-module-versions-side-by-side"></a><span data-ttu-id="340ff-164">단계별 모듈 버전 설치</span><span class="sxs-lookup"><span data-stu-id="340ff-164">Installing module versions side by side</span></span>

<span data-ttu-id="340ff-165">PowerShellGet 설치 방법은 여러 버전의 설치를 지원하는 유일한 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-165">The PowerShellGet method of installation is the only method that supports the installation of multiple versions.</span></span> <span data-ttu-id="340ff-166">예를 들어 업데이트할 시간이나 리소스가 없는 이전 버전의 Azure PowerShell을 사용하여 작성한 스크립트가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-166">For example, you may have scripts written using a previous version of Azure PowerShell that you don't have the time or resources to updated.</span></span> <span data-ttu-id="340ff-167">다음 명령에서는 여러 버전의 Azure PowerShell을 설치하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-167">The following commands illustrate how to install multiple versions of Azure PowerShell:</span></span>

```powershell
Install-Module -Name AzureRM -RequiredVersion 3.7.0
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

<span data-ttu-id="340ff-168">PowerShell 세션에서 한 버전의 모듈만 로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-168">Only one version of the module can be loaded in a PowerShell session.</span></span> <span data-ttu-id="340ff-169">새 PowerShell 창을 열고 `Import-Module`을 사용하여 특정 버전의 AzureRM cmdlet을 가져와야 합니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-169">You must open a new PowerShell window and use `Import-Module` to import a specific version of the AzureRM cmdlets:</span></span>

```powershell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

> [!NOTE]
> <span data-ttu-id="340ff-170">2.1.0 버전 및 1.2.6 버전은 나란히 설치하여 사용하도록 설계된 첫 번째 모듈 버전입니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-170">Version 2.1.0 and version 1.2.6 are the first module versions designed to be installed and used side by side.</span></span> <span data-ttu-id="340ff-171">이전 버전의 Azure PowerShell을 로드하는 경우는 호환되지 않는 **AzureRM.Profile** 모듈 버전이 로드됩니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-171">When loading an earlier version of the Azure PowerShell, incompatible versions of the **AzureRM.Profile** module are loaded.</span></span> <span data-ttu-id="340ff-172">그 결과 cmdlet을 실행할 때마다 로그인하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="340ff-172">This results in the cmdlets prompting you to log in whenever you execute a cmdlet.</span></span>

### <a name="other-installation-methods"></a><span data-ttu-id="340ff-173">다른 설치 방법</span><span class="sxs-lookup"><span data-stu-id="340ff-173">Other installation methods</span></span>

<span data-ttu-id="340ff-174">웹 플랫폼 설치 관리자 또는 MSI 패키지를 사용하여 설치하는 방법에 대한 자세한 내용은 [다른 설치 방법](other-install.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="340ff-174">For information about installing using the Web Platform Installer or the MSI Package, see [Other installation methods](other-install.md)</span></span>
