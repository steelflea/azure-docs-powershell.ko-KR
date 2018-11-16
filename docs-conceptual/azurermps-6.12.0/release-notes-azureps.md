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
ms.openlocfilehash: 8a7b184ed06eb078956229fa67d02840014e3aaf
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/15/2018
ms.locfileid: "51574535"
---
# <a name="release-notes"></a><span data-ttu-id="fd052-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="fd052-103">Release notes</span></span>

<span data-ttu-id="fd052-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6120---november-2018"></a><span data-ttu-id="fd052-105">6.12.0 - 2018년 11월</span><span class="sxs-lookup"><span data-stu-id="fd052-105">6.12.0 - November 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="fd052-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fd052-106">AzureRM.Profile</span></span>
* <span data-ttu-id="fd052-107">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-107">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="fd052-108">Connect-AzureRmAccount cmdlet의 매개 변수 TenantId 이름을 Tenant로 바꾸고 TenantId의 별칭을 추가합니다</span><span class="sxs-lookup"><span data-stu-id="fd052-108">Rename param TenantId in cmdlet Connect-AzureRmAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="fd052-109">Connect-AzureRmAccount의 업데이트된 TenantId 설명</span><span class="sxs-lookup"><span data-stu-id="fd052-109">Updated TenantId description for Connect-AzureRmAccount</span></span>
* <span data-ttu-id="fd052-110">테넌트 도메인을 제공할 때 실패한 로그인에 대한 오류 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-110">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="fd052-111">테넌트에 구독이 없는 계정의 컨텍스트 이름 충돌 문제 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-111">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="fd052-112">MSI를 사용할 때 DataLake 엔드포인트 문제 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-112">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="fd052-113">연결되지 않은 경우 'Disconnect-AzureRmAccount'가 throw하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-113">Fix issue where 'Disconnect-AzureRmAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azurermautomation"></a><span data-ttu-id="fd052-114">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="fd052-114">AzureRM.Automation</span></span>
* <span data-ttu-id="fd052-115">cmdlet DLL 파일 이름이 Microsoft.Azure.Commands.Automation.dll로 변경됨</span><span class="sxs-lookup"><span data-stu-id="fd052-115">Renamed cmdlet DLL filename to Microsoft.Azure.Commands.Automation.dll</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="fd052-116">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="fd052-116">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="fd052-117">Get-AzureRmCognitiveServicesAccountSkus 작업을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-117">Add Get-AzureRmCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fd052-118">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fd052-118">AzureRM.Compute</span></span>
* <span data-ttu-id="fd052-119">Add-AzureRmVmssVMDataDisk 및 Remove-AzureRmVmssVMDataDisk cmdlet를 추가합니다</span><span class="sxs-lookup"><span data-stu-id="fd052-119">Add Add-AzureRmVmssVMDataDisk and Remove-AzureRmVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="fd052-120">Get-AzureRmVMImage는 AutomaticOSUpgradeProperties를 표시합니다</span><span class="sxs-lookup"><span data-stu-id="fd052-120">Get-AzureRmVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="fd052-121">수정된 SetAzureRmVMChefExtension -BootstrapOptions 및 -JsonAttribute option 값이 json 형식으로 설정하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-121">Fixed SetAzureRmVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="fd052-122">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="fd052-122">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="fd052-123">DataLake 패키지를 1.1.10으로 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-123">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="fd052-124">기본 동시성을 다중 스레드 작업에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-124">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="fd052-125">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="fd052-125">AzureRM.Insights</span></span>
* <span data-ttu-id="fd052-126">해결된 문제 #7267(자동 크기 조정 영역)</span><span class="sxs-lookup"><span data-stu-id="fd052-126">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="fd052-127">열거된 매개 변수를 제대로 설정하지 않은 새 자동 크기 조정 규칙을 만드는 데 문제가 있습니다(이를 항상 기본값으로 설정함).</span><span class="sxs-lookup"><span data-stu-id="fd052-127">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="fd052-128">해결된 문제 # 7513[자세한 정보] Set-AzureRMDiagnosticSetting은 설정을 생성하는 동안 범주를 명시적으로 지정해야 합니다</span><span class="sxs-lookup"><span data-stu-id="fd052-128">Fixed issue #7513 [Insights] Set-AzureRMDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="fd052-129">이제 cmdlet은 생성 중에 사용할 범주를 명시적으로 표시할 필요가 없습니다. 즉, 문서화된대로 작동합니다</span><span class="sxs-lookup"><span data-stu-id="fd052-129">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="fd052-130">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fd052-130">AzureRM.Network</span></span>
* <span data-ttu-id="fd052-131">다음 cmdlet에 대해 PeeringType을 필수 매개 변수로 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-131">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="fd052-132">Get-AzureRmExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="fd052-132">Get-AzureRmExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="fd052-133">Get-AzureRmExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="fd052-133">Get-AzureRmExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="fd052-134">Get-AzureRmExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="fd052-134">Get-AzureRmExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="fd052-135">Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="fd052-135">Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="fd052-136">Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="fd052-136">Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="fd052-137">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="fd052-137">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="fd052-138">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="fd052-138">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="fd052-139">추가된 정책 재구성 cmdlet</span><span class="sxs-lookup"><span data-stu-id="fd052-139">Added policy remediation cmdlets</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="fd052-140">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="fd052-140">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="fd052-141">복구 서비스에 Azure 파일 공유 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="fd052-141">Added support for azure file shares in recovery services.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fd052-142">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fd052-142">AzureRM.Resources</span></span>
* <span data-ttu-id="fd052-143">https://github.com/Azure/azure-powershell/issues/7402에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-143">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="fd052-144">'Get-AzureRmResource'에 대해 '-ResourceId' 매개 변수를 사용하여 리소스 나열 허용</span><span class="sxs-lookup"><span data-stu-id="fd052-144">Allow listing resources using the '-ResourceId' parameter for 'Get-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="fd052-145">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fd052-145">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="fd052-146">마이그레이션 상태를 알 수 있도록 PSServiceBusMigrationConfigurationAttributes에 MigrationState 읽기 전용 속성 추가.</span><span class="sxs-lookup"><span data-stu-id="fd052-146">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="fd052-147">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="fd052-147">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="fd052-148">Linux Vmss에 인증서 추가 수정.</span><span class="sxs-lookup"><span data-stu-id="fd052-148">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="fd052-149">'Add-AzureRmServiceFabricClusterCertificate' 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-149">Fix 'Add-AzureRmServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="fd052-150">새 인증서(Azure/service-fabric-issues#932)에서 올바른 지문을 사용.</span><span class="sxs-lookup"><span data-stu-id="fd052-150">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="fd052-151">올바르게 예외 표시(Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="fd052-151">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="fd052-152">Vmss CreateOrUpdate 작업을 시작하기 전에 'Update-AzureRmServiceFabricDurability'를 수정하여 클러스터 구성 업데이트.</span><span class="sxs-lookup"><span data-stu-id="fd052-152">Fix 'Update-AzureRmServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="6110---october-2018"></a><span data-ttu-id="fd052-153">6.11.0 - 2018년 10월</span><span class="sxs-lookup"><span data-stu-id="fd052-153">6.11.0 - October 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="fd052-154">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fd052-154">AzureRM.Profile</span></span>
* <span data-ttu-id="fd052-155">CloudShell에서 Get-AzureRmSubscription을 사용하여 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-155">Fix issue with Get-AzureRmSubscription in CloudShell</span></span>
* <span data-ttu-id="fd052-156">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-156">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="fd052-157">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="fd052-157">AzureRM.Backup</span></span>
* <span data-ttu-id="fd052-158">Azure Backup cmdlet이 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-158">Deprecated Azure Backup cmdlets.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fd052-159">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fd052-159">AzureRM.Compute</span></span>
* <span data-ttu-id="fd052-160">'New-AzureRmVm'에 대해 간단한 매개 변수를 사용하는 경우 가속화된 네트워킹을 설정하기 위해 새 크기가 VM 크기의 허용 목록에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-160">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzureRmVm'</span></span>
* <span data-ttu-id="fd052-161">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-161">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="fd052-162">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="fd052-162">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="fd052-163">Virtual Network 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-163">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="fd052-164">Get-AzureRmDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 가져오거나 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-164">Get-AzureRmDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="fd052-165">Add-AzureRmDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 가상 네트워크 규칙을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-165">Add-AzureRmDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="fd052-166">Set-AzureRmDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에서 지정된 가상 네트워크 규칙을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-166">Set-AzureRmDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="fd052-167">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-167">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="fd052-168">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fd052-168">AzureRM.Network</span></span>
* <span data-ttu-id="fd052-169">Test-AzureRmNetworkWatcherConnectivity cmdlet을 업데이트하고, 백 엔드에 프로토콜 값을 전달합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-169">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="fd052-170">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-170">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fd052-171">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fd052-171">AzureRM.Resources</span></span>
* <span data-ttu-id="fd052-172">(기본 프로필에 구독이 없고 범위가 지정되지 않은 경우) 시나리오에서 의미 있는 예외를 추가하여 Get-AzureRMRoleDefinition이 인식할 수 없는 예외를 throw하는 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-172">Fix isssue where Get-AzureRMRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="fd052-173">또한 기본 매개 변수 집합을 'RoleDefinitionNameParameterSet'으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-173">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="6100---october-2018"></a><span data-ttu-id="fd052-174">2018년 10월 - 6.10.0</span><span class="sxs-lookup"><span data-stu-id="fd052-174">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="fd052-175">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="fd052-175">Azure.Storage</span></span>
* <span data-ttu-id="fd052-176">대상에 메타데이터가 있을 때 Blob/파일이 메타 데이터를 복사하지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-176">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="fd052-177">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="fd052-177">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="fd052-178">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="fd052-178">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="fd052-179">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="fd052-179">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="fd052-180">기존 계정이 없는 Get-AzureRmCognitiveServicesAccountSkus를 지원</span><span class="sxs-lookup"><span data-stu-id="fd052-180">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fd052-181">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fd052-181">AzureRM.Compute</span></span>
* <span data-ttu-id="fd052-182">Get-AzureRmVM -ResourceGroupName <rg>가 필요한 경우 50개가 넘는 결과를 반환하도록 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-182">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="fd052-183">'SimpleParameterSet' 예제가 New-AzureRmVmss cmdlet 도움말에 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-183">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="fd052-184">Azure Disk Encryption 진행률 메시지의 오타를 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-184">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="fd052-185">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="fd052-185">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="fd052-186">ADF.Net SDK 버전을 2.3.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-186">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="fd052-187">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fd052-187">AzureRM.Network</span></span>
* <span data-ttu-id="fd052-188">NetworkProfile 기능 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-188">Added NetworkProfile functionality.</span></span> <span data-ttu-id="fd052-189">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-189">new cmdlets added</span></span>
    - <span data-ttu-id="fd052-190">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="fd052-190">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="fd052-191">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="fd052-191">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="fd052-192">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="fd052-192">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="fd052-193">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="fd052-193">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="fd052-194">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-194">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="fd052-195">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-195">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="fd052-196">서브넷 모델에 서비스 연결 링크 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-196">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="fd052-197">New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-197">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="fd052-198">Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-198">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="fd052-199">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="fd052-199">AzureRM.RedisCache</span></span>
* <span data-ttu-id="fd052-200">모든 문자열을 Size 매개 변수로 진행되도록 허용</span><span class="sxs-lookup"><span data-stu-id="fd052-200">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="fd052-201">PSArgumentCompleter 팝업에 P5 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-201">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fd052-202">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fd052-202">AzureRM.Resources</span></span>
* <span data-ttu-id="fd052-203">-Mode 매개 변수를 Set-AzureRmPolicyDefinition에 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-203">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="fd052-204">사용자가 포함된 Origin 작업에서 Get-AzureRmProviderOperation commandlet 버그 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-204">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="fd052-205">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fd052-205">AzureRM.Sql</span></span>
* <span data-ttu-id="fd052-206">일부 백업 cmdlet이 현재 azure 구독을 인식하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-206">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="fd052-207">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="fd052-207">AzureRM.Storage</span></span>
* <span data-ttu-id="fd052-208">특정 위치의 저장소 리소스 사용을 지원하고 글로벌 저장소 리소스 사용 가져오기는 더 이상 사용되지 않는다는 경고 메시지를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-208">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="fd052-209">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="fd052-209">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="fd052-210">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="fd052-210">AzureRM.Websites</span></span>
* <span data-ttu-id="fd052-211">새 cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - 컨테이너 지속적인 배포 Webhook URL을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-211">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="fd052-212">새 cmdlet 
New-AzureRMWebAppContainerPSSession 및 Enter-WebAppContainerPSSession -  windows 컨테이너 앱에 PowerShell 원격 세션을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-212">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="fd052-213">6.9.0 - 2018년 9월</span><span class="sxs-lookup"><span data-stu-id="fd052-213">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="fd052-214">일반</span><span class="sxs-lookup"><span data-stu-id="fd052-214">General</span></span>
* <span data-ttu-id="fd052-215">AzureRM.SignalR이 AzureRM 롤업 모듈에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-215">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="fd052-216">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fd052-216">AzureRM.Profile</span></span>
* <span data-ttu-id="fd052-217">저장소 일반 코드에 대한 약간의 변경</span><span class="sxs-lookup"><span data-stu-id="fd052-217">Minor changes to the storage common code</span></span>
* <span data-ttu-id="fd052-218">전체 매개 변수 형식을 포함하도록 도움말 파일이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-218">Updated help files to include full parameter types.</span></span>
* <span data-ttu-id="fd052-219">-ServicePrincipal을 필수가 아닌 것으로 ServicePrincipalCertificateWithSubscriptionId 매개변수 집합에서 변경</span><span class="sxs-lookup"><span data-stu-id="fd052-219">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="fd052-220">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="fd052-220">Azure.Storage</span></span>
* <span data-ttu-id="fd052-221">OAuth를 사용하여 저장소 컨텍스트를 만드는 것을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-221">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="fd052-222">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="fd052-222">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="fd052-223">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="fd052-223">AzureRM.Cdn</span></span>
* <span data-ttu-id="fd052-224">Cdn 가격 책정 sku에서 Standard_Microsoft를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-224">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="fd052-225">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fd052-225">AzureRM.Compute</span></span>
* <span data-ttu-id="fd052-226">Keyvault 및 Storage에서 종속성을 일반 종속성으로 이동</span><span class="sxs-lookup"><span data-stu-id="fd052-226">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="fd052-227">AEM cmdlet에 더 많은 가상 머신 크기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-227">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="fd052-228">PublicIPPrefix 매개 변수를 New-AzureRmVmssIpConfig에 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-228">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="fd052-229">Invoke-AzureRmVMRunCommand cmdelt에 ResourceId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-229">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="fd052-230">Invoke-AzureRmVmssVMRunCommand cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-230">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="fd052-231">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="fd052-231">AzureRM.Dns</span></span>
* <span data-ttu-id="fd052-232">Dns 레코드를 만드는 동안 별칭 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-232">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="fd052-233">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="fd052-233">AzureRM.Insights</span></span>
* <span data-ttu-id="fd052-234">#6833 및 #7102 문제 수정(진단 설정 영역)</span><span class="sxs-lookup"><span data-stu-id="fd052-234">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="fd052-235">기본 이름, 즉 'service'에 진단 설정의 목록 생성 및 가져오는 동안에 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-235">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="fd052-236">범주를 사용하는 진단 설정 만들기 문제</span><span class="sxs-lookup"><span data-stu-id="fd052-236">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="fd052-237">메트릭 시간 조직 매개 변수에 대한 사용 중단 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-237">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="fd052-238">Timegrains 매개 변수는 여전히 받아들여지고 있습니다(이것은 호환성이 손상되는 변경이 아닙니다). 그러나 PT1M만 유효하므로 백엔드에서 무시됩니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-238">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="fd052-239">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fd052-239">AzureRM.Network</span></span>
* <span data-ttu-id="fd052-240">LoadBalancer cmdlet에 대한 변경</span><span class="sxs-lookup"><span data-stu-id="fd052-240">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="fd052-241">LoadBalancerInboundNatPoolConfig: IdleTimeoutInMinutes, EnableFloatingIp 및 EnableTcpReset 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-241">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="fd052-242">LoadBalancerInboundNatRuleConfig: EnableTcpReset 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-242">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="fd052-243">LoadBalancerRuleConfig: EnableTcpReset 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-243">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="fd052-244">LoadBalancerProbeConfig: 매개 변수 프로토콜에 대해 "Https" 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-244">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="fd052-245">새 LoadBalancer의 하위 리소스OutboundRule에 대한 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-245">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="fd052-246">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-246">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="fd052-247">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-247">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="fd052-248">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-248">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="fd052-249">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-249">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="fd052-250">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-250">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="fd052-251">PSNetworkInterface에 대한 새 HostedWorkloads 속성 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-251">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="fd052-252">기능에 대한 새 cmdlet 추가: ARM을 통한 Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="fd052-252">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="fd052-253">Get-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-253">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="fd052-254">Set-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-254">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="fd052-255">New-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-255">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="fd052-256">Remove-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-256">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="fd052-257">New-AzureRmFirewallApplicationRuleCollection 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-257">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="fd052-258">New-AzureRmFirewallApplicationRule 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-258">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="fd052-259">New-AzureRmFirewallNatRuleCollection 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-259">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="fd052-260">New-AzureRmFirewallNatRule 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-260">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="fd052-261">New-AzureRmFirewallNetworkRuleCollection 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-261">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="fd052-262">New-AzureRmFirewallNetworkRule 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-262">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="fd052-263">Application Gateway에서 신뢰할 수 있는 루트 인증서 및 크기 자동 조정 구성에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-263">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="fd052-264">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-264">New Cmdlets added:</span></span>
      - <span data-ttu-id="fd052-265">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="fd052-265">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="fd052-266">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="fd052-266">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="fd052-267">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="fd052-267">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="fd052-268">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="fd052-268">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="fd052-269">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="fd052-269">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="fd052-270">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd052-270">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="fd052-271">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd052-271">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="fd052-272">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd052-272">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="fd052-273">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd052-273">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="fd052-274">옵션 매개 변수를 사용하도록 업데이트된 Cmdlet-TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="fd052-274">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="fd052-275">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="fd052-275">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="fd052-276">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="fd052-276">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="fd052-277">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="fd052-277">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="fd052-278">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="fd052-278">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="fd052-279">옵션 매개 변수를 사용하도록 업데이트된 Cmdlet-AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd052-279">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="fd052-280">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="fd052-280">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="fd052-281">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="fd052-281">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="fd052-282">인터페이스 엔드포인트 Get-AzureInterfaceEndpoint에 대한 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-282">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="fd052-283">서브넷에서 여러 주소 접두사에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-283">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="fd052-284">다음 Cmdlet이 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-284">Updated cmdlets:</span></span>
  - <span data-ttu-id="fd052-285">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-285">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="fd052-286">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-286">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="fd052-287">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-287">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="fd052-288">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-288">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="fd052-289">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="fd052-289">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="fd052-290">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-290">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="fd052-291">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-291">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="fd052-292">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-292">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="fd052-293">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd052-293">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="fd052-294">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd052-294">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="fd052-295">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd052-295">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="fd052-296">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-296">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="fd052-297">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-297">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="fd052-298">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-298">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="fd052-299">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-299">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="fd052-300">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-300">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="fd052-301">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-301">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="fd052-302">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-302">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="fd052-303">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="fd052-303">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="fd052-304">서브넷 위임에 대한 cmdlet을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-304">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="fd052-305">New-AzureRmDelegation: 서브넷에 추가할 수 있는 새 위임을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-305">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="fd052-306">Remove-AzureRmDelegation: 서브넷에서 가져와서 해당 서브넷에서 제공된 위임 이름을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-306">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="fd052-307">Add-AzureRmDelegation: 서브넷에서 사용 및 제공된 서비스 이름을 해당 서브넷에 대한 위임으로 추가합니다</span><span class="sxs-lookup"><span data-stu-id="fd052-307">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="fd052-308">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="fd052-308">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="fd052-309">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="fd052-309">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="fd052-310">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="fd052-310">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="fd052-311">관리되는 관리 디스크에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="fd052-311">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="fd052-312">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="fd052-312">AzureRM.RedisCache</span></span>
* <span data-ttu-id="fd052-313">인사이트 종속성이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-313">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fd052-314">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fd052-314">AzureRM.Resources</span></span>
* <span data-ttu-id="fd052-315">New-AzureRmResourceGroupDeployment를 RollbackAction 새 매개 변수를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-315">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="fd052-316">새 매개 변수를 사용하여 OnErrorDeployment에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-316">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="fd052-317">정책 할당에서 관리되는 ID를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-317">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="fd052-318">'New-AzureRmPolicyAssignment'를 사용하여 정책을 할당할 때 기본값이 있는 매개 변수는 더 이상 필요하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-318">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="fd052-319">정책 별칭을 검색하기 위한 새 cmdlet Get-AzureRmPolicyAlias 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-319">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="fd052-320">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fd052-320">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="fd052-321">#7161 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-321">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="fd052-322">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="fd052-322">AzureRM.SignalR</span></span>
* <span data-ttu-id="fd052-323">SKU 이름을 Free_F1 및 Standard_S1로 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-323">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="fd052-324">버전 필드를 PSSignalRResource 개체에 추가하고 연결 문자열을 PSSignalRKeys개체에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-324">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="fd052-325">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="fd052-325">AzureRM.Storage</span></span>
* <span data-ttu-id="fd052-326">AzureRm.Storage에서 불변성 정책 지원</span><span class="sxs-lookup"><span data-stu-id="fd052-326">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="fd052-327">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="fd052-327">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="fd052-328">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="fd052-328">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="fd052-329">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="fd052-329">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="fd052-330">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="fd052-330">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="fd052-331">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="fd052-331">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="fd052-332">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="fd052-332">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="fd052-333">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="fd052-333">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="fd052-334">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="fd052-334">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="fd052-335">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="fd052-335">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="fd052-336">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="fd052-336">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="fd052-337">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="fd052-337">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="fd052-338">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="fd052-338">AzureRM.Websites</span></span>
* <span data-ttu-id="fd052-339">두 개의 새로운 cmdlet 추가: Get-AzureRmDeletedWebApp 및 Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="fd052-339">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="fd052-340">New-AzureRmAppServicePlan -HyperV 스위치가 창 컨테이너가 있는 앱 서비스 계획 작성용으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-340">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="fd052-341">New-AzureRmWebApp/New-AzureRmWebAppSlot/Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - Windows 컨테이너 앱을 만들고 관리하기 위한 새 매개 변수(-ContainerRegistryUser 문자열 -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment)가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-341">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="fd052-342">6.8.1 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="fd052-342">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="fd052-343">일반</span><span class="sxs-lookup"><span data-stu-id="fd052-343">General</span></span>
* <span data-ttu-id="fd052-344">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-344">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="fd052-345">공용 런타임 어셈블리가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-345">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="fd052-346">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="fd052-346">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="fd052-347">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-347">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="fd052-348">문제 https://github.com/Azure/azure-powershell/issues/6603 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-348">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="fd052-349">Import-AzureRmApiManagementApi 및 \*-AzureRmApiManagementCertificate cmdlet은 이제 상대 경로를 처리합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-349">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="fd052-350">문제 https://github.com/Azure/azure-powershell/issues/6879 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-350">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="fd052-351">CertificateInformation은 Set-AzureRmApiManagement cmdlet이 제대로 작동 하게 하는 설정 가능한 속성입니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-351">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="fd052-352">4.0.4-preview nuget으로 업그레이드하여 해결됨</span><span class="sxs-lookup"><span data-stu-id="fd052-352">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="fd052-353">문제 https://github.com/Azure/azure-powershell/issues/6853 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-353">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="fd052-354">제품에서 이름별 검색에 대해 Odata 필터가 수정됨</span><span class="sxs-lookup"><span data-stu-id="fd052-354">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="fd052-355">문제 https://github.com/Azure/azure-powershell/issues/6814 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-355">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="fd052-356">API에서 이름별 검색에 대해 Odata 필터가 수정됨</span><span class="sxs-lookup"><span data-stu-id="fd052-356">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="fd052-357">AzureMonitor 로거에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-357">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="fd052-358">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fd052-358">AzureRM.Compute</span></span>
* <span data-ttu-id="fd052-359">오류 출력에 대상이 없는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-359">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="fd052-360">관리 디스크를 사용하는 VM에 대한 저장소 계정 유형 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-360">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="fd052-361">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-361">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="fd052-362">예를 들어 Azure 중국과 같이, 다른 환경에 대한 AEM 확장 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-362">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="fd052-363">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fd052-363">AzureRM.Network</span></span>
* <span data-ttu-id="fd052-364">기본 cmdlet 출력 표시를 테이블 뷰로 변경</span><span class="sxs-lookup"><span data-stu-id="fd052-364">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="fd052-365">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="fd052-365">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="fd052-366">일시 중지된 용량을 확장하려고 할 때 Update-AzureRmPowerBIEmbeddedCapacity 실패 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-366">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="fd052-367">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fd052-367">AzureRM.Resources</span></span>
* <span data-ttu-id="fd052-368">MarketPlace에서 관리되는 응용 프로그램 생성 시의 문제 해결.</span><span class="sxs-lookup"><span data-stu-id="fd052-368">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="fd052-369">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fd052-369">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="fd052-370">해결된 문제</span><span class="sxs-lookup"><span data-stu-id="fd052-370">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="fd052-371">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="fd052-371">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="fd052-372">다중값 라우팅 메서드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-372">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="fd052-373">다중값 라우팅에 대한 새 매개 변수 'MaxReturn'</span><span class="sxs-lookup"><span data-stu-id="fd052-373">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="fd052-374">서브넷 라우팅 메서드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-374">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="fd052-375">엔드포인트의 IP 주소 범위(서브넷)에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="fd052-375">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="fd052-376">프로필 내 사용자 지정 헤더에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-376">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="fd052-377">프로필 내 예상 상태 코드 범위에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-377">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="fd052-378">엔드포인트 내 사용자 지정 헤더에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-378">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="fd052-379">6.8.0 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="fd052-379">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="fd052-380">일반</span><span class="sxs-lookup"><span data-stu-id="fd052-380">General</span></span>
* <span data-ttu-id="fd052-381">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-381">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="fd052-382">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fd052-382">AzureRM.Profile</span></span>
* <span data-ttu-id="fd052-383">Connect-AzureRmAccount 중에 반환된 토큰에 만료 속성 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-383">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fd052-384">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fd052-384">AzureRM.Compute</span></span>
* <span data-ttu-id="fd052-385">오류 출력에 대상이 없는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-385">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="fd052-386">관리 디스크를 사용하는 VM에 대한 저장소 계정 유형 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-386">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="fd052-387">예를 들어 Azure 중국과 같이, 다른 환경에 대한 AEM 확장 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-387">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="fd052-388">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="fd052-388">AzureRM.IotHub</span></span>
* <span data-ttu-id="fd052-389">New-AzureRmIotHubExportDevices 및 New-AzureRmIotHubImportDevices에 대한 예제를 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-389">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="fd052-390">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fd052-390">AzureRM.Network</span></span>
* <span data-ttu-id="fd052-391">기본 모델 표시를 테이블 뷰로 변경</span><span class="sxs-lookup"><span data-stu-id="fd052-391">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="fd052-392">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="fd052-392">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="fd052-393">일시 중지된 용량을 확장하려고 할 때 Update-AzureRmPowerBIEmbeddedCapacity 실패 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-393">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fd052-394">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fd052-394">AzureRM.Resources</span></span>
* <span data-ttu-id="fd052-395">MarketPlace에서 관리되는 응용 프로그램 생성 시의 문제 해결.</span><span class="sxs-lookup"><span data-stu-id="fd052-395">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="fd052-396">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fd052-396">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="fd052-397">문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-397">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="fd052-398">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="fd052-398">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="fd052-399">다중값 라우팅 메서드에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="fd052-399">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="fd052-400">다중값 라우팅에 대한 새 매개 변수 'MaxReturn'</span><span class="sxs-lookup"><span data-stu-id="fd052-400">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="fd052-401">서브넷 라우팅 메서드에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="fd052-401">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="fd052-402">엔드포인트의 IP 주소 범위(서브넷)에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="fd052-402">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="fd052-403">프로필 내 사용자 지정 헤더에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="fd052-403">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="fd052-404">프로필 내 예상 상태 코드 범위에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="fd052-404">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="fd052-405">엔드포인트 내 사용자 지정 헤더에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="fd052-405">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="fd052-406">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="fd052-406">AzureRM.Websites</span></span>
* <span data-ttu-id="fd052-407">기본 리소스 그룹이 잘못 설정되는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-407">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="fd052-408">6.7.0 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="fd052-408">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="fd052-409">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fd052-409">AzureRM.Profile</span></span>
* <span data-ttu-id="fd052-410">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-410">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="fd052-411">충돌을 방지하려면 기본 컨텍스트 이름으로 사용자 ID를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-411">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="fd052-412">#6398 컨텍스트를 선택할 때 문제를 발생시킨 Clear-AzureRmContext 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-412">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="fd052-413">'Connect-AzureRmAccount'에 대한 '-TenantId' 매개 변수에 전달할 테넌트 도메인을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="fd052-413">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="fd052-414">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="fd052-414">Azure.Storage</span></span>
* <span data-ttu-id="fd052-415">Azure 파일 공유 할당량에 대한 5TB 제한 제거</span><span class="sxs-lookup"><span data-stu-id="fd052-415">Remove the 5TB limitation for Azure File Share quota</span></span>
* <span data-ttu-id="fd052-416">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="fd052-416">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="fd052-417">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="fd052-417">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="fd052-418">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-418">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="fd052-419">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="fd052-419">Azure.AnalysisServices</span></span>
* <span data-ttu-id="fd052-420">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-420">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="fd052-421">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="fd052-421">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="fd052-422">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-422">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="fd052-423">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="fd052-423">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="fd052-424">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-424">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="fd052-425">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="fd052-425">AzureRM.Automation</span></span>
* <span data-ttu-id="fd052-426">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-426">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="fd052-427">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="fd052-427">AzureRM.Backup</span></span>
* <span data-ttu-id="fd052-428">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-428">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="fd052-429">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="fd052-429">AzureRM.Batch</span></span>
* <span data-ttu-id="fd052-430">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-430">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="fd052-431">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="fd052-431">AzureRM.Billing</span></span>
* <span data-ttu-id="fd052-432">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-432">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="fd052-433">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="fd052-433">AzureRM.Cdn</span></span>
* <span data-ttu-id="fd052-434">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-434">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="fd052-435">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="fd052-435">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="fd052-436">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-436">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fd052-437">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fd052-437">AzureRM.Compute</span></span>
* <span data-ttu-id="fd052-438">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-438">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="fd052-439">New-AzureRmVmssConfig에 EvictionPolicy 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-439">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="fd052-440">지정된 위치가 없는 경우에 New-AzureRmVm의 DiskFileParameterSet 내의 기본 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-440">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="fd052-441">Save-AzureRmVMImage에서 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-441">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="fd052-442">특정 singlepass 관련 시나리오에 대해 Get-AzureRmVMDiskEncryptionStatus cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-442">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="fd052-443">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="fd052-443">AzureRM.Consumption</span></span>
* <span data-ttu-id="fd052-444">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-444">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="fd052-445">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="fd052-445">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="fd052-446">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-446">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="fd052-447">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="fd052-447">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="fd052-448">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-448">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="fd052-449">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="fd052-449">AzureRM.DataFactories</span></span>
* <span data-ttu-id="fd052-450">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-450">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="fd052-451">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="fd052-451">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="fd052-452">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-452">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="fd052-453">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="fd052-453">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="fd052-454">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-454">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="fd052-455">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="fd052-455">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="fd052-456">DebugPreference가 powershell 명령줄에서 설정된 경우 디버깅 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-456">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="fd052-457">Set-AzureRmDataLakeStoreItemAcl에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-457">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="fd052-458">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-458">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="fd052-459">Set-AzureRmDataLakeStoreItemAclEntry에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-459">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="fd052-460">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="fd052-460">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="fd052-461">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-461">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="fd052-462">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="fd052-462">AzureRM.Dns</span></span>
* <span data-ttu-id="fd052-463">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-463">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="fd052-464">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="fd052-464">AzureRM.EventGrid</span></span>
* <span data-ttu-id="fd052-465">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-465">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="fd052-466">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="fd052-466">AzureRM.EventHub</span></span>
* <span data-ttu-id="fd052-467">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-467">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="fd052-468">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="fd052-468">AzureRM.HDInsight</span></span>
* <span data-ttu-id="fd052-469">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-469">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="fd052-470">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="fd052-470">AzureRM.Insights</span></span>
* <span data-ttu-id="fd052-471">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-471">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="fd052-472">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="fd052-472">AzureRM.IotHub</span></span>
* <span data-ttu-id="fd052-473">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-473">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="fd052-474">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="fd052-474">AzureRM.KeyVault</span></span>
* <span data-ttu-id="fd052-475">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-475">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="fd052-476">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="fd052-476">AzureRM.LogicApp</span></span>
* <span data-ttu-id="fd052-477">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-477">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="fd052-478">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="fd052-478">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="fd052-479">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-479">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="fd052-480">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="fd052-480">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="fd052-481">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-481">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="fd052-482">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="fd052-482">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="fd052-483">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-483">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="fd052-484">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="fd052-484">AzureRM.Media</span></span>
* <span data-ttu-id="fd052-485">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-485">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="fd052-486">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fd052-486">AzureRM.Network</span></span>
* <span data-ttu-id="fd052-487">Set-AzureRmLocalNetworkGateway에 대한 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-487">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="fd052-488">Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey, New-AzureRmVirtualNetworkGatewayConnection에 대한 예제 및 설명 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-488">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="fd052-489">Remove-AzureRmVirtualNetworkGatewayIpConfig 및 Reset-AzureRmVirtualNetworkGateway에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-489">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="fd052-490">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-490">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="fd052-491">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-491">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="fd052-492">Set-AzureRmVirtualNetworkGatewayConnection에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-492">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="fd052-493">최신 코드 생성기를 사용하여 ApplicationSecurityGroup, RouteTable 및 Usage에 대한 cmdlet을 다시 생성함</span><span class="sxs-lookup"><span data-stu-id="fd052-493">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="fd052-494">Exitc 하지 않는 서브넷을 얻으려고 할 때의 Get-AzureRmVirtualNetworkSubnetConfig에 대한 오류 메시지를 설명</span><span class="sxs-lookup"><span data-stu-id="fd052-494">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="fd052-495">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="fd052-495">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="fd052-496">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-496">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="fd052-497">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="fd052-497">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="fd052-498">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-498">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="fd052-499">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="fd052-499">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="fd052-500">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-500">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="fd052-501">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="fd052-501">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="fd052-502">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-502">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="fd052-503">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="fd052-503">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="fd052-504">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-504">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="fd052-505">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="fd052-505">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="fd052-506">Get-AzureRmRecoveryServicesBackItem cmdlet에 정책 필터 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-506">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="fd052-507">해당 명령은 지정된 정책 ID에 의해 보호되는 백업 항목의 목록을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-507">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="fd052-508">Microsoft.Azure.Management.RecoveryServices.Backup을 버전 3.0.0-preview로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="fd052-508">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="fd052-509">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-509">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="fd052-510">Restore-AzureRmRecoveryServicesBackupItem에 TargetResourceGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-510">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="fd052-511">관리 디스크가 복원될 리소스 그룹</span><span class="sxs-lookup"><span data-stu-id="fd052-511">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="fd052-512">관리 디스크가 있는 VM의 백업에 적용 가능</span><span class="sxs-lookup"><span data-stu-id="fd052-512">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="fd052-513">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="fd052-513">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="fd052-514">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-514">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="fd052-515">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="fd052-515">AzureRM.RedisCache</span></span>
* <span data-ttu-id="fd052-516">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-516">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="fd052-517">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="fd052-517">AzureRM.Relay</span></span>
* <span data-ttu-id="fd052-518">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-518">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fd052-519">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fd052-519">AzureRM.Resources</span></span>
* <span data-ttu-id="fd052-520">구독 범위에서 템플릿 배포를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-520">Support template deployment at subscription scope.</span></span> <span data-ttu-id="fd052-521">새 cmdlet 추가:</span><span class="sxs-lookup"><span data-stu-id="fd052-521">Add new Cmdlets:</span></span>
    - <span data-ttu-id="fd052-522">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="fd052-522">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="fd052-523">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="fd052-523">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="fd052-524">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="fd052-524">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="fd052-525">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="fd052-525">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="fd052-526">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="fd052-526">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="fd052-527">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="fd052-527">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="fd052-528">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="fd052-528">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="fd052-529">Set-AzureRmResource에 컨텍스트를 전달할 때 오류가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-529">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="fd052-530">New-AzureRmResourceGroupDeployment의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-530">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="fd052-531">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-531">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="fd052-532">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="fd052-532">AzureRM.Scheduler</span></span>
* <span data-ttu-id="fd052-533">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-533">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="fd052-534">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fd052-534">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="fd052-535">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-535">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="fd052-536">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="fd052-536">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="fd052-537">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-537">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="fd052-538">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fd052-538">AzureRM.Sql</span></span>
* <span data-ttu-id="fd052-539">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-539">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="fd052-540">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="fd052-540">AzureRM.Storage</span></span>
* <span data-ttu-id="fd052-541">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-541">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="fd052-542">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="fd052-542">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="fd052-543">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-543">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="fd052-544">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="fd052-544">AzureRM.Tags</span></span>
* <span data-ttu-id="fd052-545">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-545">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="fd052-546">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="fd052-546">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="fd052-547">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-547">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="fd052-548">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="fd052-548">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="fd052-549">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-549">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="fd052-550">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="fd052-550">AzureRM.Websites</span></span>
* <span data-ttu-id="fd052-551">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-551">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="fd052-552">6.6.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="fd052-552">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="fd052-553">일반</span><span class="sxs-lookup"><span data-stu-id="fd052-553">General</span></span>
* <span data-ttu-id="fd052-554">전체 매개 변수 형식 및 올바른 입/출력 형식을 포함하도록 모든 도움말 파일을 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-554">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="fd052-555">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fd052-555">AzureRM.Profile</span></span>
* <span data-ttu-id="fd052-556">Common.Strategy 라이브러리가 리소스에 대한 현재 구성이 대상 리소스와 호환되는지 유효성을 검사할 수 있도록 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-556">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="fd052-557">Common.Storage에 ps1xml 형식 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-557">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="fd052-558">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="fd052-558">Azure.Storage</span></span>
* <span data-ttu-id="fd052-559">DefaultProfile에서 저장소 컨텍스트를 가져오기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-559">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="fd052-560">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-560">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="fd052-561">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="fd052-561">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="fd052-562">문제 https://github.com/Azure/azure-powershell/issues/6370 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-562">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="fd052-563">PsApiManagementApi를 ApiContract로 좌표 이동하도록 Automapper 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="fd052-563">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="fd052-564">문제 https://github.com/Azure/azure-powershell/issues/6515 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-564">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="fd052-565">인코딩 형식을 사용하여 오버로드하지 않도록 File.Save 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="fd052-565">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="fd052-566">문제 https://github.com/Azure/azure-powershell/issues/6560 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-566">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="fd052-567">apiId에서 패턴 예외를 수정하는 4.0.3 Nuget 버전으로 업그레이드됨</span><span class="sxs-lookup"><span data-stu-id="fd052-567">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fd052-568">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fd052-568">AzureRM.Compute</span></span>
* <span data-ttu-id="fd052-569">PremiumLRS 저장소 계정 형식 이름 바꾸기로 인해 New-AzureRmVm에서 DiskFileParameterSet를 사용하여 vm 생성 시 실패하는 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-569">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="fd052-570">Invoke-AzureRmVMRunCommand cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-570">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="fd052-571">Get-AzureRmAvailabilitySet를 업데이트하여 구독에서 모든 가용성 집합 리스트를 사용하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-571">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="fd052-572">(ResouceGroupName 매개 변수는 이제 선택적 요소입니다.)</span><span class="sxs-lookup"><span data-stu-id="fd052-572">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="fd052-573">vm 선별에 가속화된 네트워크를 사용하도록 'New-AzureRmVm'의 SimpleParameterSet를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-573">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="fd052-574">New-AzureRmVmss 간단 매개 변수가 사용자 지정 LB가 이미 존재할 때 vms 생성에 실패하도록 설정하여 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-574">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="fd052-575">New-AzureRmDisk에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-575">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="fd052-576">'New-AzureRmVM'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-576">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="fd052-577">Set-AzureRmVMOSDisk에 대한 설명 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-577">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="fd052-578">Set-AzureRmVMBginfoExtension 맞춤법 및 접두사를 수정하도록 예제 1을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-578">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="fd052-579">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="fd052-579">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="fd052-580">ADF.Net SDK 버전을 1.1.0으로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-580">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="fd052-581">데이터 팩터리를 공유하는 자체 호스팅된 통합 런타임을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-581">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="fd052-582">새 매개 변수 -SharedIntegrationRuntimeResourceId를 Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="fd052-582">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="fd052-583">새로운 선택적 매개 변수 -LinkedDataFactoryName을 Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="fd052-583">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="fd052-584">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="fd052-584">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="fd052-585">DataPlane SDK(Microsoft.Azure.DataLake.Store) 버전을 1.1.9로 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-585">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="fd052-586">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="fd052-586">AzureRM.EventHub</span></span>
* <span data-ttu-id="fd052-587">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-587">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="fd052-588">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="fd052-588">AzureRM.Insights</span></span>
* <span data-ttu-id="fd052-589">도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-589">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="fd052-590">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview를 사용</span><span class="sxs-lookup"><span data-stu-id="fd052-590">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="fd052-591">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="fd052-591">AzureRM.KeyVault</span></span>
* <span data-ttu-id="fd052-592">Set-AzureRmKeyVaultAccessPolicy 내 파이핑 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-592">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="fd052-593">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fd052-593">AzureRM.Network</span></span>
* <span data-ttu-id="fd052-594">LoadBalancerInboundNatPoolConfig cmdlet에 대한 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-594">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fd052-595">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fd052-595">AzureRM.Resources</span></span>
* <span data-ttu-id="fd052-596">'Get-AzureRmResource'에 대한 태그 이름 및 값을 제공할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-596">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="fd052-597">'Set-AzureRmResource'를 사용하여 파이핑 시나리오 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-597">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="fd052-598">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fd052-598">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="fd052-599">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-599">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="fd052-600">몇 가지 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-600">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="fd052-601">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fd052-601">AzureRM.Sql</span></span>
* <span data-ttu-id="fd052-602">다음 cmdlet 사용하여 서버 Advanced Threat Protection 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-602">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="fd052-603">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fd052-603">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="fd052-604">다음 cmdlet을 사용하여 취약성 평가 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-604">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="fd052-605">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="fd052-605">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="fd052-606">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="fd052-606">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="fd052-607">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="fd052-607">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="fd052-608">Remove-AzureRmSqlServerFirewallRule의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-608">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="fd052-609">Get-AzureSqlSyncGroupLog에서 미국이 아닌 문화권에서 날짜/시간을 올바르지 않게 다루는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-609">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="fd052-610">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="fd052-610">AzureRM.Storage</span></span>
* <span data-ttu-id="fd052-611">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-611">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="fd052-612">StorageAccount cmdlet 출력을 테이블 뷰로 표시</span><span class="sxs-lookup"><span data-stu-id="fd052-612">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="fd052-613">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="fd052-613">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="fd052-614">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="fd052-614">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="fd052-615">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="fd052-615">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="fd052-616">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="fd052-616">AzureRM.Tags</span></span>
* <span data-ttu-id="fd052-617">태그 cmdlet 도움말에서 잘못된 문을 제거합니다</span><span class="sxs-lookup"><span data-stu-id="fd052-617">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="fd052-618">6.5.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="fd052-618">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="fd052-619">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fd052-619">AzureRM.Profile</span></span>
* <span data-ttu-id="fd052-620">'Get-AzureRmContextAutosaveSetting'에 대한 도움말이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-620">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="fd052-621">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="fd052-621">Azure.Storage</span></span>
* <span data-ttu-id="fd052-622">쓰기 전용 SaS 토큰을 사용하는 Blob 또는 파일 업로드 지원</span><span class="sxs-lookup"><span data-stu-id="fd052-622">Support Upload Blob or File with write only Sas token</span></span>
* <span data-ttu-id="fd052-623">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="fd052-623">Set-AzureStorageBlobContent</span></span>
* <span data-ttu-id="fd052-624">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="fd052-624">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="fd052-625">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="fd052-625">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="fd052-626">필수 속성 ResourceGroupName을 AS에 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-626">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="fd052-627">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="fd052-627">AzureRM.Automation</span></span>
* <span data-ttu-id="fd052-628">도움말을 업데이트하고 'New-AzureRMAutomationSchedule'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-628">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fd052-629">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fd052-629">AzureRM.Compute</span></span>
* <span data-ttu-id="fd052-630">-Tag 매개 변수를 Update/New-AzureRmAvailabilitySet에 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-630">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="fd052-631">‘Add-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-631">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="fd052-632">‘Remove-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-632">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="fd052-633">‘Set-AzureRmVMAccessExtension’에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-633">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="fd052-634">기본으로 SinglePlacementGroup을 false로 설정하고 단일 배치 그룹에 VMSS를 만들 수 있는 스위치 매개 변수 'SinglePlacementGroup'을 추가하도록 New-AzureRmVmss에 대한 SimpleParameterSet을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-634">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="fd052-635">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="fd052-635">AzureRM.EventHub</span></span>
* <span data-ttu-id="fd052-636">PSEventHubDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="fd052-636">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="fd052-637">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="fd052-637">AzureRM.KeyVault</span></span>
* <span data-ttu-id="fd052-638">Set-AzureRmKeyVaultAccessPolicy에 대한 오류 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-638">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="fd052-639">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="fd052-639">AzureRM.LogicApp</span></span>
* <span data-ttu-id="fd052-640">New-AzureRmLogicApp에서 "매개 변수 집합을 확인할 수 없습니다" 오류 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-640">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="fd052-641">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fd052-641">AzureRM.Network</span></span>
* <span data-ttu-id="fd052-642">Set/Add-AzureRmVirtualNetworkPeering에 대한 여러 테넌트의 가상 네트워크에서 피어링을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="fd052-642">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="fd052-643">Application Gateway에 대한 아래 cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-643">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="fd052-644">New-AzureRmApplicationGateway: EnableFIPS 플래그 및 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-644">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="fd052-645">New-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-645">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="fd052-646">Set-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-646">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="fd052-647">최신 생성기를 사용하여 RouteTable cmdlet을 재생성</span><span class="sxs-lookup"><span data-stu-id="fd052-647">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="fd052-648">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="fd052-648">AzureRM.Relay</span></span>
* <span data-ttu-id="fd052-649">markdown 파일을 업데이트하여 예제에서 매개 변수 이름 문제에 대해 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-649">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fd052-650">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fd052-650">AzureRM.Resources</span></span>
* <span data-ttu-id="fd052-651">Roledefinition 및 Roleassignment cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-651">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="fd052-652">페이징의 일부분으로 수행하는 추가 roledefinition 호출을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-652">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="fd052-653">Get-AzureRmRoleAssignment cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-653">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="fd052-654">-ExpandPrincipalGroups 명령 매개 변수 기능 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-654">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="fd052-655">'Get-AzureRmResource'에서 '-ResourceType' 매개 변수가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-655">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="fd052-656">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fd052-656">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="fd052-657">top 및 skip 매개 변수가 cmdlet 목록을 나열하도록 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-657">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="fd052-658">표준을 프리미엄 네임스페이스 마이그레이션 cmdlet에 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-658">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="fd052-659">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="fd052-659">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="fd052-660">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="fd052-660">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="fd052-661">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="fd052-661">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="fd052-662">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="fd052-662">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="fd052-663">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="fd052-663">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="fd052-664">PSServiceBusDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="fd052-664">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="fd052-665">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="fd052-665">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="fd052-666">‘New-AzureRmServiceFabricCluster’에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-666">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="fd052-667">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fd052-667">AzureRM.Sql</span></span>
* <span data-ttu-id="fd052-668">Management.Sql에 대한 새 cmdlet을 추가하여 고객이 TDE 인증서를 SQL Server 인스턴스 또는 Managed Instance에 추가할 수 있도록 허용</span><span class="sxs-lookup"><span data-stu-id="fd052-668">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="fd052-669">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="fd052-669">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="fd052-670">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="fd052-670">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="fd052-671">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="fd052-671">AzureRM.Websites</span></span>
* <span data-ttu-id="fd052-672">`Set-AzureRmWebApp -AssignIdentity` 및 `Set-AzureRmWebAppSlot -AssignIdentity`가 false로 설정되면 사이트 개체에서 Identity 속성이 제거됩니다. 미리보기 태그도 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-672">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="fd052-673">`Get-AzureRmWebAppMetrics`, `Get-AzureRmAppServicePlanMetrics` 예제가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-673">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="fd052-674">`Set-AzureRmWebApp -PhpVersion`이 유효한 php 버전으로 해제 지원</span><span class="sxs-lookup"><span data-stu-id="fd052-674">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="fd052-675">6.4.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="fd052-675">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="fd052-676">일반</span><span class="sxs-lookup"><span data-stu-id="fd052-676">General</span></span>
* <span data-ttu-id="fd052-677">대부분의 모듈에 대한 도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-677">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="fd052-678">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fd052-678">AzureRM.Profile</span></span>
* <span data-ttu-id="fd052-679">기본 출력 형식에 추가된 Ps1Xml 특성</span><span class="sxs-lookup"><span data-stu-id="fd052-679">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fd052-680">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fd052-680">AzureRM.Compute</span></span>
* <span data-ttu-id="fd052-681">VMSS에 대한 IP 태그 기능</span><span class="sxs-lookup"><span data-stu-id="fd052-681">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="fd052-682">'New-AzureRmVmssIpTagConfig' cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-682">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="fd052-683">New-AzureRmVmssIpConfig에 IpTag 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-683">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="fd052-684">VMSS에 대한 자동 OS 롤백 기능</span><span class="sxs-lookup"><span data-stu-id="fd052-684">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="fd052-685">New-AzureRmVmssConfig 및 Update-AzureRmVmss에 DisableAutoRollback 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-685">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="fd052-686">Vmss에 대한 OS 업그레이드 기록 기능</span><span class="sxs-lookup"><span data-stu-id="fd052-686">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="fd052-687">Get-AzureRmVmss에 OSUpgradeHistory 스위치 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-687">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="fd052-688">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="fd052-688">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="fd052-689">다음 명령을 통해 카탈로그 액세스 제어 목록에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-689">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="fd052-690">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="fd052-690">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="fd052-691">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="fd052-691">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="fd052-692">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="fd052-692">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="fd052-693">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="fd052-693">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="fd052-694">Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl에 대한 취소 지원 및 진행률 추적 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-694">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="fd052-695">Export-AzureRmDataLakeStoreChildItemProperties에 대한 취소 지원 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-695">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="fd052-696">재귀 작업을 수행하는 cmdlet에 대한 디버그 메시지 플러시 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-696">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="fd052-697">DataLake cmdlet의 테스트 위치 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-697">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="fd052-698">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="fd052-698">AzureRM.EventHub</span></span>
* <span data-ttu-id="fd052-699">목록 작업 cmdlet Get-AzureRmEventHub 및 Get-AzureRmEventHubConsumerGroup에 선택적 MaxCount 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-699">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="fd052-700">새 EventHub 만드는 동안 하나 이상의 매개 변수가 필요한 New-AzureRmEventHub cmdlet 문제를 해결.</span><span class="sxs-lookup"><span data-stu-id="fd052-700">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="fd052-701">기본 매개 변수 집합을 제공.</span><span class="sxs-lookup"><span data-stu-id="fd052-701">Provided Default Parameter set.</span></span>
* <span data-ttu-id="fd052-702">선택적 매개 변수 -KeyValue를 New-AzureRmEventHubKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-702">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="fd052-703">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="fd052-703">AzureRM.KeyVault</span></span>
* <span data-ttu-id="fd052-704">Get-AzureRmKeyVault -Tag 실행 시 모든 리소스가 리턴되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-704">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="fd052-705">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fd052-705">AzureRM.Network</span></span>
* <span data-ttu-id="fd052-706">영역 중복 VirtualNetworkGateways에 대한 새 Sku를 노출합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-706">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="fd052-707">기능에 대한 새 명령이 추가됨: ARM을 통한 ExpressRoute Partner APIs</span><span class="sxs-lookup"><span data-stu-id="fd052-707">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="fd052-708">Get- AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-708">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="fd052-709">Set-AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-709">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="fd052-710">Add-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-710">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="fd052-711">Get-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-711">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="fd052-712">Remove-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-712">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="fd052-713">Get-AzureRMExpressRouteCrossConnectionArpTable 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-713">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="fd052-714">Get-AzureRMExpressRouteCrossConnectionRouteTable 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-714">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="fd052-715">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-715">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="fd052-716">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="fd052-716">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="fd052-717">Get-AzureRmRecoveryServicesBackupStatus cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-717">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="fd052-718">이 cmdlet은 VM ID를 가져와서 VM이 구독에서 일부 자격 증명 모음으로 보호되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-718">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="fd052-719">이러한 자격 증명 모음이 존재하는 경우 cmdlet은 자격 증명 모음 세부 정보를 출력 합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-719">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fd052-720">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fd052-720">AzureRM.Resources</span></span>
* <span data-ttu-id="fd052-721">Get-AzureRmPolicyAssignment cmdlet을 다음과 같이 업데이트함.</span><span class="sxs-lookup"><span data-stu-id="fd052-721">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="fd052-722">관리 그룹 수준에서 -Scope 값 리스팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-722">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="fd052-723">관리 그룹 수준에서 -Scope 값을 사용하여 개별 할당값을 검색하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-723">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="fd052-724">제어 매개 변수에 -Effective 및 -All 스위치 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-724">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="fd052-725">Get/New/Remove/Set-AzureRmPolicyDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-725">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="fd052-726">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-726">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="fd052-727">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-727">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="fd052-728">Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-728">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="fd052-729">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-729">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="fd052-730">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-730">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="fd052-731">'New-AzureRmResourceGroupDeployment'에서 'TemplateParameterObject'를 사용하는 경우 매개 변수에 KeyVault 비밀 참조 지원 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-731">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="fd052-732">'New-AzureRmADAppCredential'에 대해 '-EndDate' 매개 변수가 무시되는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-732">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="fd052-733">'Add-AzureRmADGroupMember'가 요청에 잘못된 URL을 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-733">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="fd052-734">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fd052-734">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="fd052-735">선택적 매개 변수 -KeyValue를 New-AzureRmServiceBusKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-735">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="fd052-736">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fd052-736">AzureRM.Sql</span></span>
* <span data-ttu-id="fd052-737">New-AzureRmSqlDatabaseRestorePoint 도움말에서 SQLDW에 대한 사용자 정의 복원 지점 명시</span><span class="sxs-lookup"><span data-stu-id="fd052-737">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="fd052-738">몇 가지 cmdlet에서-ComputeGeneration 매개 변수의 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-738">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="fd052-739">6.3.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="fd052-739">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="fd052-740">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fd052-740">AzureRM.Profile</span></span>
* <span data-ttu-id="fd052-741">Enable-AzureRmContextAutoSave에 대한 오류 메시지 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-741">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="fd052-742">이전 컨텍스트 없이 'Connect-AzureRmAccount' 실행 시 각 구독에 대한 컨텍스트 생성</span><span class="sxs-lookup"><span data-stu-id="fd052-742">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="fd052-743">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="fd052-743">Azure.Storage</span></span>
* <span data-ttu-id="fd052-744">도움말 파일 내 -Permissions 매개 변수에 대한 추가 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-744">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fd052-745">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fd052-745">AzureRM.Compute</span></span>
* <span data-ttu-id="fd052-746">'Get-AzureRmVmDiskEncryptionStatus'가 데이터 디스크가 없는 VM에 대해 관찰된 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-746">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="fd052-747">Compute 클라이언트 라이브러리 버전을 업데이트하여 다음 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-747">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="fd052-748">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="fd052-748">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="fd052-749">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="fd052-749">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="fd052-750">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="fd052-750">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="fd052-751">다음 cmdlet이 '작업 ID' 및 '작업 상태'를 올바르게 표시하도록 수정:</span><span class="sxs-lookup"><span data-stu-id="fd052-751">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="fd052-752">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="fd052-752">Start-AzureRmVM</span></span>
    - <span data-ttu-id="fd052-753">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="fd052-753">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="fd052-754">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="fd052-754">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="fd052-755">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="fd052-755">Set-AzureRmVM</span></span>
    - <span data-ttu-id="fd052-756">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="fd052-756">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="fd052-757">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="fd052-757">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="fd052-758">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="fd052-758">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="fd052-759">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="fd052-759">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="fd052-760">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="fd052-760">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="fd052-761">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="fd052-761">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="fd052-762">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="fd052-762">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="fd052-763">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="fd052-763">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="fd052-764">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="fd052-764">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="fd052-765">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="fd052-765">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="fd052-766">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="fd052-766">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="fd052-767">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="fd052-767">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="fd052-768">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="fd052-768">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="fd052-769">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="fd052-769">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="fd052-770">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="fd052-770">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="fd052-771">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="fd052-771">AzureRM.EventGrid</span></span>
* <span data-ttu-id="fd052-772">Update-AzureRmEventGridSubscription cmdlet의 SubjectBeginsWith/SubjectEndsWith에 대한 ValidateNotNullOrEmpty 유효성 검사 조건을 제거하여 필요에 따라 이러한 매개 변수를 빈 문자열로 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-772">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="fd052-773">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="fd052-773">AzureRM.KeyVault</span></span>
* <span data-ttu-id="fd052-774">Get-AzureRmKeyVault -Tag 실행 시 태그가 리턴되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-774">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="fd052-775">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="fd052-775">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="fd052-776">Policy Insights cmdlet의 공개 릴리스</span><span class="sxs-lookup"><span data-stu-id="fd052-776">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="fd052-777">API 버전 2018-04-04 사용</span><span class="sxs-lookup"><span data-stu-id="fd052-777">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="fd052-778">PolicyDefinitionReferenceId를 Get-AzureRmPolicyStateSummary의 결과 집합에 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-778">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="fd052-779">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="fd052-779">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="fd052-780">-Vault 매개 변수를 RecoveryServices.Backup cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="fd052-780">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="fd052-781">전달되는 경우 이는 Set-AzureRmRecoveryServicesContext cmdlet을 재정의함.</span><span class="sxs-lookup"><span data-stu-id="fd052-781">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="fd052-782">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fd052-782">AzureRM.Sql</span></span>
* <span data-ttu-id="fd052-783">Get-AzureRmSqlDatabaseExpanded에 대한 도움말 파일의 예가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-783">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="fd052-784">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="fd052-784">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="fd052-785">Add-AzureRmTrafficManagerEndpointConfig에대한 도움말 파일이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-785">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="fd052-786">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="fd052-786">AzureRM.Websites</span></span>
* <span data-ttu-id="fd052-787">-AssignIdentity를 사용할 때 AppSetting을 덮어쓰지 않도록 'Set-AzureRmWebApp'이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-787">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="fd052-788">'New-AzureRmWebAppSlot'이 AppServicePlan을 옵션 매개변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-788">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="fd052-789">6.2.1 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="fd052-789">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="fd052-790">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="fd052-790">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="fd052-791">PSWorkspace 모델이 Network 형식을 매개 변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="fd052-791">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="fd052-792">6.2.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="fd052-792">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="fd052-793">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fd052-793">AzureRM.Profile</span></span>
* <span data-ttu-id="fd052-794">Newtonsoft.Json의 버전 10.0.3이 모듈 가져오기에 로드되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-794">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fd052-795">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fd052-795">AzureRM.Compute</span></span>
* <span data-ttu-id="fd052-796">VMSS VM 업데이트 기능</span><span class="sxs-lookup"><span data-stu-id="fd052-796">VMSS VM Update feature</span></span>
    - <span data-ttu-id="fd052-797">'Update-AzureRmVmssVM' 및 'New-AzureRmVMDataDisk' cmdlets 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-797">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="fd052-798">데이터 디스크를 Vmss VM에 추가할 수 있도록 지원하기 위해 VirtualMachineScaleSetVM 매개변수를 'Add-AzureRmVMDataDisk' cmdlet에 추가하였습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-798">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="fd052-799">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="fd052-799">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="fd052-800">ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.8.0-preview로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-800">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="fd052-801">팩터리 리포지토리 작업 구성 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-801">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="fd052-802">QuickBooks LinkedService가 ConsumerKey 및 consumerSecret 속성을 노출하도록 업데이트됨 </span><span class="sxs-lookup"><span data-stu-id="fd052-802">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="fd052-803">여러 모델 유형을 SecretBase에서 개체로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="fd052-803">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="fd052-804">Blob 이벤트 트리거 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-804">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="fd052-805">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="fd052-805">AzureRM.KeyVault</span></span>
* <span data-ttu-id="fd052-806">예제 출력으로 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-806">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="fd052-807">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fd052-807">AzureRM.Network</span></span>
* <span data-ttu-id="fd052-808">Network Watcher cmdlet에서 트래픽 분석 매개 변수를 사용가능하도록 설정</span><span class="sxs-lookup"><span data-stu-id="fd052-808">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fd052-809">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fd052-809">AzureRM.Resources</span></span>
* <span data-ttu-id="fd052-810">'Get AzureRmResource'에서 반환된 'PSResource' 개체의 'Properties' 속성의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-810">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="fd052-811">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="fd052-811">AzureRM.Scheduler</span></span>
* <span data-ttu-id="fd052-812">ServiceBusQueueJob 업데이트가 새 인증 값을 설정하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="fd052-812">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="fd052-813">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fd052-813">AzureRM.Sql</span></span>
* <span data-ttu-id="fd052-814">옵션 LicenseType 매개 변수를 사용하여 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="fd052-814">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="fd052-815">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="fd052-815">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="fd052-816">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="fd052-816">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="fd052-817">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="fd052-817">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="fd052-818">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="fd052-818">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="fd052-819">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="fd052-819">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="fd052-820">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="fd052-820">AzureRM.Websites</span></span>
* <span data-ttu-id="fd052-821">'New-AzureRMWebApp'이 전략 라이브러리의 공통 알고리즘을 사용하도록 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-821">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="fd052-822">6.1.0 - 2018년 5월</span><span class="sxs-lookup"><span data-stu-id="fd052-822">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="fd052-823">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fd052-823">AzureRM.Profile</span></span>
* <span data-ttu-id="fd052-824">'Clear-AzureRmContext'를 실행하면 이전 기본 컨텍스트의 이름으로 빈 컨텍스트가 유지되어 사용자가 이전 이름으로 새 컨텍스트를 만들지 못하게 되는 문제를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-824">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="fd052-825">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="fd052-825">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="fd052-826">AS에서 게이트웨이가 작업을 연결하거나 연결 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-826">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="fd052-827">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="fd052-827">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="fd052-828">ApiVersions, ApiReleases 및 ApiRevisions에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-828">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="fd052-829">ServiceFabric 백 엔드에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-829">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="fd052-830">Application Insights 로거에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-830">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="fd052-831">'기본' SKU를 API Management 서비스의 유효한 SKU로 인식하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-831">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="fd052-832">개인 CA가 발급한 인증서를 루트 또는 CA로 설치하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-832">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="fd052-833">KeyVault 및 다중 프록시 호스트 이름을 통한 사용자 정의 SSL 인증서를 수락하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-833">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="fd052-834">MSI ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="fd052-834">Added support for MSI identity</span></span>
* <span data-ttu-id="fd052-835">URL을 통한 정책을 수락하는 지원 추가됨 참고: 다음 cmdlet은 이후 릴리스에서 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-835">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="fd052-836">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="fd052-836">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="fd052-837">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd052-837">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="fd052-838">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="fd052-838">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="fd052-839">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="fd052-839">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="fd052-840">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="fd052-840">AzureRM.Batch</span></span>
* <span data-ttu-id="fd052-841">새 cmdlet Get AzureBatchPoolNodeCounts 릴리스</span><span class="sxs-lookup"><span data-stu-id="fd052-841">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="fd052-842">새 cmdlet Start-AzureBatchComputeNodeServiceLogUpload 릴리스</span><span class="sxs-lookup"><span data-stu-id="fd052-842">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="fd052-843">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="fd052-843">AzureRM.Consumption</span></span>
* <span data-ttu-id="fd052-844">Expand, ResourceGroup, InstanceName, InstanceId, Tags, Top on Cmdlet Get-AzureRmConsumptionUsageDetail 등 새 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="fd052-844">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="fd052-845">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="fd052-845">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="fd052-846">Export-AzureRmDataLakeStoreChildItemProperties에 대한 예제 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-846">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="fd052-847">Set-AzureRmDataLakeStoreItemAclEntry에서 재귀 사례에 대한 null 매개 변수 예외 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-847">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="fd052-848">Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry에 대한 도움말 파일 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-848">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="fd052-849">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fd052-849">AzureRM.Network</span></span>
* <span data-ttu-id="fd052-850">18.0.0-preview에서 19.0.0-preview로 네트워크 SDK 버전 업그레이드</span><span class="sxs-lookup"><span data-stu-id="fd052-850">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="fd052-851">프로토콜 구성을 만들기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="fd052-851">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="fd052-852">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd052-852">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="fd052-853">기존 Express 경로 회로에 새 회로 연결을 추가하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="fd052-853">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="fd052-854">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-854">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="fd052-855">기존 Express 경로 회로에서 회로 연결을 제거하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="fd052-855">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="fd052-856">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-856">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="fd052-857">회로 연결을 검색하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="fd052-857">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="fd052-858">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="fd052-858">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="fd052-859">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="fd052-859">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="fd052-860">생성된 인증서로 고정 서버 인증 사용(문제 # 5998)</span><span class="sxs-lookup"><span data-stu-id="fd052-860">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="fd052-861">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fd052-861">AzureRM.Sql</span></span>
* <span data-ttu-id="fd052-862">AuditActions 또는 AuditActionGroups를 제거할 수 있도록 업데이트된 감사 cmdlet</span><span class="sxs-lookup"><span data-stu-id="fd052-862">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="fd052-863">'Azure 복구 서비스 자격 증명 모음을 사용하여 장기 보존 정책을 구성하면 정책이 더 이상 지원되지 않습니다. 새로운 유연 보유 정책으로 요청을 제출하십시오.'라는 메시지와 함께 명령이 실패하는 새로운 유연 보유 정책을 설정할 때</span><span class="sxs-lookup"><span data-stu-id="fd052-863">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="fd052-864">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy의 문제 수정</span><span class="sxs-lookup"><span data-stu-id="fd052-864">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="fd052-865">Azure SQL Database/ElasticPool Creation/Update 관련 cmdlet을 모두 업데이트하여 규모 및 계층 관련 속성에 대한 SKU 속성을 지원하는 새 데이터베이스 API를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-865">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="fd052-866">업데이트된 cmdlet는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-866">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="fd052-867">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="fd052-867">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="fd052-868">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="fd052-868">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="fd052-869">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="fd052-869">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="fd052-870">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="fd052-870">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="fd052-871">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="fd052-871">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="fd052-872">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="fd052-872">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="fd052-873">-Name 매개 변수를 사용할 때 -ResourceGroupName 매개 변수가 필요하도록 'Get-AzureRmTrafficManagerProfile'에 대한 매개 변수를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="fd052-873">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
