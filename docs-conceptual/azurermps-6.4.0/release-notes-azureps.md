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
ms.openlocfilehash: 255e26aea5ea3cea866faa0d095cdf643c8ef0a8
ms.sourcegitcommit: de0e60800df1add9f3400166faacca202ef567d9
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2018
ms.locfileid: "37406486"
---
# <a name="release-notes"></a><span data-ttu-id="30c47-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="30c47-103">Release notes</span></span>

<span data-ttu-id="30c47-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="640---july-2018"></a><span data-ttu-id="30c47-105">6.4.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="30c47-105">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="30c47-106">일반</span><span class="sxs-lookup"><span data-stu-id="30c47-106">General</span></span>
* <span data-ttu-id="30c47-107">대부분의 모듈에 대한 도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="30c47-107">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="30c47-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="30c47-108">AzureRM.Profile</span></span>
* <span data-ttu-id="30c47-109">기본 출력 형식에 추가된 Ps1Xml 특성</span><span class="sxs-lookup"><span data-stu-id="30c47-109">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="30c47-110">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="30c47-110">AzureRM.Compute</span></span>
* <span data-ttu-id="30c47-111">VMSS에 대한 IP 태그 기능</span><span class="sxs-lookup"><span data-stu-id="30c47-111">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="30c47-112">'New-AzureRmVmssIpTagConfig' cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-112">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="30c47-113">New-AzureRmVmssIpConfig에 IpTag 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="30c47-113">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="30c47-114">VMSS에 대한 자동 OS 롤백 기능</span><span class="sxs-lookup"><span data-stu-id="30c47-114">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="30c47-115">New-AzureRmVmssConfig 및 Update-AzureRmVmss에 DisableAutoRollback 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="30c47-115">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="30c47-116">Vmss에 대한 OS 업그레이드 기록 기능</span><span class="sxs-lookup"><span data-stu-id="30c47-116">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="30c47-117">Get-AzureRmVmss에 OSUpgradeHistory 스위치 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-117">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="30c47-118">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="30c47-118">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="30c47-119">다음 명령을 통해 카탈로그 액세스 제어 목록에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-119">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="30c47-120">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="30c47-120">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="30c47-121">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="30c47-121">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="30c47-122">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="30c47-122">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="30c47-123">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="30c47-123">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="30c47-124">Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl에 대한 취소 지원 및 진행률 추적 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-124">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="30c47-125">Export-AzureRmDataLakeStoreChildItemProperties에 대한 취소 지원 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-125">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="30c47-126">재귀 작업을 수행하는 cmdlet에 대한 디버그 메시지 플러시 수정</span><span class="sxs-lookup"><span data-stu-id="30c47-126">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="30c47-127">DataLake cmdlet의 테스트 위치 수정</span><span class="sxs-lookup"><span data-stu-id="30c47-127">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="30c47-128">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="30c47-128">AzureRM.EventHub</span></span>
* <span data-ttu-id="30c47-129">목록 작업 cmdlet Get-AzureRmEventHub 및 Get-AzureRmEventHubConsumerGroup에 선택적 MaxCount 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-129">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="30c47-130">새 EventHub 만드는 동안 하나 이상의 매개 변수가 필요한 New-AzureRmEventHub cmdlet 문제를 해결.</span><span class="sxs-lookup"><span data-stu-id="30c47-130">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="30c47-131">기본 매개 변수 집합을 제공.</span><span class="sxs-lookup"><span data-stu-id="30c47-131">Provided Default Parameter set.</span></span>
* <span data-ttu-id="30c47-132">선택적 매개 변수 -KeyValue를 New-AzureRmEventHubKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-132">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="30c47-133">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="30c47-133">AzureRM.KeyVault</span></span>
* <span data-ttu-id="30c47-134">Get-AzureRmKeyVault -Tag 실행 시 모든 리소스가 리턴되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="30c47-134">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="30c47-135">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="30c47-135">AzureRM.Network</span></span>
* <span data-ttu-id="30c47-136">영역 중복 VirtualNetworkGateways에 대한 새 Sku를 노출합니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-136">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="30c47-137">기능에 대한 새 명령이 추가됨: ARM을 통한 ExpressRoute Partner APIs</span><span class="sxs-lookup"><span data-stu-id="30c47-137">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="30c47-138">Get- AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-138">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="30c47-139">Set-AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-139">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="30c47-140">Add-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-140">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="30c47-141">Get-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-141">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="30c47-142">Remove-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-142">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="30c47-143">Get-AzureRMExpressRouteCrossConnectionArpTable 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-143">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="30c47-144">Get-AzureRMExpressRouteCrossConnectionRouteTable 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-144">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="30c47-145">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-145">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="30c47-146">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="30c47-146">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="30c47-147">Get-AzureRmRecoveryServicesBackupStatus cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-147">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="30c47-148">이 cmdlet은 VM ID를 가져와서 VM이 구독에서 일부 자격 증명 모음으로 보호되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-148">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="30c47-149">이러한 자격 증명 모음이 존재하는 경우 cmdlet은 자격 증명 모음 세부 정보를 출력 합니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-149">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="30c47-150">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="30c47-150">AzureRM.Resources</span></span>
* <span data-ttu-id="30c47-151">Get-AzureRmPolicyAssignment cmdlet을 다음과 같이 업데이트함.</span><span class="sxs-lookup"><span data-stu-id="30c47-151">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="30c47-152">관리 그룹 수준에서 -Scope 값 리스팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-152">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="30c47-153">관리 그룹 수준에서 -Scope 값을 사용하여 개별 할당값을 검색하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-153">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="30c47-154">제어 매개 변수에 -Effective 및 -All 스위치 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-154">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="30c47-155">Get/New/Remove/Set-AzureRmPolicyDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="30c47-155">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="30c47-156">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-156">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="30c47-157">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-157">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="30c47-158">Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="30c47-158">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="30c47-159">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-159">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="30c47-160">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-160">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="30c47-161">'New-AzureRmResourceGroupDeployment'에서 'TemplateParameterObject'를 사용하는 경우 매개 변수에 KeyVault 비밀 참조 지원 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-161">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="30c47-162">'New-AzureRmADAppCredential'에 대해 '-EndDate' 매개 변수가 무시되는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="30c47-162">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="30c47-163">'Add-AzureRmADGroupMember'가 요청에 잘못된 URL을 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="30c47-163">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="30c47-164">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="30c47-164">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="30c47-165">선택적 매개 변수 -KeyValue를 New-AzureRmServiceBusKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-165">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="30c47-166">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="30c47-166">AzureRM.Sql</span></span>
* <span data-ttu-id="30c47-167">New-AzureRmSqlDatabaseRestorePoint 도움말에서 SQLDW에 대한 사용자 정의 복원 지점 명시</span><span class="sxs-lookup"><span data-stu-id="30c47-167">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="30c47-168">몇 가지 cmdlet에서-ComputeGeneration 매개 변수의 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="30c47-168">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="30c47-169">6.3.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="30c47-169">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="30c47-170">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="30c47-170">AzureRM.Profile</span></span>
* <span data-ttu-id="30c47-171">Enable-AzureRmContextAutoSave에 대한 오류 메시지 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="30c47-171">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="30c47-172">이전 컨텍스트 없이 'Connect-AzureRmAccount' 실행 시 각 구독에 대한 컨텍스트 생성</span><span class="sxs-lookup"><span data-stu-id="30c47-172">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="30c47-173">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="30c47-173">Azure.Storage</span></span>
* <span data-ttu-id="30c47-174">도움말 파일 내 -Permissions 매개 변수에 대한 추가 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="30c47-174">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="30c47-175">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="30c47-175">AzureRM.Compute</span></span>
* <span data-ttu-id="30c47-176">'Get-AzureRmVmDiskEncryptionStatus'가 데이터 디스크가 없는 VM에 대해 관찰된 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="30c47-176">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="30c47-177">Compute 클라이언트 라이브러리 버전을 업데이트하여 다음 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="30c47-177">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="30c47-178">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="30c47-178">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="30c47-179">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="30c47-179">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="30c47-180">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="30c47-180">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="30c47-181">다음 cmdlet이 '작업 ID' 및 '작업 상태'를 올바르게 표시하도록 수정:</span><span class="sxs-lookup"><span data-stu-id="30c47-181">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="30c47-182">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="30c47-182">Start-AzureRmVM</span></span>
    - <span data-ttu-id="30c47-183">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="30c47-183">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="30c47-184">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="30c47-184">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="30c47-185">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="30c47-185">Set-AzureRmVM</span></span>
    - <span data-ttu-id="30c47-186">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="30c47-186">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="30c47-187">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="30c47-187">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="30c47-188">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="30c47-188">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="30c47-189">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="30c47-189">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="30c47-190">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="30c47-190">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="30c47-191">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="30c47-191">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="30c47-192">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="30c47-192">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="30c47-193">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="30c47-193">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="30c47-194">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="30c47-194">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="30c47-195">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="30c47-195">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="30c47-196">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="30c47-196">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="30c47-197">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="30c47-197">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="30c47-198">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="30c47-198">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="30c47-199">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="30c47-199">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="30c47-200">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="30c47-200">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="30c47-201">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="30c47-201">AzureRM.EventGrid</span></span>
* <span data-ttu-id="30c47-202">Update-AzureRmEventGridSubscription cmdlet의 SubjectBeginsWith/SubjectEndsWith에 대한 ValidateNotNullOrEmpty 유효성 검사 조건을 제거하여 필요에 따라 이러한 매개 변수를 빈 문자열로 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-202">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="30c47-203">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="30c47-203">AzureRM.KeyVault</span></span>
* <span data-ttu-id="30c47-204">Get-AzureRmKeyVault -Tag 실행 시 태그가 리턴되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="30c47-204">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="30c47-205">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="30c47-205">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="30c47-206">Policy Insights cmdlet의 공개 릴리스</span><span class="sxs-lookup"><span data-stu-id="30c47-206">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="30c47-207">API 버전 2018-04-04 사용</span><span class="sxs-lookup"><span data-stu-id="30c47-207">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="30c47-208">PolicyDefinitionReferenceId를 Get-AzureRmPolicyStateSummary의 결과 집합에 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-208">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="30c47-209">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="30c47-209">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="30c47-210">-Vault 매개 변수를 RecoveryServices.Backup cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="30c47-210">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="30c47-211">전달되는 경우 이는 Set-AzureRmRecoveryServicesContext cmdlet을 재정의함.</span><span class="sxs-lookup"><span data-stu-id="30c47-211">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="30c47-212">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="30c47-212">AzureRM.Sql</span></span>
* <span data-ttu-id="30c47-213">Get-AzureRmSqlDatabaseExpanded에 대한 도움말 파일의 예가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="30c47-213">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="30c47-214">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="30c47-214">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="30c47-215">Add-AzureRmTrafficManagerEndpointConfig에대한 도움말 파일이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="30c47-215">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="30c47-216">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="30c47-216">AzureRM.Websites</span></span>
* <span data-ttu-id="30c47-217">-AssignIdentity를 사용할 때 AppSetting을 덮어쓰지 않도록 'Set-AzureRmWebApp'이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="30c47-217">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="30c47-218">'New-AzureRmWebAppSlot'이 AppServicePlan을 옵션 매개변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="30c47-218">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="30c47-219">6.2.1 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="30c47-219">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="30c47-220">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="30c47-220">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="30c47-221">PSWorkspace 모델이 Network 형식을 매개 변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="30c47-221">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="30c47-222">6.2.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="30c47-222">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="30c47-223">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="30c47-223">AzureRM.Profile</span></span>
* <span data-ttu-id="30c47-224">Newtonsoft.Json의 버전 10.0.3이 모듈 가져오기에 로드되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="30c47-224">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="30c47-225">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="30c47-225">AzureRM.Compute</span></span>
* <span data-ttu-id="30c47-226">VMSS VM 업데이트 기능</span><span class="sxs-lookup"><span data-stu-id="30c47-226">VMSS VM Update feature</span></span>
    - <span data-ttu-id="30c47-227">'Update-AzureRmVmssVM' 및 'New-AzureRmVMDataDisk' cmdlets 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-227">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="30c47-228">데이터 디스크를 Vmss VM에 추가할 수 있도록 지원하기 위해 VirtualMachineScaleSetVM 매개변수를 'Add-AzureRmVMDataDisk' cmdlet에 추가하였습니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-228">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="30c47-229">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="30c47-229">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="30c47-230">ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.8.0-preview로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-230">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="30c47-231">팩터리 리포지토리 작업 구성 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-231">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="30c47-232">QuickBooks LinkedService가 ConsumerKey 및 consumerSecret 속성을 노출하도록 업데이트됨 </span><span class="sxs-lookup"><span data-stu-id="30c47-232">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="30c47-233">여러 모델 유형을 SecretBase에서 개체로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="30c47-233">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="30c47-234">Blob 이벤트 트리거 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-234">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="30c47-235">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="30c47-235">AzureRM.KeyVault</span></span>
* <span data-ttu-id="30c47-236">예제 출력으로 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="30c47-236">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="30c47-237">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="30c47-237">AzureRM.Network</span></span>
* <span data-ttu-id="30c47-238">Network Watcher cmdlet에서 트래픽 분석 매개 변수를 사용가능하도록 설정</span><span class="sxs-lookup"><span data-stu-id="30c47-238">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="30c47-239">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="30c47-239">AzureRM.Resources</span></span>
* <span data-ttu-id="30c47-240">'Get AzureRmResource'에서 반환된 'PSResource' 개체의 'Properties' 속성의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="30c47-240">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="30c47-241">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="30c47-241">AzureRM.Scheduler</span></span>
* <span data-ttu-id="30c47-242">ServiceBusQueueJob 업데이트가 새 인증 값을 설정하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="30c47-242">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="30c47-243">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="30c47-243">AzureRM.Sql</span></span>
* <span data-ttu-id="30c47-244">옵션 LicenseType 매개 변수를 사용하여 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="30c47-244">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="30c47-245">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="30c47-245">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="30c47-246">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="30c47-246">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="30c47-247">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="30c47-247">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="30c47-248">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="30c47-248">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="30c47-249">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="30c47-249">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="30c47-250">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="30c47-250">AzureRM.Websites</span></span>
* <span data-ttu-id="30c47-251">'New-AzureRMWebApp'이 전략 라이브러리의 공통 알고리즘을 사용하도록 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-251">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="30c47-252">6.1.0 - 2018년 5월</span><span class="sxs-lookup"><span data-stu-id="30c47-252">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="30c47-253">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="30c47-253">AzureRM.Profile</span></span>
* <span data-ttu-id="30c47-254">'Clear-AzureRmContext'를 실행하면 이전 기본 컨텍스트의 이름으로 빈 컨텍스트가 유지되어 사용자가 이전 이름으로 새 컨텍스트를 만들지 못하게 되는 문제를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-254">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="30c47-255">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="30c47-255">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="30c47-256">AS에서 게이트웨이가 작업을 연결하거나 연결 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-256">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="30c47-257">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="30c47-257">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="30c47-258">ApiVersions, ApiReleases 및 ApiRevisions에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="30c47-258">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="30c47-259">ServiceFabric 백 엔드에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="30c47-259">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="30c47-260">Application Insights 로거에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="30c47-260">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="30c47-261">'기본' SKU를 API Management 서비스의 유효한 SKU로 인식하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="30c47-261">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="30c47-262">개인 CA가 발급한 인증서를 루트 또는 CA로 설치하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="30c47-262">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="30c47-263">KeyVault 및 다중 프록시 호스트 이름을 통한 사용자 정의 SSL 인증서를 수락하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="30c47-263">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="30c47-264">MSI ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="30c47-264">Added support for MSI identity</span></span>
* <span data-ttu-id="30c47-265">URL을 통한 정책을 수락하는 지원 추가됨 참고: 다음 cmdlet은 이후 릴리스에서 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-265">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="30c47-266">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="30c47-266">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="30c47-267">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="30c47-267">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="30c47-268">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="30c47-268">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="30c47-269">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="30c47-269">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="30c47-270">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="30c47-270">AzureRM.Batch</span></span>
* <span data-ttu-id="30c47-271">새 cmdlet Get AzureBatchPoolNodeCounts 릴리스</span><span class="sxs-lookup"><span data-stu-id="30c47-271">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="30c47-272">새 cmdlet Start-AzureBatchComputeNodeServiceLogUpload 릴리스</span><span class="sxs-lookup"><span data-stu-id="30c47-272">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="30c47-273">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="30c47-273">AzureRM.Consumption</span></span>
* <span data-ttu-id="30c47-274">Expand, ResourceGroup, InstanceName, InstanceId, Tags, Top on Cmdlet Get-AzureRmConsumptionUsageDetail 등 새 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="30c47-274">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="30c47-275">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="30c47-275">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="30c47-276">Export-AzureRmDataLakeStoreChildItemProperties에 대한 예제 수정</span><span class="sxs-lookup"><span data-stu-id="30c47-276">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="30c47-277">Set-AzureRmDataLakeStoreItemAclEntry에서 재귀 사례에 대한 null 매개 변수 예외 수정</span><span class="sxs-lookup"><span data-stu-id="30c47-277">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="30c47-278">Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry에 대한 도움말 파일 수정</span><span class="sxs-lookup"><span data-stu-id="30c47-278">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="30c47-279">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="30c47-279">AzureRM.Network</span></span>
* <span data-ttu-id="30c47-280">18.0.0-preview에서 19.0.0-preview로 네트워크 SDK 버전 업그레이드</span><span class="sxs-lookup"><span data-stu-id="30c47-280">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="30c47-281">프로토콜 구성을 만들기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="30c47-281">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="30c47-282">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="30c47-282">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="30c47-283">기존 Express 경로 회로에 새 회로 연결을 추가하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="30c47-283">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="30c47-284">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="30c47-284">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="30c47-285">기존 Express 경로 회로에서 회로 연결을 제거하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="30c47-285">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="30c47-286">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="30c47-286">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="30c47-287">회로 연결을 검색하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="30c47-287">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="30c47-288">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="30c47-288">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="30c47-289">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="30c47-289">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="30c47-290">생성된 인증서로 고정 서버 인증 사용(문제 # 5998)</span><span class="sxs-lookup"><span data-stu-id="30c47-290">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="30c47-291">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="30c47-291">AzureRM.Sql</span></span>
* <span data-ttu-id="30c47-292">AuditActions 또는 AuditActionGroups를 제거할 수 있도록 업데이트된 감사 cmdlet</span><span class="sxs-lookup"><span data-stu-id="30c47-292">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="30c47-293">'Azure 복구 서비스 자격 증명 모음을 사용하여 장기 보존 정책을 구성하면 정책이 더 이상 지원되지 않습니다. 새로운 유연 보유 정책으로 요청을 제출하십시오.'라는 메시지와 함께 명령이 실패하는 새로운 유연 보유 정책을 설정할 때</span><span class="sxs-lookup"><span data-stu-id="30c47-293">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="30c47-294">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy의 문제 수정</span><span class="sxs-lookup"><span data-stu-id="30c47-294">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="30c47-295">Azure SQL Database/ElasticPool Creation/Update 관련 cmdlet을 모두 업데이트하여 규모 및 계층 관련 속성에 대한 SKU 속성을 지원하는 새 데이터베이스 API를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-295">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="30c47-296">업데이트된 cmdlet는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-296">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="30c47-297">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="30c47-297">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="30c47-298">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="30c47-298">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="30c47-299">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="30c47-299">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="30c47-300">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="30c47-300">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="30c47-301">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="30c47-301">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="30c47-302">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="30c47-302">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="30c47-303">-Name 매개 변수를 사용할 때 -ResourceGroupName 매개 변수가 필요하도록 'Get-AzureRmTrafficManagerProfile'에 대한 매개 변수를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="30c47-303">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>