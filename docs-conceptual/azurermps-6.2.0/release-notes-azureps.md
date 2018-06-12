---
title: Azure PowerShell 변경 로그 | Microsoft Docs
description: Azure PowerShell에 대한 최신 릴리스의 변경 내용입니다.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: f90c77d8c9cd78315264fb0a0a58e047aefc5041
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/06/2018
ms.locfileid: "34821873"
---
# <a name="release-notes"></a><span data-ttu-id="09469-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="09469-103">Release notes</span></span>

<span data-ttu-id="09469-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="09469-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="620---june-2018"></a><span data-ttu-id="09469-105">6.2.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="09469-105">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="09469-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="09469-106">AzureRM.Profile</span></span>
* <span data-ttu-id="09469-107">Newtonsoft.Json의 버전 10.0.3이 모듈 가져오기에 로드되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="09469-107">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="09469-108">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="09469-108">AzureRM.Compute</span></span>
* <span data-ttu-id="09469-109">VMSS VM 업데이트 기능</span><span class="sxs-lookup"><span data-stu-id="09469-109">VMSS VM Update feature</span></span>
    - <span data-ttu-id="09469-110">'Update-AzureRmVmssVM' 및 'New-AzureRmVMDataDisk' cmdlets 추가</span><span class="sxs-lookup"><span data-stu-id="09469-110">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="09469-111">데이터 디스크를 Vmss VM에 추가할 수 있도록 지원하기 위해 VirtualMachineScaleSetVM 매개변수를 'Add-AzureRmVMDataDisk' cmdlet에 추가하였습니다.</span><span class="sxs-lookup"><span data-stu-id="09469-111">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="09469-112">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="09469-112">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="09469-113">ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.8.0-preview로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="09469-113">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="09469-114">팩터리 리포지토리 작업 구성 추가</span><span class="sxs-lookup"><span data-stu-id="09469-114">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="09469-115">QuickBooks LinkedService가 ConsumerKey 및 consumerSecret 속성을 노출하도록 업데이트됨 </span><span class="sxs-lookup"><span data-stu-id="09469-115">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="09469-116">여러 모델 유형을 SecretBase에서 개체로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="09469-116">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="09469-117">Blob 이벤트 트리거 추가</span><span class="sxs-lookup"><span data-stu-id="09469-117">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="09469-118">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="09469-118">AzureRM.KeyVault</span></span>
* <span data-ttu-id="09469-119">예제 출력으로 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="09469-119">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="09469-120">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="09469-120">AzureRM.Network</span></span>
* <span data-ttu-id="09469-121">Network Watcher cmdlet에서 트래픽 분석 매개 변수를 사용가능하도록 설정</span><span class="sxs-lookup"><span data-stu-id="09469-121">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="09469-122">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="09469-122">AzureRM.Resources</span></span>
* <span data-ttu-id="09469-123">'Get AzureRmResource'에서 반환된 'PSResource' 개체의 'Properties' 속성의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="09469-123">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="09469-124">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="09469-124">AzureRM.Scheduler</span></span>
* <span data-ttu-id="09469-125">ServiceBusQueueJob 업데이트가 새 인증 값을 설정하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="09469-125">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="09469-126">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="09469-126">AzureRM.Sql</span></span>
* <span data-ttu-id="09469-127">옵션 LicenseType 매개 변수를 사용하여 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="09469-127">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="09469-128">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="09469-128">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="09469-129">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="09469-129">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="09469-130">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="09469-130">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="09469-131">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="09469-131">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="09469-132">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="09469-132">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="09469-133">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="09469-133">AzureRM.Websites</span></span>
* <span data-ttu-id="09469-134">'New-AzureRMWebApp'이 전략 라이브러리의 공통 알고리즘을 사용하도록 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="09469-134">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="09469-135">6.1.0 - 2018년 5월</span><span class="sxs-lookup"><span data-stu-id="09469-135">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="09469-136">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="09469-136">AzureRM.Profile</span></span>
* <span data-ttu-id="09469-137">'Clear-AzureRmContext'를 실행하면 이전 기본 컨텍스트의 이름으로 빈 컨텍스트가 유지되어 사용자가 이전 이름으로 새 컨텍스트를 만들지 못하게 되는 문제를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="09469-137">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="09469-138">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="09469-138">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="09469-139">AS에서 게이트웨이가 작업을 연결하거나 연결 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="09469-139">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="09469-140">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="09469-140">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="09469-141">ApiVersions, ApiReleases 및 ApiRevisions에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="09469-141">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="09469-142">ServiceFabric 백 엔드에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="09469-142">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="09469-143">Application Insights 로거에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="09469-143">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="09469-144">'기본' SKU를 API Management 서비스의 유효한 SKU로 인식하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="09469-144">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="09469-145">개인 CA가 발급한 인증서를 루트 또는 CA로 설치하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="09469-145">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="09469-146">KeyVault 및 다중 프록시 호스트 이름을 통한 사용자 정의 SSL 인증서를 수락하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="09469-146">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="09469-147">MSI ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="09469-147">Added support for MSI identity</span></span>
* <span data-ttu-id="09469-148">URL을 통한 정책을 수락하는 지원 추가됨 참고: 다음 cmdlet은 이후 릴리스에서 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="09469-148">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="09469-149">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="09469-149">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="09469-150">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="09469-150">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="09469-151">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="09469-151">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="09469-152">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="09469-152">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="09469-153">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="09469-153">AzureRM.Batch</span></span>
* <span data-ttu-id="09469-154">새 cmdlet Get AzureBatchPoolNodeCounts 릴리스</span><span class="sxs-lookup"><span data-stu-id="09469-154">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="09469-155">새 cmdlet Start-AzureBatchComputeNodeServiceLogUpload 릴리스</span><span class="sxs-lookup"><span data-stu-id="09469-155">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="09469-156">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="09469-156">AzureRM.Consumption</span></span>
* <span data-ttu-id="09469-157">Expand, ResourceGroup, InstanceName, InstanceId, Tags, Top on Cmdlet Get-AzureRmConsumptionUsageDetail 등 새 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="09469-157">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="09469-158">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="09469-158">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="09469-159">Export-AzureRmDataLakeStoreChildItemProperties에 대한 예제 수정</span><span class="sxs-lookup"><span data-stu-id="09469-159">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="09469-160">Set-AzureRmDataLakeStoreItemAclEntry에서 재귀 사례에 대한 null 매개 변수 예외 수정</span><span class="sxs-lookup"><span data-stu-id="09469-160">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="09469-161">Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry에 대한 도움말 파일 수정</span><span class="sxs-lookup"><span data-stu-id="09469-161">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="09469-162">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="09469-162">AzureRM.Network</span></span>
* <span data-ttu-id="09469-163">18.0.0-preview에서 19.0.0-preview로 네트워크 SDK 버전 업그레이드</span><span class="sxs-lookup"><span data-stu-id="09469-163">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="09469-164">프로토콜 구성을 만들기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="09469-164">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="09469-165">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="09469-165">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="09469-166">기존 Express 경로 회로에 새 회로 연결을 추가하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="09469-166">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="09469-167">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="09469-167">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="09469-168">기존 Express 경로 회로에서 회로 연결을 제거하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="09469-168">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="09469-169">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="09469-169">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="09469-170">회로 연결을 검색하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="09469-170">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="09469-171">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="09469-171">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="09469-172">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="09469-172">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="09469-173">생성된 인증서로 고정 서버 인증 사용(문제 # 5998)</span><span class="sxs-lookup"><span data-stu-id="09469-173">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="09469-174">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="09469-174">AzureRM.Sql</span></span>
* <span data-ttu-id="09469-175">AuditActions 또는 AuditActionGroups를 제거할 수 있도록 업데이트된 감사 cmdlet</span><span class="sxs-lookup"><span data-stu-id="09469-175">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="09469-176">'Azure 복구 서비스 자격 증명 모음을 사용하여 장기 보존 정책을 구성하면 정책이 더 이상 지원되지 않습니다. 새로운 유연 보유 정책으로 요청을 제출하십시오.'라는 메시지와 함께 명령이 실패하는 새로운 유연 보유 정책을 설정할 때</span><span class="sxs-lookup"><span data-stu-id="09469-176">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="09469-177">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy의 문제 수정</span><span class="sxs-lookup"><span data-stu-id="09469-177">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="09469-178">Azure SQL Database/ElasticPool Creation/Update 관련 cmdlet을 모두 업데이트하여 규모 및 계층 관련 속성에 대한 SKU 속성을 지원하는 새 데이터베이스 API를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="09469-178">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="09469-179">업데이트된 cmdlet는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="09469-179">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="09469-180">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="09469-180">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="09469-181">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="09469-181">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="09469-182">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="09469-182">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="09469-183">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="09469-183">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="09469-184">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="09469-184">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="09469-185">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="09469-185">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="09469-186">-Name 매개 변수를 사용할 때 -ResourceGroupName 매개 변수가 필요하도록 'Get-AzureRmTrafficManagerProfile'에 대한 매개 변수를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="09469-186">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>