---
title: Azure PowerShell 변경 로그 | Microsoft Docs
description: Azure PowerShell에 대한 최신 릴리스의 변경 내용입니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 3811e28dda69d194d23934943fb47d562f869fc4
ms.sourcegitcommit: 5a5b6dd216d5f805204244146cf6f88ad2f34fb4
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/19/2018
ms.locfileid: "36237816"
---
# <a name="release-notes"></a><span data-ttu-id="ec23a-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="ec23a-103">Release notes</span></span>

<span data-ttu-id="ec23a-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="ec23a-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="630---june-2018"></a><span data-ttu-id="ec23a-105">6.3.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="ec23a-105">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="ec23a-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="ec23a-106">AzureRM.Profile</span></span>
* <span data-ttu-id="ec23a-107">Enable-AzureRmContextAutoSave에 대한 오류 메시지 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-107">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="ec23a-108">이전 컨텍스트 없이 'Connect-AzureRmAccount' 실행 시 각 구독에 대한 컨텍스트 생성</span><span class="sxs-lookup"><span data-stu-id="ec23a-108">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="ec23a-109">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="ec23a-109">Azure.Storage</span></span>
* <span data-ttu-id="ec23a-110">도움말 파일 내 -Permissions 매개 변수에 대한 추가 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-110">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="ec23a-111">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="ec23a-111">AzureRM.Compute</span></span>
* <span data-ttu-id="ec23a-112">'Get-AzureRmVmDiskEncryptionStatus'가 데이터 디스크가 없는 VM에 대해 관찰된 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="ec23a-112">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="ec23a-113">Compute 클라이언트 라이브러리 버전을 업데이트하여 다음 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="ec23a-113">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="ec23a-114">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="ec23a-114">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="ec23a-115">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="ec23a-115">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="ec23a-116">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="ec23a-116">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="ec23a-117">다음 cmdlet이 '작업 ID' 및 '작업 상태'를 올바르게 표시하도록 수정:</span><span class="sxs-lookup"><span data-stu-id="ec23a-117">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="ec23a-118">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="ec23a-118">Start-AzureRmVM</span></span>
    - <span data-ttu-id="ec23a-119">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="ec23a-119">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="ec23a-120">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="ec23a-120">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="ec23a-121">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="ec23a-121">Set-AzureRmVM</span></span>
    - <span data-ttu-id="ec23a-122">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="ec23a-122">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="ec23a-123">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="ec23a-123">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="ec23a-124">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="ec23a-124">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="ec23a-125">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="ec23a-125">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="ec23a-126">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="ec23a-126">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="ec23a-127">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="ec23a-127">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="ec23a-128">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="ec23a-128">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="ec23a-129">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="ec23a-129">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="ec23a-130">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="ec23a-130">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="ec23a-131">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="ec23a-131">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="ec23a-132">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="ec23a-132">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="ec23a-133">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="ec23a-133">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="ec23a-134">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="ec23a-134">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="ec23a-135">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="ec23a-135">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="ec23a-136">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="ec23a-136">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="ec23a-137">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ec23a-137">AzureRM.EventGrid</span></span>
* <span data-ttu-id="ec23a-138">Update-AzureRmEventGridSubscription cmdlet의 SubjectBeginsWith/SubjectEndsWith에 대한 ValidateNotNullOrEmpty 유효성 검사 조건을 제거하여 필요에 따라 이러한 매개 변수를 빈 문자열로 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ec23a-138">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="ec23a-139">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ec23a-139">AzureRM.KeyVault</span></span>
* <span data-ttu-id="ec23a-140">Get-AzureRmKeyVault -Tag 실행 시 태그가 리턴되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ec23a-140">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="ec23a-141">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ec23a-141">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="ec23a-142">Policy Insights cmdlet의 공개 릴리스</span><span class="sxs-lookup"><span data-stu-id="ec23a-142">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="ec23a-143">API 버전 2018-04-04 사용</span><span class="sxs-lookup"><span data-stu-id="ec23a-143">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="ec23a-144">PolicyDefinitionReferenceId를 Get-AzureRmPolicyStateSummary의 결과 집합에 추가</span><span class="sxs-lookup"><span data-stu-id="ec23a-144">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="ec23a-145">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="ec23a-145">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="ec23a-146">-Vault 매개 변수를 RecoveryServices.Backup cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="ec23a-146">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="ec23a-147">전달되는 경우 이는 Set-AzureRmRecoveryServicesContext cmdlet을 재정의함.</span><span class="sxs-lookup"><span data-stu-id="ec23a-147">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="ec23a-148">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="ec23a-148">AzureRM.Sql</span></span>
* <span data-ttu-id="ec23a-149">Get-AzureRmSqlDatabaseExpanded에 대한 도움말 파일의 예가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-149">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="ec23a-150">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ec23a-150">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="ec23a-151">Add-AzureRmTrafficManagerEndpointConfig에대한 도움말 파일이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-151">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="ec23a-152">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="ec23a-152">AzureRM.Websites</span></span>
* <span data-ttu-id="ec23a-153">-AssignIdentity를 사용할 때 AppSetting을 덮어쓰지 않도록 'Set-AzureRmWebApp'이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-153">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="ec23a-154">'New-AzureRmWebAppSlot'이 AppServicePlan을 옵션 매개변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-154">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="ec23a-155">6.2.1 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="ec23a-155">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="ec23a-156">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ec23a-156">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="ec23a-157">PSWorkspace 모델이 Network 형식을 매개 변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-157">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="ec23a-158">6.2.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="ec23a-158">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="ec23a-159">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="ec23a-159">AzureRM.Profile</span></span>
* <span data-ttu-id="ec23a-160">Newtonsoft.Json의 버전 10.0.3이 모듈 가져오기에 로드되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ec23a-160">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="ec23a-161">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="ec23a-161">AzureRM.Compute</span></span>
* <span data-ttu-id="ec23a-162">VMSS VM 업데이트 기능</span><span class="sxs-lookup"><span data-stu-id="ec23a-162">VMSS VM Update feature</span></span>
    - <span data-ttu-id="ec23a-163">'Update-AzureRmVmssVM' 및 'New-AzureRmVMDataDisk' cmdlets 추가</span><span class="sxs-lookup"><span data-stu-id="ec23a-163">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="ec23a-164">데이터 디스크를 Vmss VM에 추가할 수 있도록 지원하기 위해 VirtualMachineScaleSetVM 매개변수를 'Add-AzureRmVMDataDisk' cmdlet에 추가하였습니다.</span><span class="sxs-lookup"><span data-stu-id="ec23a-164">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="ec23a-165">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="ec23a-165">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="ec23a-166">ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.8.0-preview로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ec23a-166">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="ec23a-167">팩터리 리포지토리 작업 구성 추가</span><span class="sxs-lookup"><span data-stu-id="ec23a-167">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="ec23a-168">QuickBooks LinkedService가 ConsumerKey 및 consumerSecret 속성을 노출하도록 업데이트됨 </span><span class="sxs-lookup"><span data-stu-id="ec23a-168">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="ec23a-169">여러 모델 유형을 SecretBase에서 개체로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="ec23a-169">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="ec23a-170">Blob 이벤트 트리거 추가</span><span class="sxs-lookup"><span data-stu-id="ec23a-170">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="ec23a-171">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ec23a-171">AzureRM.KeyVault</span></span>
* <span data-ttu-id="ec23a-172">예제 출력으로 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="ec23a-172">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="ec23a-173">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="ec23a-173">AzureRM.Network</span></span>
* <span data-ttu-id="ec23a-174">Network Watcher cmdlet에서 트래픽 분석 매개 변수를 사용가능하도록 설정</span><span class="sxs-lookup"><span data-stu-id="ec23a-174">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="ec23a-175">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="ec23a-175">AzureRM.Resources</span></span>
* <span data-ttu-id="ec23a-176">'Get AzureRmResource'에서 반환된 'PSResource' 개체의 'Properties' 속성의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ec23a-176">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="ec23a-177">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="ec23a-177">AzureRM.Scheduler</span></span>
* <span data-ttu-id="ec23a-178">ServiceBusQueueJob 업데이트가 새 인증 값을 설정하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ec23a-178">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="ec23a-179">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="ec23a-179">AzureRM.Sql</span></span>
* <span data-ttu-id="ec23a-180">옵션 LicenseType 매개 변수를 사용하여 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="ec23a-180">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="ec23a-181">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="ec23a-181">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="ec23a-182">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="ec23a-182">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="ec23a-183">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="ec23a-183">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="ec23a-184">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="ec23a-184">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="ec23a-185">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="ec23a-185">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="ec23a-186">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="ec23a-186">AzureRM.Websites</span></span>
* <span data-ttu-id="ec23a-187">'New-AzureRMWebApp'이 전략 라이브러리의 공통 알고리즘을 사용하도록 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ec23a-187">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="ec23a-188">6.1.0 - 2018년 5월</span><span class="sxs-lookup"><span data-stu-id="ec23a-188">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="ec23a-189">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="ec23a-189">AzureRM.Profile</span></span>
* <span data-ttu-id="ec23a-190">'Clear-AzureRmContext'를 실행하면 이전 기본 컨텍스트의 이름으로 빈 컨텍스트가 유지되어 사용자가 이전 이름으로 새 컨텍스트를 만들지 못하게 되는 문제를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="ec23a-190">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="ec23a-191">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ec23a-191">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="ec23a-192">AS에서 게이트웨이가 작업을 연결하거나 연결 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ec23a-192">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="ec23a-193">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ec23a-193">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="ec23a-194">ApiVersions, ApiReleases 및 ApiRevisions에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-194">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="ec23a-195">ServiceFabric 백 엔드에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-195">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="ec23a-196">Application Insights 로거에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-196">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="ec23a-197">'기본' SKU를 API Management 서비스의 유효한 SKU로 인식하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-197">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="ec23a-198">개인 CA가 발급한 인증서를 루트 또는 CA로 설치하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-198">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="ec23a-199">KeyVault 및 다중 프록시 호스트 이름을 통한 사용자 정의 SSL 인증서를 수락하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-199">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="ec23a-200">MSI ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="ec23a-200">Added support for MSI identity</span></span>
* <span data-ttu-id="ec23a-201">URL을 통한 정책을 수락하는 지원 추가됨 참고: 다음 cmdlet은 이후 릴리스에서 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ec23a-201">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="ec23a-202">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="ec23a-202">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="ec23a-203">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec23a-203">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="ec23a-204">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="ec23a-204">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="ec23a-205">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="ec23a-205">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="ec23a-206">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="ec23a-206">AzureRM.Batch</span></span>
* <span data-ttu-id="ec23a-207">새 cmdlet Get AzureBatchPoolNodeCounts 릴리스</span><span class="sxs-lookup"><span data-stu-id="ec23a-207">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="ec23a-208">새 cmdlet Start-AzureBatchComputeNodeServiceLogUpload 릴리스</span><span class="sxs-lookup"><span data-stu-id="ec23a-208">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="ec23a-209">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="ec23a-209">AzureRM.Consumption</span></span>
* <span data-ttu-id="ec23a-210">Expand, ResourceGroup, InstanceName, InstanceId, Tags, Top on Cmdlet Get-AzureRmConsumptionUsageDetail 등 새 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="ec23a-210">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="ec23a-211">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ec23a-211">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="ec23a-212">Export-AzureRmDataLakeStoreChildItemProperties에 대한 예제 수정</span><span class="sxs-lookup"><span data-stu-id="ec23a-212">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="ec23a-213">Set-AzureRmDataLakeStoreItemAclEntry에서 재귀 사례에 대한 null 매개 변수 예외 수정</span><span class="sxs-lookup"><span data-stu-id="ec23a-213">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="ec23a-214">Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry에 대한 도움말 파일 수정</span><span class="sxs-lookup"><span data-stu-id="ec23a-214">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="ec23a-215">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="ec23a-215">AzureRM.Network</span></span>
* <span data-ttu-id="ec23a-216">18.0.0-preview에서 19.0.0-preview로 네트워크 SDK 버전 업그레이드</span><span class="sxs-lookup"><span data-stu-id="ec23a-216">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="ec23a-217">프로토콜 구성을 만들기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="ec23a-217">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="ec23a-218">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec23a-218">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="ec23a-219">기존 Express 경로 회로에 새 회로 연결을 추가하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="ec23a-219">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="ec23a-220">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="ec23a-220">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="ec23a-221">기존 Express 경로 회로에서 회로 연결을 제거하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="ec23a-221">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="ec23a-222">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="ec23a-222">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="ec23a-223">회로 연결을 검색하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="ec23a-223">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="ec23a-224">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="ec23a-224">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="ec23a-225">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ec23a-225">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="ec23a-226">생성된 인증서로 고정 서버 인증 사용(문제 # 5998)</span><span class="sxs-lookup"><span data-stu-id="ec23a-226">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="ec23a-227">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="ec23a-227">AzureRM.Sql</span></span>
* <span data-ttu-id="ec23a-228">AuditActions 또는 AuditActionGroups를 제거할 수 있도록 업데이트된 감사 cmdlet</span><span class="sxs-lookup"><span data-stu-id="ec23a-228">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="ec23a-229">'Azure 복구 서비스 자격 증명 모음을 사용하여 장기 보존 정책을 구성하면 정책이 더 이상 지원되지 않습니다. 새로운 유연 보유 정책으로 요청을 제출하십시오.'라는 메시지와 함께 명령이 실패하는 새로운 유연 보유 정책을 설정할 때</span><span class="sxs-lookup"><span data-stu-id="ec23a-229">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="ec23a-230">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy의 문제 수정</span><span class="sxs-lookup"><span data-stu-id="ec23a-230">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="ec23a-231">Azure SQL Database/ElasticPool Creation/Update 관련 cmdlet을 모두 업데이트하여 규모 및 계층 관련 속성에 대한 SKU 속성을 지원하는 새 데이터베이스 API를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="ec23a-231">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="ec23a-232">업데이트된 cmdlet는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="ec23a-232">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="ec23a-233">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="ec23a-233">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="ec23a-234">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="ec23a-234">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="ec23a-235">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="ec23a-235">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="ec23a-236">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="ec23a-236">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="ec23a-237">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="ec23a-237">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="ec23a-238">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ec23a-238">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="ec23a-239">-Name 매개 변수를 사용할 때 -ResourceGroupName 매개 변수가 필요하도록 'Get-AzureRmTrafficManagerProfile'에 대한 매개 변수를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="ec23a-239">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>