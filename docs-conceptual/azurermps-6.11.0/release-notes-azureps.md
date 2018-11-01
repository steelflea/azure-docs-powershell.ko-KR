---
title: Azure PowerShell 변경 로그 | Microsoft Docs
description: Azure PowerShell에 대한 최신 릴리스의 변경 내용입니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 08/28/2018
ms.openlocfilehash: eec8b5960f787fa9ca1130b4f8b49c9d896aa99e
ms.sourcegitcommit: ff44dec6418a449757bded3c6ebe0a7d4c05ee6e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/01/2018
ms.locfileid: "50738107"
---
# <a name="release-notes"></a><span data-ttu-id="19d40-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="19d40-103">Release notes</span></span>

<span data-ttu-id="19d40-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6110---october-2018"></a><span data-ttu-id="19d40-105">6.11.0 - 2018년 10월</span><span class="sxs-lookup"><span data-stu-id="19d40-105">6.11.0 - October 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="19d40-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="19d40-106">AzureRM.Profile</span></span>
* <span data-ttu-id="19d40-107">CloudShell에서 Get-AzureRmSubscription을 사용하여 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-107">Fix issue with Get-AzureRmSubscription in CloudShell</span></span>
* <span data-ttu-id="19d40-108">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-108">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="19d40-109">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="19d40-109">AzureRM.Backup</span></span>
* <span data-ttu-id="19d40-110">Azure Backup cmdlet이 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-110">Deprecated Azure Backup cmdlets.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="19d40-111">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="19d40-111">AzureRM.Compute</span></span>
* <span data-ttu-id="19d40-112">'New-AzureRmVm'에 대해 간단한 매개 변수를 사용하는 경우 가속화된 네트워킹을 설정하기 위해 새 크기가 VM 크기의 허용 목록에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-112">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzureRmVm'</span></span>
* <span data-ttu-id="19d40-113">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-113">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="19d40-114">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="19d40-114">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="19d40-115">Virtual Network 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-115">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="19d40-116">Get-AzureRmDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 가져오거나 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-116">Get-AzureRmDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="19d40-117">Add-AzureRmDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 가상 네트워크 규칙을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-117">Add-AzureRmDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="19d40-118">Set-AzureRmDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에서 지정된 가상 네트워크 규칙을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-118">Set-AzureRmDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="19d40-119">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-119">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="19d40-120">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="19d40-120">AzureRM.Network</span></span>
* <span data-ttu-id="19d40-121">Test-AzureRmNetworkWatcherConnectivity cmdlet을 업데이트하고, 백 엔드에 프로토콜 값을 전달합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-121">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="19d40-122">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-122">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="19d40-123">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="19d40-123">AzureRM.Resources</span></span>
* <span data-ttu-id="19d40-124">(기본 프로필에 구독이 없고 범위가 지정되지 않은 경우) 시나리오에서 의미 있는 예외를 추가하여 Get-AzureRMRoleDefinition이 인식할 수 없는 예외를 throw하는 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-124">Fix isssue where Get-AzureRMRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="19d40-125">또한 기본 매개 변수 집합을 'RoleDefinitionNameParameterSet'으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-125">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="6100---october-2018"></a><span data-ttu-id="19d40-126">2018년 10월 - 6.10.0</span><span class="sxs-lookup"><span data-stu-id="19d40-126">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="19d40-127">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="19d40-127">Azure.Storage</span></span>
* <span data-ttu-id="19d40-128">대상에 메타데이터가 있을 때 Blob/파일이 메타 데이터를 복사하지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-128">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="19d40-129">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="19d40-129">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="19d40-130">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="19d40-130">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="19d40-131">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="19d40-131">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="19d40-132">기존 계정이 없는 Get-AzureRmCognitiveServicesAccountSkus를 지원</span><span class="sxs-lookup"><span data-stu-id="19d40-132">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="19d40-133">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="19d40-133">AzureRM.Compute</span></span>
* <span data-ttu-id="19d40-134">Get-AzureRmVM -ResourceGroupName <rg>가 필요한 경우 50개가 넘는 결과를 반환하도록 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-134">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="19d40-135">'SimpleParameterSet' 예제가 New-AzureRmVmss cmdlet 도움말에 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-135">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="19d40-136">Azure Disk Encryption 진행률 메시지의 오타를 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-136">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="19d40-137">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="19d40-137">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="19d40-138">ADF.Net SDK 버전을 2.3.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-138">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="19d40-139">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="19d40-139">AzureRM.Network</span></span>
* <span data-ttu-id="19d40-140">NetworkProfile 기능 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-140">Added NetworkProfile functionality.</span></span> <span data-ttu-id="19d40-141">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-141">new cmdlets added</span></span>
    - <span data-ttu-id="19d40-142">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="19d40-142">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="19d40-143">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="19d40-143">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="19d40-144">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="19d40-144">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="19d40-145">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="19d40-145">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="19d40-146">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-146">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="19d40-147">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-147">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="19d40-148">서브넷 모델에 서비스 연결 링크 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-148">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="19d40-149">New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-149">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="19d40-150">Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-150">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="19d40-151">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="19d40-151">AzureRM.RedisCache</span></span>
* <span data-ttu-id="19d40-152">모든 문자열을 Size 매개 변수로 진행되도록 허용</span><span class="sxs-lookup"><span data-stu-id="19d40-152">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="19d40-153">PSArgumentCompleter 팝업에 P5 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-153">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="19d40-154">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="19d40-154">AzureRM.Resources</span></span>
* <span data-ttu-id="19d40-155">-Mode 매개 변수를 Set-AzureRmPolicyDefinition에 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-155">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="19d40-156">사용자가 포함된 Origin 작업에서 Get-AzureRmProviderOperation commandlet 버그 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-156">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="19d40-157">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="19d40-157">AzureRM.Sql</span></span>
* <span data-ttu-id="19d40-158">일부 백업 cmdlet이 현재 azure 구독을 인식하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-158">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="19d40-159">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="19d40-159">AzureRM.Storage</span></span>
* <span data-ttu-id="19d40-160">특정 위치의 저장소 리소스 사용을 지원하고 글로벌 저장소 리소스 사용 가져오기는 더 이상 사용되지 않는다는 경고 메시지를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-160">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="19d40-161">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="19d40-161">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="19d40-162">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="19d40-162">AzureRM.Websites</span></span>
* <span data-ttu-id="19d40-163">새 cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - 컨테이너 지속적인 배포 Webhook URL을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-163">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="19d40-164">새 cmdlet 
New-AzureRMWebAppContainerPSSession 및 Enter-WebAppContainerPSSession -  windows 컨테이너 앱에 PowerShell 원격 세션을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-164">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="19d40-165">6.9.0 - 2018년 9월</span><span class="sxs-lookup"><span data-stu-id="19d40-165">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="19d40-166">일반</span><span class="sxs-lookup"><span data-stu-id="19d40-166">General</span></span>
* <span data-ttu-id="19d40-167">AzureRM.SignalR이 AzureRM 롤업 모듈에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-167">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="19d40-168">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="19d40-168">AzureRM.Profile</span></span>
* <span data-ttu-id="19d40-169">저장소 일반 코드에 대한 약간의 변경</span><span class="sxs-lookup"><span data-stu-id="19d40-169">Minor changes to the storage common code</span></span>
* <span data-ttu-id="19d40-170">전체 매개 변수 형식을 포함하도록 도움말 파일이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-170">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="19d40-171">-ServicePrincipal을 필수가 아닌 것으로 ServicePrincipalCertificateWithSubscriptionId 매개변수 집합에서 변경</span><span class="sxs-lookup"><span data-stu-id="19d40-171">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="19d40-172">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="19d40-172">Azure.Storage</span></span>
* <span data-ttu-id="19d40-173">OAuth를 사용하여 저장소 컨텍스트를 만드는 것을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-173">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="19d40-174">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="19d40-174">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="19d40-175">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="19d40-175">AzureRM.Cdn</span></span>
* <span data-ttu-id="19d40-176">Cdn 가격 책정 sku에서 Standard_Microsoft를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-176">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="19d40-177">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="19d40-177">AzureRM.Compute</span></span>
* <span data-ttu-id="19d40-178">Keyvault 및 Storage에서 종속성을 일반 종속성으로 이동</span><span class="sxs-lookup"><span data-stu-id="19d40-178">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="19d40-179">AEM cmdlet에 더 많은 가상 머신 크기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-179">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="19d40-180">PublicIPPrefix 매개 변수를 New-AzureRmVmssIpConfig에 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-180">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="19d40-181">Invoke-AzureRmVMRunCommand cmdelt에 ResourceId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-181">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="19d40-182">Invoke-AzureRmVmssVMRunCommand cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-182">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="19d40-183">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="19d40-183">AzureRM.Dns</span></span>
* <span data-ttu-id="19d40-184">Dns 레코드를 만드는 동안 별칭 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-184">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="19d40-185">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="19d40-185">AzureRM.Insights</span></span>
* <span data-ttu-id="19d40-186">#6833 및 #7102 문제 수정(진단 설정 영역)</span><span class="sxs-lookup"><span data-stu-id="19d40-186">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="19d40-187">기본 이름, 즉 'service'에 진단 설정의 목록 생성 및 가져오는 동안에 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-187">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="19d40-188">범주를 사용하는 진단 설정 만들기 문제</span><span class="sxs-lookup"><span data-stu-id="19d40-188">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="19d40-189">메트릭 시간 조직 매개 변수에 대한 사용 중단 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-189">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="19d40-190">Timegrains 매개 변수는 여전히 받아들여지고 있습니다(이것은 호환성이 손상되는 변경이 아닙니다). 그러나 PT1M만 유효하므로 백엔드에서 무시됩니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-190">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="19d40-191">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="19d40-191">AzureRM.Network</span></span>
* <span data-ttu-id="19d40-192">LoadBalancer cmdlet에 대한 변경</span><span class="sxs-lookup"><span data-stu-id="19d40-192">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="19d40-193">LoadBalancerInboundNatPoolConfig: IdleTimeoutInMinutes, EnableFloatingIp 및 EnableTcpReset 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-193">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="19d40-194">LoadBalancerInboundNatRuleConfig: EnableTcpReset 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-194">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="19d40-195">LoadBalancerRuleConfig: EnableTcpReset 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-195">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="19d40-196">LoadBalancerProbeConfig: 매개 변수 프로토콜에 대해 "Https" 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-196">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="19d40-197">새 LoadBalancer의 하위 리소스OutboundRule에 대한 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-197">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="19d40-198">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-198">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="19d40-199">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-199">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="19d40-200">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-200">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="19d40-201">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-201">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="19d40-202">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-202">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="19d40-203">PSNetworkInterface에 대한 새 HostedWorkloads 속성 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-203">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="19d40-204">기능에 대한 새 cmdlet 추가: ARM을 통한 Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="19d40-204">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="19d40-205">Get-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-205">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="19d40-206">Set-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-206">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="19d40-207">New-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-207">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="19d40-208">Remove-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-208">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="19d40-209">New-AzureRmFirewallApplicationRuleCollection 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-209">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="19d40-210">New-AzureRmFirewallApplicationRule 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-210">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="19d40-211">New-AzureRmFirewallNatRuleCollection 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-211">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="19d40-212">New-AzureRmFirewallNatRule 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-212">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="19d40-213">New-AzureRmFirewallNetworkRuleCollection 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-213">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="19d40-214">New-AzureRmFirewallNetworkRule 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-214">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="19d40-215">Application Gateway에서 신뢰할 수 있는 루트 인증서 및 크기 자동 조정 구성에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-215">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="19d40-216">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-216">New Cmdlets added:</span></span>
      - <span data-ttu-id="19d40-217">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="19d40-217">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="19d40-218">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="19d40-218">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="19d40-219">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="19d40-219">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="19d40-220">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="19d40-220">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="19d40-221">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="19d40-221">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="19d40-222">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="19d40-222">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="19d40-223">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="19d40-223">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="19d40-224">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="19d40-224">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="19d40-225">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="19d40-225">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="19d40-226">옵션 매개 변수를 사용하도록 업데이트된 Cmdlet-TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="19d40-226">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="19d40-227">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="19d40-227">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="19d40-228">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="19d40-228">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="19d40-229">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="19d40-229">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="19d40-230">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="19d40-230">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="19d40-231">옵션 매개 변수를 사용하도록 업데이트된 Cmdlet-AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="19d40-231">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="19d40-232">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="19d40-232">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="19d40-233">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="19d40-233">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="19d40-234">인터페이스 엔드포인트 Get-AzureInterfaceEndpoint에 대한 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-234">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="19d40-235">서브넷에서 여러 주소 접두사에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-235">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="19d40-236">다음 Cmdlet이 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-236">Updated cmdlets:</span></span>
  - <span data-ttu-id="19d40-237">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-237">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="19d40-238">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-238">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="19d40-239">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-239">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="19d40-240">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-240">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="19d40-241">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="19d40-241">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="19d40-242">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-242">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="19d40-243">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-243">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="19d40-244">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-244">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="19d40-245">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="19d40-245">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="19d40-246">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="19d40-246">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="19d40-247">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="19d40-247">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="19d40-248">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-248">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="19d40-249">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-249">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="19d40-250">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-250">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="19d40-251">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-251">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="19d40-252">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-252">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="19d40-253">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-253">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="19d40-254">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-254">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="19d40-255">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="19d40-255">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="19d40-256">서브넷 위임에 대한 cmdlet을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-256">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="19d40-257">New-AzureRmDelegation: 서브넷에 추가할 수 있는 새 위임을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-257">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="19d40-258">Remove-AzureRmDelegation: 서브넷에서 가져와서 해당 서브넷에서 제공된 위임 이름을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-258">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="19d40-259">Add-AzureRmDelegation: 서브넷에서 사용 및 제공된 서비스 이름을 해당 서브넷에 대한 위임으로 추가합니다</span><span class="sxs-lookup"><span data-stu-id="19d40-259">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="19d40-260">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="19d40-260">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="19d40-261">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="19d40-261">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="19d40-262">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="19d40-262">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="19d40-263">관리되는 관리 디스크에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="19d40-263">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="19d40-264">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="19d40-264">AzureRM.RedisCache</span></span>
* <span data-ttu-id="19d40-265">인사이트 종속성이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-265">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="19d40-266">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="19d40-266">AzureRM.Resources</span></span>
* <span data-ttu-id="19d40-267">New-AzureRmResourceGroupDeployment를 RollbackAction 새 매개 변수를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-267">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="19d40-268">새 매개 변수를 사용하여 OnErrorDeployment에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-268">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="19d40-269">정책 할당에서 관리되는 ID를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-269">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="19d40-270">'New-AzureRmPolicyAssignment'를 사용하여 정책을 할당할 때 기본값이 있는 매개 변수는 더 이상 필요하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-270">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="19d40-271">정책 별칭을 검색하기 위한 새 cmdlet Get-AzureRmPolicyAlias 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-271">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="19d40-272">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="19d40-272">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="19d40-273">#7161 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-273">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="19d40-274">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="19d40-274">AzureRM.SignalR</span></span>
* <span data-ttu-id="19d40-275">SKU 이름을 Free_F1 및 Standard_S1로 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-275">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="19d40-276">버전 필드를 PSSignalRResource 개체에 추가하고 연결 문자열을 PSSignalRKeys개체에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-276">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="19d40-277">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="19d40-277">AzureRM.Storage</span></span>
* <span data-ttu-id="19d40-278">AzureRm.Storage에서 불변성 정책 지원</span><span class="sxs-lookup"><span data-stu-id="19d40-278">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="19d40-279">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="19d40-279">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="19d40-280">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="19d40-280">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="19d40-281">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="19d40-281">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="19d40-282">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="19d40-282">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="19d40-283">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="19d40-283">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="19d40-284">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="19d40-284">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="19d40-285">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="19d40-285">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="19d40-286">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="19d40-286">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="19d40-287">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="19d40-287">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="19d40-288">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="19d40-288">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="19d40-289">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="19d40-289">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="19d40-290">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="19d40-290">AzureRM.Websites</span></span>
* <span data-ttu-id="19d40-291">두 개의 새로운 cmdlet 추가: Get-AzureRmDeletedWebApp 및 Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="19d40-291">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="19d40-292">New-AzureRmAppServicePlan -HyperV 스위치가 창 컨테이너가 있는 앱 서비스 계획 작성용으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-292">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="19d40-293">New-AzureRmWebApp/New-AzureRmWebAppSlot/Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - Windows 컨테이너 앱을 만들고 관리하기 위한 새 매개 변수(-ContainerRegistryUser 문자열 -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment)가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-293">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="19d40-294">6.8.1 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="19d40-294">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="19d40-295">일반</span><span class="sxs-lookup"><span data-stu-id="19d40-295">General</span></span>
* <span data-ttu-id="19d40-296">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-296">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="19d40-297">공용 런타임 어셈블리가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-297">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="19d40-298">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="19d40-298">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="19d40-299">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-299">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="19d40-300">문제 https://github.com/Azure/azure-powershell/issues/6603 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-300">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="19d40-301">Import-AzureRmApiManagementApi 및 \*-AzureRmApiManagementCertificate cmdlet은 이제 상대 경로를 처리합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-301">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="19d40-302">문제 https://github.com/Azure/azure-powershell/issues/6879 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-302">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="19d40-303">CertificateInformation은 Set-AzureRmApiManagement cmdlet이 제대로 작동 하게 하는 설정 가능한 속성입니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-303">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="19d40-304">4.0.4-preview nuget으로 업그레이드하여 해결됨</span><span class="sxs-lookup"><span data-stu-id="19d40-304">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="19d40-305">문제 https://github.com/Azure/azure-powershell/issues/6853 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-305">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="19d40-306">제품에서 이름별 검색에 대해 Odata 필터가 수정됨</span><span class="sxs-lookup"><span data-stu-id="19d40-306">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="19d40-307">문제 https://github.com/Azure/azure-powershell/issues/6814 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-307">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="19d40-308">API에서 이름별 검색에 대해 Odata 필터가 수정됨</span><span class="sxs-lookup"><span data-stu-id="19d40-308">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="19d40-309">AzureMonitor 로거에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-309">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="19d40-310">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="19d40-310">AzureRM.Compute</span></span>
* <span data-ttu-id="19d40-311">오류 출력에 대상이 없는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-311">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="19d40-312">관리 디스크를 사용하는 VM에 대한 저장소 계정 유형 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-312">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="19d40-313">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-313">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="19d40-314">예를 들어 Azure 중국과 같이, 다른 환경에 대한 AEM 확장 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-314">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="19d40-315">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="19d40-315">AzureRM.Network</span></span>
* <span data-ttu-id="19d40-316">기본 cmdlet 출력 표시를 테이블 뷰로 변경</span><span class="sxs-lookup"><span data-stu-id="19d40-316">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="19d40-317">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="19d40-317">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="19d40-318">일시 중지된 용량을 확장하려고 할 때 Update-AzureRmPowerBIEmbeddedCapacity 실패 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-318">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="19d40-319">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="19d40-319">AzureRM.Resources</span></span>
* <span data-ttu-id="19d40-320">MarketPlace에서 관리되는 응용 프로그램 생성 시의 문제 해결.</span><span class="sxs-lookup"><span data-stu-id="19d40-320">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="19d40-321">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="19d40-321">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="19d40-322">해결된 문제</span><span class="sxs-lookup"><span data-stu-id="19d40-322">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="19d40-323">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="19d40-323">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="19d40-324">다중값 라우팅 메서드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-324">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="19d40-325">다중값 라우팅에 대한 새 매개 변수 'MaxReturn'</span><span class="sxs-lookup"><span data-stu-id="19d40-325">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="19d40-326">서브넷 라우팅 메서드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-326">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="19d40-327">엔드포인트의 IP 주소 범위(서브넷)에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="19d40-327">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="19d40-328">프로필 내 사용자 지정 헤더에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-328">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="19d40-329">프로필 내 예상 상태 코드 범위에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-329">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="19d40-330">엔드포인트 내 사용자 지정 헤더에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-330">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="19d40-331">6.8.0 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="19d40-331">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="19d40-332">일반</span><span class="sxs-lookup"><span data-stu-id="19d40-332">General</span></span>
* <span data-ttu-id="19d40-333">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-333">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="19d40-334">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="19d40-334">AzureRM.Profile</span></span>
* <span data-ttu-id="19d40-335">Connect-AzureRmAccount 중에 반환된 토큰에 만료 속성 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-335">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="19d40-336">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="19d40-336">AzureRM.Compute</span></span>
* <span data-ttu-id="19d40-337">오류 출력에 대상이 없는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-337">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="19d40-338">관리 디스크를 사용하는 VM에 대한 저장소 계정 유형 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-338">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="19d40-339">예를 들어 Azure 중국과 같이, 다른 환경에 대한 AEM 확장 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-339">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="19d40-340">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="19d40-340">AzureRM.IotHub</span></span>
* <span data-ttu-id="19d40-341">New-AzureRmIotHubExportDevices 및 New-AzureRmIotHubImportDevices에 대한 예제를 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-341">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="19d40-342">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="19d40-342">AzureRM.Network</span></span>
* <span data-ttu-id="19d40-343">기본 모델 표시를 테이블 뷰로 변경</span><span class="sxs-lookup"><span data-stu-id="19d40-343">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="19d40-344">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="19d40-344">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="19d40-345">일시 중지된 용량을 확장하려고 할 때 Update-AzureRmPowerBIEmbeddedCapacity 실패 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-345">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="19d40-346">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="19d40-346">AzureRM.Resources</span></span>
* <span data-ttu-id="19d40-347">MarketPlace에서 관리되는 응용 프로그램 생성 시의 문제 해결.</span><span class="sxs-lookup"><span data-stu-id="19d40-347">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="19d40-348">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="19d40-348">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="19d40-349">문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-349">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="19d40-350">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="19d40-350">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="19d40-351">다중값 라우팅 메서드에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="19d40-351">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="19d40-352">다중값 라우팅에 대한 새 매개 변수 'MaxReturn'</span><span class="sxs-lookup"><span data-stu-id="19d40-352">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="19d40-353">서브넷 라우팅 메서드에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="19d40-353">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="19d40-354">엔드포인트의 IP 주소 범위(서브넷)에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="19d40-354">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="19d40-355">프로필 내 사용자 지정 헤더에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="19d40-355">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="19d40-356">프로필 내 예상 상태 코드 범위에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="19d40-356">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="19d40-357">엔드포인트 내 사용자 지정 헤더에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="19d40-357">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="19d40-358">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="19d40-358">AzureRM.Websites</span></span>
* <span data-ttu-id="19d40-359">기본 리소스 그룹이 잘못 설정되는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-359">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="19d40-360">6.7.0 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="19d40-360">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="19d40-361">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="19d40-361">AzureRM.Profile</span></span>
* <span data-ttu-id="19d40-362">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-362">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="19d40-363">충돌을 방지하려면 기본 컨텍스트 이름으로 사용자 ID를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-363">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="19d40-364">#6398 컨텍스트를 선택할 때 문제를 발생시킨 Clear-AzureRmContext 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-364">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="19d40-365">'Connect-AzureRmAccount'에 대한 '-TenantId' 매개 변수에 전달할 테넌트 도메인을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="19d40-365">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="19d40-366">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="19d40-366">Azure.Storage</span></span>
* <span data-ttu-id="19d40-367">Azure 파일 공유 할당량에 대한 5TB 제한 제거</span><span class="sxs-lookup"><span data-stu-id="19d40-367">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="19d40-368">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="19d40-368">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="19d40-369">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="19d40-369">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="19d40-370">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-370">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="19d40-371">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="19d40-371">Azure.AnalysisServices</span></span>
* <span data-ttu-id="19d40-372">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-372">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="19d40-373">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="19d40-373">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="19d40-374">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-374">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="19d40-375">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="19d40-375">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="19d40-376">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-376">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="19d40-377">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="19d40-377">AzureRM.Automation</span></span>
* <span data-ttu-id="19d40-378">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-378">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="19d40-379">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="19d40-379">AzureRM.Backup</span></span>
* <span data-ttu-id="19d40-380">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-380">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="19d40-381">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="19d40-381">AzureRM.Batch</span></span>
* <span data-ttu-id="19d40-382">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-382">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="19d40-383">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="19d40-383">AzureRM.Billing</span></span>
* <span data-ttu-id="19d40-384">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-384">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="19d40-385">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="19d40-385">AzureRM.Cdn</span></span>
* <span data-ttu-id="19d40-386">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-386">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="19d40-387">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="19d40-387">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="19d40-388">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-388">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="19d40-389">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="19d40-389">AzureRM.Compute</span></span>
* <span data-ttu-id="19d40-390">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-390">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="19d40-391">New-AzureRmVmssConfig에 EvictionPolicy 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-391">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="19d40-392">지정된 위치가 없는 경우에 New-AzureRmVm의 DiskFileParameterSet 내의 기본 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-392">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="19d40-393">Save-AzureRmVMImage에서 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-393">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="19d40-394">특정 singlepass 관련 시나리오에 대해 Get-AzureRmVMDiskEncryptionStatus cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-394">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="19d40-395">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="19d40-395">AzureRM.Consumption</span></span>
* <span data-ttu-id="19d40-396">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="19d40-397">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="19d40-397">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="19d40-398">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-398">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="19d40-399">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="19d40-399">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="19d40-400">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-400">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="19d40-401">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="19d40-401">AzureRM.DataFactories</span></span>
* <span data-ttu-id="19d40-402">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-402">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="19d40-403">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="19d40-403">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="19d40-404">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-404">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="19d40-405">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="19d40-405">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="19d40-406">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="19d40-407">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="19d40-407">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="19d40-408">DebugPreference가 powershell 명령줄에서 설정된 경우 디버깅 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-408">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="19d40-409">Set-AzureRmDataLakeStoreItemAcl에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-409">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="19d40-410">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-410">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="19d40-411">Set-AzureRmDataLakeStoreItemAclEntry에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-411">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="19d40-412">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="19d40-412">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="19d40-413">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-413">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="19d40-414">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="19d40-414">AzureRM.Dns</span></span>
* <span data-ttu-id="19d40-415">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-415">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="19d40-416">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="19d40-416">AzureRM.EventGrid</span></span>
* <span data-ttu-id="19d40-417">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-417">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="19d40-418">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="19d40-418">AzureRM.EventHub</span></span>
* <span data-ttu-id="19d40-419">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-419">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="19d40-420">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="19d40-420">AzureRM.HDInsight</span></span>
* <span data-ttu-id="19d40-421">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-421">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="19d40-422">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="19d40-422">AzureRM.Insights</span></span>
* <span data-ttu-id="19d40-423">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-423">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="19d40-424">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="19d40-424">AzureRM.IotHub</span></span>
* <span data-ttu-id="19d40-425">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-425">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="19d40-426">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="19d40-426">AzureRM.KeyVault</span></span>
* <span data-ttu-id="19d40-427">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="19d40-428">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="19d40-428">AzureRM.LogicApp</span></span>
* <span data-ttu-id="19d40-429">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="19d40-430">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="19d40-430">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="19d40-431">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="19d40-432">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="19d40-432">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="19d40-433">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="19d40-434">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="19d40-434">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="19d40-435">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="19d40-436">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="19d40-436">AzureRM.Media</span></span>
* <span data-ttu-id="19d40-437">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-437">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="19d40-438">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="19d40-438">AzureRM.Network</span></span>
* <span data-ttu-id="19d40-439">Set-AzureRmLocalNetworkGateway에 대한 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-439">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="19d40-440">Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey, New-AzureRmVirtualNetworkGatewayConnection에 대한 예제 및 설명 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-440">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="19d40-441">Remove-AzureRmVirtualNetworkGatewayIpConfig 및 Reset-AzureRmVirtualNetworkGateway에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-441">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="19d40-442">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-442">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="19d40-443">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-443">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="19d40-444">Set-AzureRmVirtualNetworkGatewayConnection에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-444">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="19d40-445">최신 코드 생성기를 사용하여 ApplicationSecurityGroup, RouteTable 및 Usage에 대한 cmdlet을 다시 생성함</span><span class="sxs-lookup"><span data-stu-id="19d40-445">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="19d40-446">Exitc 하지 않는 서브넷을 얻으려고 할 때의 Get-AzureRmVirtualNetworkSubnetConfig에 대한 오류 메시지를 설명</span><span class="sxs-lookup"><span data-stu-id="19d40-446">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="19d40-447">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="19d40-447">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="19d40-448">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-448">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="19d40-449">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="19d40-449">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="19d40-450">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-450">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="19d40-451">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="19d40-451">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="19d40-452">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-452">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="19d40-453">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="19d40-453">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="19d40-454">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-454">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="19d40-455">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="19d40-455">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="19d40-456">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-456">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="19d40-457">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="19d40-457">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="19d40-458">Get-AzureRmRecoveryServicesBackItem cmdlet에 정책 필터 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-458">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="19d40-459">해당 명령은 지정된 정책 ID에 의해 보호되는 백업 항목의 목록을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-459">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="19d40-460">Microsoft.Azure.Management.RecoveryServices.Backup을 버전 3.0.0-preview로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="19d40-460">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="19d40-461">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-461">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="19d40-462">Restore-AzureRmRecoveryServicesBackupItem에 TargetResourceGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-462">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="19d40-463">관리 디스크가 복원될 리소스 그룹</span><span class="sxs-lookup"><span data-stu-id="19d40-463">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="19d40-464">관리 디스크가 있는 VM의 백업에 적용 가능</span><span class="sxs-lookup"><span data-stu-id="19d40-464">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="19d40-465">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="19d40-465">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="19d40-466">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-466">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="19d40-467">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="19d40-467">AzureRM.RedisCache</span></span>
* <span data-ttu-id="19d40-468">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-468">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="19d40-469">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="19d40-469">AzureRM.Relay</span></span>
* <span data-ttu-id="19d40-470">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-470">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="19d40-471">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="19d40-471">AzureRM.Resources</span></span>
* <span data-ttu-id="19d40-472">구독 범위에서 템플릿 배포를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-472">Support template deployment at subscription scope.</span></span> <span data-ttu-id="19d40-473">새 cmdlet 추가:</span><span class="sxs-lookup"><span data-stu-id="19d40-473">Add new Cmdlets:</span></span>
    - <span data-ttu-id="19d40-474">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="19d40-474">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="19d40-475">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="19d40-475">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="19d40-476">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="19d40-476">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="19d40-477">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="19d40-477">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="19d40-478">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="19d40-478">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="19d40-479">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="19d40-479">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="19d40-480">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="19d40-480">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="19d40-481">Set-AzureRmResource에 컨텍스트를 전달할 때 오류가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-481">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="19d40-482">New-AzureRmResourceGroupDeployment의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-482">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="19d40-483">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-483">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="19d40-484">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="19d40-484">AzureRM.Scheduler</span></span>
* <span data-ttu-id="19d40-485">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-485">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="19d40-486">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="19d40-486">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="19d40-487">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-487">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="19d40-488">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="19d40-488">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="19d40-489">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-489">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="19d40-490">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="19d40-490">AzureRM.Sql</span></span>
* <span data-ttu-id="19d40-491">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-491">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="19d40-492">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="19d40-492">AzureRM.Storage</span></span>
* <span data-ttu-id="19d40-493">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-493">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="19d40-494">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="19d40-494">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="19d40-495">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-495">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="19d40-496">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="19d40-496">AzureRM.Tags</span></span>
* <span data-ttu-id="19d40-497">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-497">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="19d40-498">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="19d40-498">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="19d40-499">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-499">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="19d40-500">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="19d40-500">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="19d40-501">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-501">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="19d40-502">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="19d40-502">AzureRM.Websites</span></span>
* <span data-ttu-id="19d40-503">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-503">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="19d40-504">6.6.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="19d40-504">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="19d40-505">일반</span><span class="sxs-lookup"><span data-stu-id="19d40-505">General</span></span>
* <span data-ttu-id="19d40-506">전체 매개 변수 형식 및 올바른 입/출력 형식을 포함하도록 모든 도움말 파일을 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-506">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="19d40-507">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="19d40-507">AzureRM.Profile</span></span>
* <span data-ttu-id="19d40-508">Common.Strategy 라이브러리가 리소스에 대한 현재 구성이 대상 리소스와 호환되는지 유효성을 검사할 수 있도록 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-508">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="19d40-509">Common.Storage에 ps1xml 형식 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-509">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="19d40-510">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="19d40-510">Azure.Storage</span></span>
* <span data-ttu-id="19d40-511">DefaultProfile에서 저장소 컨텍스트를 가져오기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-511">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="19d40-512">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-512">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="19d40-513">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="19d40-513">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="19d40-514">문제 https://github.com/Azure/azure-powershell/issues/6370 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-514">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="19d40-515">PsApiManagementApi를 ApiContract로 좌표 이동하도록 Automapper 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="19d40-515">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="19d40-516">문제 https://github.com/Azure/azure-powershell/issues/6515 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-516">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="19d40-517">인코딩 형식을 사용하여 오버로드하지 않도록 File.Save 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="19d40-517">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="19d40-518">문제 https://github.com/Azure/azure-powershell/issues/6560 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-518">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="19d40-519">apiId에서 패턴 예외를 수정하는 4.0.3 Nuget 버전으로 업그레이드됨</span><span class="sxs-lookup"><span data-stu-id="19d40-519">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="19d40-520">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="19d40-520">AzureRM.Compute</span></span>
* <span data-ttu-id="19d40-521">PremiumLRS 저장소 계정 형식 이름 바꾸기로 인해 New-AzureRmVm에서 DiskFileParameterSet를 사용하여 vm 생성 시 실패하는 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-521">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="19d40-522">Invoke-AzureRmVMRunCommand cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-522">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="19d40-523">Get-AzureRmAvailabilitySet를 업데이트하여 구독에서 모든 가용성 집합 리스트를 사용하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-523">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="19d40-524">(ResouceGroupName 매개 변수는 이제 선택적 요소입니다.)</span><span class="sxs-lookup"><span data-stu-id="19d40-524">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="19d40-525">vm 선별에 가속화된 네트워크를 사용하도록 'New-AzureRmVm'의 SimpleParameterSet를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-525">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="19d40-526">New-AzureRmVmss 간단 매개 변수가 사용자 지정 LB가 이미 존재할 때 vms 생성에 실패하도록 설정하여 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-526">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="19d40-527">New-AzureRmDisk에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-527">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="19d40-528">'New-AzureRmVM'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-528">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="19d40-529">Set-AzureRmVMOSDisk에 대한 설명 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-529">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="19d40-530">Set-AzureRmVMBginfoExtension 맞춤법 및 접두사를 수정하도록 예제 1을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-530">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="19d40-531">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="19d40-531">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="19d40-532">ADF.Net SDK 버전을 1.1.0으로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-532">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="19d40-533">데이터 팩터리를 공유하는 자체 호스팅된 통합 런타임을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-533">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="19d40-534">새 매개 변수 -SharedIntegrationRuntimeResourceId를 Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="19d40-534">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="19d40-535">새로운 선택적 매개 변수 -LinkedDataFactoryName을 Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="19d40-535">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="19d40-536">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="19d40-536">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="19d40-537">DataPlane SDK(Microsoft.Azure.DataLake.Store) 버전을 1.1.9로 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-537">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="19d40-538">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="19d40-538">AzureRM.EventHub</span></span>
* <span data-ttu-id="19d40-539">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-539">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="19d40-540">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="19d40-540">AzureRM.Insights</span></span>
* <span data-ttu-id="19d40-541">도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-541">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="19d40-542">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview를 사용</span><span class="sxs-lookup"><span data-stu-id="19d40-542">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="19d40-543">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="19d40-543">AzureRM.KeyVault</span></span>
* <span data-ttu-id="19d40-544">Set-AzureRmKeyVaultAccessPolicy 내 파이핑 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-544">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="19d40-545">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="19d40-545">AzureRM.Network</span></span>
* <span data-ttu-id="19d40-546">LoadBalancerInboundNatPoolConfig cmdlet에 대한 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-546">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="19d40-547">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="19d40-547">AzureRM.Resources</span></span>
* <span data-ttu-id="19d40-548">'Get-AzureRmResource'에 대한 태그 이름 및 값을 제공할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-548">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="19d40-549">'Set-AzureRmResource'를 사용하여 파이핑 시나리오 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-549">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="19d40-550">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="19d40-550">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="19d40-551">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-551">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="19d40-552">몇 가지 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-552">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="19d40-553">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="19d40-553">AzureRM.Sql</span></span>
* <span data-ttu-id="19d40-554">다음 cmdlet 사용하여 서버 Advanced Threat Protection 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-554">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="19d40-555">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="19d40-555">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="19d40-556">다음 cmdlet을 사용하여 취약성 평가 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-556">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="19d40-557">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="19d40-557">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="19d40-558">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="19d40-558">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="19d40-559">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="19d40-559">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="19d40-560">Remove-AzureRmSqlServerFirewallRule의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-560">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="19d40-561">Get-AzureSqlSyncGroupLog에서 미국이 아닌 문화권에서 날짜/시간을 올바르지 않게 다루는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-561">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="19d40-562">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="19d40-562">AzureRM.Storage</span></span>
* <span data-ttu-id="19d40-563">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-563">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="19d40-564">StorageAccount cmdlet 출력을 테이블 뷰로 표시</span><span class="sxs-lookup"><span data-stu-id="19d40-564">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="19d40-565">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="19d40-565">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="19d40-566">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="19d40-566">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="19d40-567">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="19d40-567">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="19d40-568">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="19d40-568">AzureRM.Tags</span></span>
* <span data-ttu-id="19d40-569">태그 cmdlet 도움말에서 잘못된 문을 제거합니다</span><span class="sxs-lookup"><span data-stu-id="19d40-569">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="19d40-570">6.5.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="19d40-570">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="19d40-571">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="19d40-571">AzureRM.Profile</span></span>
* <span data-ttu-id="19d40-572">'Get-AzureRmContextAutosaveSetting'에 대한 도움말이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-572">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="19d40-573">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="19d40-573">Azure.Storage</span></span>
* <span data-ttu-id="19d40-574">쓰기 전용 SaS 토큰을 사용하는 Blob 또는 파일 업로드 지원</span><span class="sxs-lookup"><span data-stu-id="19d40-574">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="19d40-575">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="19d40-575">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="19d40-576">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="19d40-576">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="19d40-577">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="19d40-577">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="19d40-578">필수 속성 ResourceGroupName을 AS에 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-578">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="19d40-579">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="19d40-579">AzureRM.Automation</span></span>
* <span data-ttu-id="19d40-580">도움말을 업데이트하고 'New-AzureRMAutomationSchedule'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-580">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="19d40-581">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="19d40-581">AzureRM.Compute</span></span>
* <span data-ttu-id="19d40-582">-Tag 매개 변수를 Update/New-AzureRmAvailabilitySet에 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-582">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="19d40-583">‘Add-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-583">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="19d40-584">‘Remove-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-584">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="19d40-585">‘Set-AzureRmVMAccessExtension’에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-585">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="19d40-586">기본으로 SinglePlacementGroup을 false로 설정하고 단일 배치 그룹에 VMSS를 만들 수 있는 스위치 매개 변수 'SinglePlacementGroup'을 추가하도록 New-AzureRmVmss에 대한 SimpleParameterSet을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-586">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="19d40-587">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="19d40-587">AzureRM.EventHub</span></span>
* <span data-ttu-id="19d40-588">PSEventHubDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="19d40-588">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="19d40-589">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="19d40-589">AzureRM.KeyVault</span></span>
* <span data-ttu-id="19d40-590">Set-AzureRmKeyVaultAccessPolicy에 대한 오류 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-590">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="19d40-591">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="19d40-591">AzureRM.LogicApp</span></span>
* <span data-ttu-id="19d40-592">New-AzureRmLogicApp에서 "매개 변수 집합을 확인할 수 없습니다" 오류 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-592">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="19d40-593">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="19d40-593">AzureRM.Network</span></span>
* <span data-ttu-id="19d40-594">Set/Add-AzureRmVirtualNetworkPeering에 대한 여러 테넌트의 가상 네트워크에서 피어링을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="19d40-594">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="19d40-595">Application Gateway에 대한 아래 cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-595">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="19d40-596">New-AzureRmApplicationGateway: EnableFIPS 플래그 및 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-596">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="19d40-597">New-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-597">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="19d40-598">Set-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-598">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="19d40-599">최신 생성기를 사용하여 RouteTable cmdlet을 재생성</span><span class="sxs-lookup"><span data-stu-id="19d40-599">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="19d40-600">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="19d40-600">AzureRM.Relay</span></span>
* <span data-ttu-id="19d40-601">markdown 파일을 업데이트하여 예제에서 매개 변수 이름 문제에 대해 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-601">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="19d40-602">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="19d40-602">AzureRM.Resources</span></span>
* <span data-ttu-id="19d40-603">Roledefinition 및 Roleassignment cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-603">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="19d40-604">페이징의 일부분으로 수행하는 추가 roledefinition 호출을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-604">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="19d40-605">Get-AzureRmRoleAssignment cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-605">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="19d40-606">-ExpandPrincipalGroups 명령 매개 변수 기능 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-606">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="19d40-607">'Get-AzureRmResource'에서 '-ResourceType' 매개 변수가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-607">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="19d40-608">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="19d40-608">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="19d40-609">top 및 skip 매개 변수가 cmdlet 목록을 나열하도록 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-609">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="19d40-610">표준을 프리미엄 네임스페이스 마이그레이션 cmdlet에 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-610">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="19d40-611">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="19d40-611">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="19d40-612">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="19d40-612">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="19d40-613">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="19d40-613">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="19d40-614">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="19d40-614">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="19d40-615">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="19d40-615">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="19d40-616">PSServiceBusDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="19d40-616">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="19d40-617">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="19d40-617">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="19d40-618">‘New-AzureRmServiceFabricCluster’에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-618">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="19d40-619">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="19d40-619">AzureRM.Sql</span></span>
* <span data-ttu-id="19d40-620">Management.Sql에 대한 새 cmdlet을 추가하여 고객이 TDE 인증서를 SQL Server 인스턴스 또는 Managed Instance에 추가할 수 있도록 허용</span><span class="sxs-lookup"><span data-stu-id="19d40-620">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="19d40-621">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="19d40-621">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="19d40-622">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="19d40-622">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="19d40-623">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="19d40-623">AzureRM.Websites</span></span>
* <span data-ttu-id="19d40-624">`Set-AzureRmWebApp -AssignIdentity` 및 `Set-AzureRmWebAppSlot -AssignIdentity`가 false로 설정되면 사이트 개체에서 Identity 속성이 제거됩니다. 미리보기 태그도 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-624">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="19d40-625">`Get-AzureRmWebAppMetrics`, `Get-AzureRmAppServicePlanMetrics` 예제가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-625">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="19d40-626">`Set-AzureRmWebApp -PhpVersion`이 유효한 php 버전으로 해제 지원</span><span class="sxs-lookup"><span data-stu-id="19d40-626">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="19d40-627">6.4.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="19d40-627">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="19d40-628">일반</span><span class="sxs-lookup"><span data-stu-id="19d40-628">General</span></span>
* <span data-ttu-id="19d40-629">대부분의 모듈에 대한 도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-629">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="19d40-630">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="19d40-630">AzureRM.Profile</span></span>
* <span data-ttu-id="19d40-631">기본 출력 형식에 추가된 Ps1Xml 특성</span><span class="sxs-lookup"><span data-stu-id="19d40-631">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="19d40-632">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="19d40-632">AzureRM.Compute</span></span>
* <span data-ttu-id="19d40-633">VMSS에 대한 IP 태그 기능</span><span class="sxs-lookup"><span data-stu-id="19d40-633">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="19d40-634">'New-AzureRmVmssIpTagConfig' cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-634">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="19d40-635">New-AzureRmVmssIpConfig에 IpTag 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-635">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="19d40-636">VMSS에 대한 자동 OS 롤백 기능</span><span class="sxs-lookup"><span data-stu-id="19d40-636">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="19d40-637">New-AzureRmVmssConfig 및 Update-AzureRmVmss에 DisableAutoRollback 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-637">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="19d40-638">Vmss에 대한 OS 업그레이드 기록 기능</span><span class="sxs-lookup"><span data-stu-id="19d40-638">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="19d40-639">Get-AzureRmVmss에 OSUpgradeHistory 스위치 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-639">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="19d40-640">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="19d40-640">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="19d40-641">다음 명령을 통해 카탈로그 액세스 제어 목록에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-641">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="19d40-642">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="19d40-642">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="19d40-643">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="19d40-643">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="19d40-644">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="19d40-644">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="19d40-645">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="19d40-645">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="19d40-646">Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl에 대한 취소 지원 및 진행률 추적 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-646">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="19d40-647">Export-AzureRmDataLakeStoreChildItemProperties에 대한 취소 지원 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-647">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="19d40-648">재귀 작업을 수행하는 cmdlet에 대한 디버그 메시지 플러시 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-648">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="19d40-649">DataLake cmdlet의 테스트 위치 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-649">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="19d40-650">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="19d40-650">AzureRM.EventHub</span></span>
* <span data-ttu-id="19d40-651">목록 작업 cmdlet Get-AzureRmEventHub 및 Get-AzureRmEventHubConsumerGroup에 선택적 MaxCount 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-651">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="19d40-652">새 EventHub 만드는 동안 하나 이상의 매개 변수가 필요한 New-AzureRmEventHub cmdlet 문제를 해결.</span><span class="sxs-lookup"><span data-stu-id="19d40-652">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="19d40-653">기본 매개 변수 집합을 제공.</span><span class="sxs-lookup"><span data-stu-id="19d40-653">Provided Default Parameter set.</span></span>
* <span data-ttu-id="19d40-654">선택적 매개 변수 -KeyValue를 New-AzureRmEventHubKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-654">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="19d40-655">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="19d40-655">AzureRM.KeyVault</span></span>
* <span data-ttu-id="19d40-656">Get-AzureRmKeyVault -Tag 실행 시 모든 리소스가 리턴되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-656">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="19d40-657">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="19d40-657">AzureRM.Network</span></span>
* <span data-ttu-id="19d40-658">영역 중복 VirtualNetworkGateways에 대한 새 Sku를 노출합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-658">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="19d40-659">기능에 대한 새 명령이 추가됨: ARM을 통한 ExpressRoute Partner APIs</span><span class="sxs-lookup"><span data-stu-id="19d40-659">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="19d40-660">Get- AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-660">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="19d40-661">Set-AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-661">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="19d40-662">Add-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-662">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="19d40-663">Get-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-663">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="19d40-664">Remove-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-664">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="19d40-665">Get-AzureRMExpressRouteCrossConnectionArpTable 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-665">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="19d40-666">Get-AzureRMExpressRouteCrossConnectionRouteTable 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-666">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="19d40-667">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-667">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="19d40-668">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="19d40-668">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="19d40-669">Get-AzureRmRecoveryServicesBackupStatus cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-669">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="19d40-670">이 cmdlet은 VM ID를 가져와서 VM이 구독에서 일부 자격 증명 모음으로 보호되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-670">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="19d40-671">이러한 자격 증명 모음이 존재하는 경우 cmdlet은 자격 증명 모음 세부 정보를 출력 합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-671">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="19d40-672">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="19d40-672">AzureRM.Resources</span></span>
* <span data-ttu-id="19d40-673">Get-AzureRmPolicyAssignment cmdlet을 다음과 같이 업데이트함.</span><span class="sxs-lookup"><span data-stu-id="19d40-673">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="19d40-674">관리 그룹 수준에서 -Scope 값 리스팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-674">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="19d40-675">관리 그룹 수준에서 -Scope 값을 사용하여 개별 할당값을 검색하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-675">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="19d40-676">제어 매개 변수에 -Effective 및 -All 스위치 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-676">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="19d40-677">Get/New/Remove/Set-AzureRmPolicyDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-677">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="19d40-678">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-678">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="19d40-679">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-679">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="19d40-680">Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-680">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="19d40-681">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-681">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="19d40-682">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-682">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="19d40-683">'New-AzureRmResourceGroupDeployment'에서 'TemplateParameterObject'를 사용하는 경우 매개 변수에 KeyVault 비밀 참조 지원 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-683">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="19d40-684">'New-AzureRmADAppCredential'에 대해 '-EndDate' 매개 변수가 무시되는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-684">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="19d40-685">'Add-AzureRmADGroupMember'가 요청에 잘못된 URL을 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-685">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="19d40-686">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="19d40-686">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="19d40-687">선택적 매개 변수 -KeyValue를 New-AzureRmServiceBusKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-687">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="19d40-688">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="19d40-688">AzureRM.Sql</span></span>
* <span data-ttu-id="19d40-689">New-AzureRmSqlDatabaseRestorePoint 도움말에서 SQLDW에 대한 사용자 정의 복원 지점 명시</span><span class="sxs-lookup"><span data-stu-id="19d40-689">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="19d40-690">몇 가지 cmdlet에서-ComputeGeneration 매개 변수의 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-690">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="19d40-691">6.3.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="19d40-691">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="19d40-692">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="19d40-692">AzureRM.Profile</span></span>
* <span data-ttu-id="19d40-693">Enable-AzureRmContextAutoSave에 대한 오류 메시지 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-693">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="19d40-694">이전 컨텍스트 없이 'Connect-AzureRmAccount' 실행 시 각 구독에 대한 컨텍스트 생성</span><span class="sxs-lookup"><span data-stu-id="19d40-694">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="19d40-695">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="19d40-695">Azure.Storage</span></span>
* <span data-ttu-id="19d40-696">도움말 파일 내 -Permissions 매개 변수에 대한 추가 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-696">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="19d40-697">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="19d40-697">AzureRM.Compute</span></span>
* <span data-ttu-id="19d40-698">'Get-AzureRmVmDiskEncryptionStatus'가 데이터 디스크가 없는 VM에 대해 관찰된 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-698">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="19d40-699">Compute 클라이언트 라이브러리 버전을 업데이트하여 다음 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-699">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="19d40-700">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="19d40-700">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="19d40-701">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="19d40-701">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="19d40-702">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="19d40-702">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="19d40-703">다음 cmdlet이 '작업 ID' 및 '작업 상태'를 올바르게 표시하도록 수정:</span><span class="sxs-lookup"><span data-stu-id="19d40-703">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="19d40-704">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="19d40-704">Start-AzureRmVM</span></span>
    - <span data-ttu-id="19d40-705">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="19d40-705">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="19d40-706">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="19d40-706">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="19d40-707">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="19d40-707">Set-AzureRmVM</span></span>
    - <span data-ttu-id="19d40-708">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="19d40-708">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="19d40-709">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="19d40-709">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="19d40-710">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="19d40-710">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="19d40-711">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="19d40-711">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="19d40-712">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="19d40-712">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="19d40-713">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="19d40-713">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="19d40-714">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="19d40-714">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="19d40-715">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="19d40-715">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="19d40-716">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="19d40-716">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="19d40-717">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="19d40-717">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="19d40-718">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="19d40-718">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="19d40-719">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="19d40-719">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="19d40-720">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="19d40-720">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="19d40-721">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="19d40-721">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="19d40-722">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="19d40-722">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="19d40-723">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="19d40-723">AzureRM.EventGrid</span></span>
* <span data-ttu-id="19d40-724">Update-AzureRmEventGridSubscription cmdlet의 SubjectBeginsWith/SubjectEndsWith에 대한 ValidateNotNullOrEmpty 유효성 검사 조건을 제거하여 필요에 따라 이러한 매개 변수를 빈 문자열로 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-724">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="19d40-725">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="19d40-725">AzureRM.KeyVault</span></span>
* <span data-ttu-id="19d40-726">Get-AzureRmKeyVault -Tag 실행 시 태그가 리턴되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-726">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="19d40-727">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="19d40-727">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="19d40-728">Policy Insights cmdlet의 공개 릴리스</span><span class="sxs-lookup"><span data-stu-id="19d40-728">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="19d40-729">API 버전 2018-04-04 사용</span><span class="sxs-lookup"><span data-stu-id="19d40-729">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="19d40-730">PolicyDefinitionReferenceId를 Get-AzureRmPolicyStateSummary의 결과 집합에 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-730">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="19d40-731">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="19d40-731">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="19d40-732">-Vault 매개 변수를 RecoveryServices.Backup cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="19d40-732">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="19d40-733">전달되는 경우 이는 Set-AzureRmRecoveryServicesContext cmdlet을 재정의함.</span><span class="sxs-lookup"><span data-stu-id="19d40-733">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="19d40-734">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="19d40-734">AzureRM.Sql</span></span>
* <span data-ttu-id="19d40-735">Get-AzureRmSqlDatabaseExpanded에 대한 도움말 파일의 예가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-735">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="19d40-736">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="19d40-736">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="19d40-737">Add-AzureRmTrafficManagerEndpointConfig에대한 도움말 파일이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-737">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="19d40-738">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="19d40-738">AzureRM.Websites</span></span>
* <span data-ttu-id="19d40-739">-AssignIdentity를 사용할 때 AppSetting을 덮어쓰지 않도록 'Set-AzureRmWebApp'이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-739">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="19d40-740">'New-AzureRmWebAppSlot'이 AppServicePlan을 옵션 매개변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-740">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="19d40-741">6.2.1 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="19d40-741">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="19d40-742">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="19d40-742">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="19d40-743">PSWorkspace 모델이 Network 형식을 매개 변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="19d40-743">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="19d40-744">6.2.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="19d40-744">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="19d40-745">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="19d40-745">AzureRM.Profile</span></span>
* <span data-ttu-id="19d40-746">Newtonsoft.Json의 버전 10.0.3이 모듈 가져오기에 로드되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-746">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="19d40-747">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="19d40-747">AzureRM.Compute</span></span>
* <span data-ttu-id="19d40-748">VMSS VM 업데이트 기능</span><span class="sxs-lookup"><span data-stu-id="19d40-748">VMSS VM Update feature</span></span>
    - <span data-ttu-id="19d40-749">'Update-AzureRmVmssVM' 및 'New-AzureRmVMDataDisk' cmdlets 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-749">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="19d40-750">데이터 디스크를 Vmss VM에 추가할 수 있도록 지원하기 위해 VirtualMachineScaleSetVM 매개변수를 'Add-AzureRmVMDataDisk' cmdlet에 추가하였습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-750">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="19d40-751">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="19d40-751">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="19d40-752">ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.8.0-preview로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-752">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="19d40-753">팩터리 리포지토리 작업 구성 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-753">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="19d40-754">QuickBooks LinkedService가 ConsumerKey 및 consumerSecret 속성을 노출하도록 업데이트됨 </span><span class="sxs-lookup"><span data-stu-id="19d40-754">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="19d40-755">여러 모델 유형을 SecretBase에서 개체로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="19d40-755">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="19d40-756">Blob 이벤트 트리거 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-756">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="19d40-757">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="19d40-757">AzureRM.KeyVault</span></span>
* <span data-ttu-id="19d40-758">예제 출력으로 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-758">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="19d40-759">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="19d40-759">AzureRM.Network</span></span>
* <span data-ttu-id="19d40-760">Network Watcher cmdlet에서 트래픽 분석 매개 변수를 사용가능하도록 설정</span><span class="sxs-lookup"><span data-stu-id="19d40-760">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="19d40-761">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="19d40-761">AzureRM.Resources</span></span>
* <span data-ttu-id="19d40-762">'Get AzureRmResource'에서 반환된 'PSResource' 개체의 'Properties' 속성의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-762">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="19d40-763">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="19d40-763">AzureRM.Scheduler</span></span>
* <span data-ttu-id="19d40-764">ServiceBusQueueJob 업데이트가 새 인증 값을 설정하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="19d40-764">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="19d40-765">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="19d40-765">AzureRM.Sql</span></span>
* <span data-ttu-id="19d40-766">옵션 LicenseType 매개 변수를 사용하여 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="19d40-766">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="19d40-767">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="19d40-767">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="19d40-768">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="19d40-768">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="19d40-769">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="19d40-769">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="19d40-770">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="19d40-770">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="19d40-771">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="19d40-771">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="19d40-772">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="19d40-772">AzureRM.Websites</span></span>
* <span data-ttu-id="19d40-773">'New-AzureRMWebApp'이 전략 라이브러리의 공통 알고리즘을 사용하도록 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-773">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="19d40-774">6.1.0 - 2018년 5월</span><span class="sxs-lookup"><span data-stu-id="19d40-774">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="19d40-775">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="19d40-775">AzureRM.Profile</span></span>
* <span data-ttu-id="19d40-776">'Clear-AzureRmContext'를 실행하면 이전 기본 컨텍스트의 이름으로 빈 컨텍스트가 유지되어 사용자가 이전 이름으로 새 컨텍스트를 만들지 못하게 되는 문제를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-776">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="19d40-777">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="19d40-777">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="19d40-778">AS에서 게이트웨이가 작업을 연결하거나 연결 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-778">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="19d40-779">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="19d40-779">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="19d40-780">ApiVersions, ApiReleases 및 ApiRevisions에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-780">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="19d40-781">ServiceFabric 백 엔드에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-781">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="19d40-782">Application Insights 로거에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-782">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="19d40-783">'기본' SKU를 API Management 서비스의 유효한 SKU로 인식하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-783">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="19d40-784">개인 CA가 발급한 인증서를 루트 또는 CA로 설치하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-784">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="19d40-785">KeyVault 및 다중 프록시 호스트 이름을 통한 사용자 정의 SSL 인증서를 수락하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-785">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="19d40-786">MSI ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="19d40-786">Added support for MSI identity</span></span>
* <span data-ttu-id="19d40-787">URL을 통한 정책을 수락하는 지원 추가됨 참고: 다음 cmdlet은 이후 릴리스에서 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-787">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="19d40-788">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="19d40-788">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="19d40-789">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="19d40-789">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="19d40-790">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="19d40-790">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="19d40-791">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="19d40-791">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="19d40-792">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="19d40-792">AzureRM.Batch</span></span>
* <span data-ttu-id="19d40-793">새 cmdlet Get AzureBatchPoolNodeCounts 릴리스</span><span class="sxs-lookup"><span data-stu-id="19d40-793">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="19d40-794">새 cmdlet Start-AzureBatchComputeNodeServiceLogUpload 릴리스</span><span class="sxs-lookup"><span data-stu-id="19d40-794">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="19d40-795">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="19d40-795">AzureRM.Consumption</span></span>
* <span data-ttu-id="19d40-796">Expand, ResourceGroup, InstanceName, InstanceId, Tags, Top on Cmdlet Get-AzureRmConsumptionUsageDetail 등 새 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="19d40-796">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="19d40-797">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="19d40-797">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="19d40-798">Export-AzureRmDataLakeStoreChildItemProperties에 대한 예제 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-798">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="19d40-799">Set-AzureRmDataLakeStoreItemAclEntry에서 재귀 사례에 대한 null 매개 변수 예외 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-799">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="19d40-800">Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry에 대한 도움말 파일 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-800">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="19d40-801">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="19d40-801">AzureRM.Network</span></span>
* <span data-ttu-id="19d40-802">18.0.0-preview에서 19.0.0-preview로 네트워크 SDK 버전 업그레이드</span><span class="sxs-lookup"><span data-stu-id="19d40-802">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="19d40-803">프로토콜 구성을 만들기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="19d40-803">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="19d40-804">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="19d40-804">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="19d40-805">기존 Express 경로 회로에 새 회로 연결을 추가하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="19d40-805">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="19d40-806">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-806">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="19d40-807">기존 Express 경로 회로에서 회로 연결을 제거하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="19d40-807">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="19d40-808">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-808">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="19d40-809">회로 연결을 검색하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="19d40-809">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="19d40-810">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="19d40-810">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="19d40-811">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="19d40-811">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="19d40-812">생성된 인증서로 고정 서버 인증 사용(문제 # 5998)</span><span class="sxs-lookup"><span data-stu-id="19d40-812">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="19d40-813">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="19d40-813">AzureRM.Sql</span></span>
* <span data-ttu-id="19d40-814">AuditActions 또는 AuditActionGroups를 제거할 수 있도록 업데이트된 감사 cmdlet</span><span class="sxs-lookup"><span data-stu-id="19d40-814">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="19d40-815">'Azure 복구 서비스 자격 증명 모음을 사용하여 장기 보존 정책을 구성하면 정책이 더 이상 지원되지 않습니다. 새로운 유연 보유 정책으로 요청을 제출하십시오.'라는 메시지와 함께 명령이 실패하는 새로운 유연 보유 정책을 설정할 때</span><span class="sxs-lookup"><span data-stu-id="19d40-815">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="19d40-816">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy의 문제 수정</span><span class="sxs-lookup"><span data-stu-id="19d40-816">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="19d40-817">Azure SQL Database/ElasticPool Creation/Update 관련 cmdlet을 모두 업데이트하여 규모 및 계층 관련 속성에 대한 SKU 속성을 지원하는 새 데이터베이스 API를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-817">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="19d40-818">업데이트된 cmdlet는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-818">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="19d40-819">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="19d40-819">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="19d40-820">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="19d40-820">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="19d40-821">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="19d40-821">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="19d40-822">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="19d40-822">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="19d40-823">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="19d40-823">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="19d40-824">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="19d40-824">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="19d40-825">-Name 매개 변수를 사용할 때 -ResourceGroupName 매개 변수가 필요하도록 'Get-AzureRmTrafficManagerProfile'에 대한 매개 변수를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="19d40-825">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
