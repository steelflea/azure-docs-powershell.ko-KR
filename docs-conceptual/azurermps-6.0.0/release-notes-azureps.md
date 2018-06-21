---
title: Azure PowerShell 변경 로그 | Microsoft Docs
description: Azure PowerShell에 대한 최신 릴리스의 변경 내용입니다.
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 8515a267e80e5d1f7bb97557efa72b9e86b7b45d
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/08/2018
ms.locfileid: "33912006"
---
# <a name="release-notes"></a><span data-ttu-id="b3f7c-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="b3f7c-103">Release notes</span></span>

<span data-ttu-id="b3f7c-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---

## <a name="600---may-2018"></a><span data-ttu-id="b3f7c-105">6.0.0 - 2018년 5월</span><span class="sxs-lookup"><span data-stu-id="b3f7c-105">6.0.0 - May 2018</span></span>

### <a name="general"></a><span data-ttu-id="b3f7c-106">일반</span><span class="sxs-lookup"><span data-stu-id="b3f7c-106">General</span></span>
* <span data-ttu-id="b3f7c-107">모듈의 최소 종속성이 PowerShell 5.0으로 설정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-107">Set minimum dependency of modules to PowerShell 5.0</span></span>

### <a name="azurestorage"></a><span data-ttu-id="b3f7c-108">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="b3f7c-108">Azure.Storage</span></span>
* <span data-ttu-id="b3f7c-109">Storage Blob 컨테이너 이름으로 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-109">Support  as Storage blob container name</span></span>
    - <span data-ttu-id="b3f7c-110">New-AzureStorageBlobContainer</span><span class="sxs-lookup"><span data-stu-id="b3f7c-110">New-AzureStorageBlobContainer</span></span>
    - <span data-ttu-id="b3f7c-111">Remove-AzureStorageBlobContainer</span><span class="sxs-lookup"><span data-stu-id="b3f7c-111">Remove-AzureStorageBlobContainer</span></span>
    - <span data-ttu-id="b3f7c-112">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="b3f7c-112">Set-AzureStorageBlobContent</span></span>
    - <span data-ttu-id="b3f7c-113">Get-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="b3f7c-113">Get-AzureStorageBlobContent</span></span>
* <span data-ttu-id="b3f7c-114">일부 Storage cmdlet 실패 출력에 오류 세부 정보가 포함되지 않는 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-114">Fix the issue that some Storage cmdlets failure output not contain detail failure information</span></span>

### <a name="azurermapimanagement"></a><span data-ttu-id="b3f7c-115">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="b3f7c-115">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="b3f7c-116">여러 가지 주요 변경이 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-116">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="b3f7c-117">자세한 내용은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-117">Please refer to the migration guide for more information</span></span>

### <a name="azurermautomation"></a><span data-ttu-id="b3f7c-118">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="b3f7c-118">AzureRM.Automation</span></span>
* <span data-ttu-id="b3f7c-119">다음 cmdlet에서 사용되지 않는 'Tags' 별칭이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-119">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="b3f7c-120">'Set-AzureRmAutomationRunbook'</span><span class="sxs-lookup"><span data-stu-id="b3f7c-120">'Set-AzureRmAutomationRunbook'</span></span>

### <a name="azurermbatch"></a><span data-ttu-id="b3f7c-121">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="b3f7c-121">AzureRM.Batch</span></span>
* <span data-ttu-id="b3f7c-122">사용되지 않는 예제를 제거하도록 New-AzureBatchPool 설명서가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-122">Updated New-AzureBatchPool documentation to remove deprecated example</span></span>

### <a name="azurermcdn"></a><span data-ttu-id="b3f7c-123">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="b3f7c-123">AzureRM.Cdn</span></span>
* <span data-ttu-id="b3f7c-124">여러 가지 주요 변경이 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-124">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="b3f7c-125">자세한 내용은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-125">Please refer to the migration guide for more information</span></span>

### <a name="azurermcompute"></a><span data-ttu-id="b3f7c-126">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="b3f7c-126">AzureRM.Compute</span></span>
* <span data-ttu-id="b3f7c-127">'New-AzureRmVm'과 'New-AzureRmVmss'에서 매개 변수의 자세한 정보 출력을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-127">'New-AzureRmVm' and 'New-AzureRmVmss' support verbose output of parameters</span></span>
* <span data-ttu-id="b3f7c-128">'New-AzureRmVm' 및 'New-AzureRmVmss'(단순 매개 변수 집합)에서 사용자 정의 및(또는) 시스템 정의 ID를 VM에 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-128">'New-AzureRmVm' and 'New-AzureRmVmss' (simple parameter set) support assigning user defined and(or) system defined identities to the VM(s).</span></span>
* <span data-ttu-id="b3f7c-129">VMSS 재배포 및 PerformMaintenance 기능</span><span class="sxs-lookup"><span data-stu-id="b3f7c-129">VMSS Redeploy and PerformMaintenance feature</span></span>
    -  <span data-ttu-id="b3f7c-130">새 스위치 매개 변수(-Redeploy 및 -PerformMaintenance)가 'Set-AzureRmVmss' 및 'Set-AzureRmVmssVM'에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-130">Add new switch parameter -Redeploy and -PerformMaintenance to 'Set-AzureRmVmss' and 'Set-AzureRmVmssVM'</span></span>
* <span data-ttu-id="b3f7c-131">DisableVMAgent 스위치 매개 변수가 'Set-AzureRmVMOperatingSystem' cmdlet에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-131">Add DisableVMAgent switch parameter to 'Set-AzureRmVMOperatingSystem' cmdlet</span></span>
* <span data-ttu-id="b3f7c-132">'New-AzureRmVm'과 'New-AzureRmVmss'(단순 매개 변수 집합)에서 'Win10' 이미지를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-132">'New-AzureRmVm' and 'New-AzureRmVmss' (simple parameter set) support a 'Win10' image.</span></span>
* <span data-ttu-id="b3f7c-133">'Repair-AzureRmVmssServiceFabricUpdateDomain' cmdlet이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-133">'Repair-AzureRmVmssServiceFabricUpdateDomain' cmdlet is added.</span></span>
* <span data-ttu-id="b3f7c-134">여러 가지 주요 변경이 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-134">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="b3f7c-135">자세한 내용은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-135">Please refer to the migration guide for more details</span></span>
* <span data-ttu-id="b3f7c-136">'Set-AzureRmVmDiskEncryptionExtension'에서 AAD 매개 변수를 선택적으로 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-136">'Set-AzureRmVmDiskEncryptionExtension' makes AAD parameters optional</span></span>

### <a name="azurermdatafactories"></a><span data-ttu-id="b3f7c-137">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="b3f7c-137">AzureRM.DataFactories</span></span>
* <span data-ttu-id="b3f7c-138">다음 cmdlet에서 사용되지 않는 'Tags' 별칭이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-138">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="b3f7c-139">New-AzureRmDataFactory</span><span class="sxs-lookup"><span data-stu-id="b3f7c-139">New-AzureRmDataFactory</span></span>

### <a name="azurermdatafactoryv2"></a><span data-ttu-id="b3f7c-140">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="b3f7c-140">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="b3f7c-141">ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.7.0-preview로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-141">Updated the ADF .Net SDK version to 0.7.0-preview containing following changes:</span></span>
    - <span data-ttu-id="b3f7c-142">ExecuteSSISPackage 활동에 실행 매개 변수 및 연결 관리자 속성이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-142">Added execution parameters and connection managers property on ExecuteSSISPackage Activity</span></span>
    - <span data-ttu-id="b3f7c-143">PostgreSql, MySql 연결된 서비스에서 서버, 데이터베이스, 스키마, 사용자 이름 및 암호 대신 전체 연결 문자열을 사용하도록 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-143">Updated PostgreSql, MySql llinked service to use full connection string instead of server, database, schema, username and password</span></span>
    - <span data-ttu-id="b3f7c-144">DB2 연결된 서비스에서 스키마가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-144">Removed the schema from DB2 linked service</span></span>
    - <span data-ttu-id="b3f7c-145">Teradata 연결된 서비스에서 스키마 속성이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-145">Removed schema property from Teradata linked service</span></span>
    - <span data-ttu-id="b3f7c-146">Responsys에 대한 LinkedService, Dataset, CopySource가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-146">Added LinkedService, Dataset, CopySource for Responsys</span></span>

### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="b3f7c-147">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="b3f7c-147">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="b3f7c-148">다음 cmdlet에서 사용되지 않는 'Tags' 별칭이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-148">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="b3f7c-149">'New-AzureRmDataLakeAnalyticsAccount'</span><span class="sxs-lookup"><span data-stu-id="b3f7c-149">'New-AzureRmDataLakeAnalyticsAccount'</span></span>
    - <span data-ttu-id="b3f7c-150">'Set-AzureRmDataLakeAnalyticsAccount'</span><span class="sxs-lookup"><span data-stu-id="b3f7c-150">'Set-AzureRmDataLakeAnalyticsAccount'</span></span>

### <a name="azurermdatalakestore"></a><span data-ttu-id="b3f7c-151">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b3f7c-151">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="b3f7c-152">재귀적 Acl 변경에 대한 새 기능이 Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-152">Add new feature of recursive Acl Change to Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="b3f7c-153">디렉터리 아래에서 콘텐츠 요약을 검색하는 새 cmdlet이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-153">Add new cmdlet for retrieving the content summary under a directory</span></span>
* <span data-ttu-id="b3f7c-154">디스크 사용 및 Acl 덤프를 검색하는 새 cmdlet이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-154">Add new cmdlet for retrieving the disk usage and Acl dump</span></span>
* <span data-ttu-id="b3f7c-155">Set-AzureRmDataLakeStoreItemAcl 부울의 반환 형식이 IEnumerable<DataLakeStoreItemAce>로 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-155">Correct return type of Set-AzureRmDataLakeStoreItemAcl bool to IEnumerable<DataLakeStoreItemAce></span></span>
* <span data-ttu-id="b3f7c-156">Set-AzureRmDataLakeStoreItemAclEntry 부울의 반환 형식이 IEnumerable<DataLakeStoreItemAce>로 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-156">Correct return type of Set-AzureRmDataLakeStoreItemAclEntry bool to IEnumerable<DataLakeStoreItemAce></span></span>
* <span data-ttu-id="b3f7c-157">Export-AzureRmDataLakeStoreItem, Import-AzureRmDataLakeStoreItem, Remove-AzureRmDataLakeStoreItem이 크게 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-157">Breaking changes in Export-AzureRmDataLakeStoreItem, Import-AzureRmDataLakeStoreItem, Remove-AzureRmDataLakeStoreItem</span></span>

### <a name="azurermdns"></a><span data-ttu-id="b3f7c-158">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="b3f7c-158">AzureRM.Dns</span></span>
* <span data-ttu-id="b3f7c-159">여러 가지 주요 변경이 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-159">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="b3f7c-160">자세한 내용은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-160">Please refer to the migration guide for more information</span></span>

### <a name="azurermeventhub"></a><span data-ttu-id="b3f7c-161">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="b3f7c-161">AzureRM.EventHub</span></span>
* <span data-ttu-id="b3f7c-162">누락된 예제가 있는 cmdlet에 대한 도움말이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-162">Updated Help for cmdlets with missing examples</span></span>

### <a name="azurerminsights"></a><span data-ttu-id="b3f7c-163">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="b3f7c-163">AzureRM.Insights</span></span>
* <span data-ttu-id="b3f7c-164">여러 가지 주요 변경이 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-164">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="b3f7c-165">자세한 내용은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-165">Please refer to the migration guide for more information</span></span>

### <a name="azurermiothub"></a><span data-ttu-id="b3f7c-166">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="b3f7c-166">AzureRM.IotHub</span></span>
* <span data-ttu-id="b3f7c-167">IotHub에서 태그 및 기본 SKU를 사용하도록 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-167">Enable tags and Basic Sku to the IotHub</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="b3f7c-168">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="b3f7c-168">AzureRM.KeyVault</span></span>
* <span data-ttu-id="b3f7c-169">파이핑 시나리오를 지원하도록 크게 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-169">Breaking changes to support piping scenarios</span></span>
* <span data-ttu-id="b3f7c-170">추가된 새 cmdlet: Backup/Restore-AzureKeyVaultManagedStorageAccount, Backup/Restore-AzureKeyVaultCertificate, Undo-AzureKeyVaultManagedStorageSasDefinitionRemoval 및 Undo-AzureKeyVaultManagedStorageAccountRemoval</span><span class="sxs-lookup"><span data-stu-id="b3f7c-170">Added new cmdlets: Backup/Restore-AzureKeyVaultManagedStorageAccount, Backup/Restore-AzureKeyVaultCertificate, Undo-AzureKeyVaultManagedStorageSasDefinitionRemoval, and Undo-AzureKeyVaultManagedStorageAccountRemoval</span></span>

### <a name="azurermmachinelearning"></a><span data-ttu-id="b3f7c-171">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="b3f7c-171">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="b3f7c-172">다음 cmdlet에서 사용되지 않는 'Tags' 별칭이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-172">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="b3f7c-173">Update-AzureRmMlCommitmentPlan</span><span class="sxs-lookup"><span data-stu-id="b3f7c-173">Update-AzureRmMlCommitmentPlan</span></span>

### <a name="azurermmedia"></a><span data-ttu-id="b3f7c-174">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="b3f7c-174">AzureRM.Media</span></span>
* <span data-ttu-id="b3f7c-175">다음 cmdlet에서 사용되지 않는 'Tags' 별칭이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-175">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="b3f7c-176">'Set-AzureRmMediaService'</span><span class="sxs-lookup"><span data-stu-id="b3f7c-176">'Set-AzureRmMediaService'</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="b3f7c-177">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="b3f7c-177">AzureRM.Network</span></span>
* <span data-ttu-id="b3f7c-178">DDoS 보호 계획 리소스에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-178">Add support for DDoS protection plan resource</span></span>
* <span data-ttu-id="b3f7c-179">여러 가지 주요 변경이 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-179">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="b3f7c-180">자세한 내용은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-180">Please refer to the migration guide for more information</span></span>

### <a name="azurermnotificationhubs"></a><span data-ttu-id="b3f7c-181">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="b3f7c-181">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="b3f7c-182">여러 가지 주요 변경이 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-182">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="b3f7c-183">자세한 내용은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-183">Please refer to the migration guide for more information</span></span>

### <a name="azurermoperationalinsights"></a><span data-ttu-id="b3f7c-184">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="b3f7c-184">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="b3f7c-185">여러 가지 주요 변경이 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-185">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="b3f7c-186">자세한 내용은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-186">Please refer to the migration guide for more information</span></span>

### <a name="azurermprofile"></a><span data-ttu-id="b3f7c-187">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="b3f7c-187">AzureRM.Profile</span></span>
* <span data-ttu-id="b3f7c-188">기본적으로 컨텍스트 자동 저장을 사용하도록 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-188">Enable context autosave by default</span></span>
* <span data-ttu-id="b3f7c-189">미국 정부를 위한 Azure 환경에 USGovernmentOperationalInsightsEndpoint 및 USGovernmentOperationalInsightsEndpointResourceId 속성이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-189">Add USGovernmentOperationalInsightsEndpoint and USGovernmentOperationalInsightsEndpointResourceId properties to Azure environment for US Gov.</span></span>

### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="b3f7c-190">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="b3f7c-190">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="b3f7c-191">SiteRecovery 시나리오의 인증 헤더가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-191">Fixed Authentication Header in SiteRecovery scenarios</span></span>

### <a name="azurermrediscache"></a><span data-ttu-id="b3f7c-192">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="b3f7c-192">AzureRM.RedisCache</span></span>
* <span data-ttu-id="b3f7c-193">여러 가지 주요 변경이 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-193">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="b3f7c-194">자세한 내용은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-194">Please refer to the migration guide for more information</span></span>

### <a name="azurermresources"></a><span data-ttu-id="b3f7c-195">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="b3f7c-195">AzureRM.Resources</span></span>
* <span data-ttu-id="b3f7c-196">Get-AzureRmRoledefinition 호출에서 사용되지 않는 -AtScopeAndBelow 매개 변수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-196">Remove obsolete parameter -AtScopeAndBelow from Get-AzureRmRoledefinition call</span></span>
* <span data-ttu-id="b3f7c-197">삭제된 USers/Groups/ServicePrincipals에 대한 할당이 Get-AzureRmRoleAssignment 결과에 포함되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-197">Include assignments to deleted USers/Groups/ServicePrincipals in Get-AzureRmRoleAssignment result</span></span>
* <span data-ttu-id="b3f7c-198">Scope 및 ResourceType에 대한 Tab 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-198">Add Tab completers for Scope and ResourceType</span></span>
* <span data-ttu-id="b3f7c-199">ServicePrincipals를 만드는 편리한 cmdlet이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-199">Add convenience cmdlet for creating ServicePrincipals</span></span>
* <span data-ttu-id="b3f7c-200">Get-AzureRmResource에서 Get- 및 Find- 기능이 병합되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-200">Merge Get- and Find- functionality in Get-AzureRmResource</span></span>
* <span data-ttu-id="b3f7c-201">추가된 AD cmdlet:</span><span class="sxs-lookup"><span data-stu-id="b3f7c-201">Add AD Cmdlets:</span></span>
  - <span data-ttu-id="b3f7c-202">Remove-AzureRmADGroupMember</span><span class="sxs-lookup"><span data-stu-id="b3f7c-202">Remove-AzureRmADGroupMember</span></span>
  - <span data-ttu-id="b3f7c-203">Get-AzureRmADGroup</span><span class="sxs-lookup"><span data-stu-id="b3f7c-203">Get-AzureRmADGroup</span></span>
  - <span data-ttu-id="b3f7c-204">New-AzureRmADGroup</span><span class="sxs-lookup"><span data-stu-id="b3f7c-204">New-AzureRmADGroup</span></span>
  - <span data-ttu-id="b3f7c-205">Remove-AzureRmADGroup</span><span class="sxs-lookup"><span data-stu-id="b3f7c-205">Remove-AzureRmADGroup</span></span>
  - <span data-ttu-id="b3f7c-206">Remove-AzureRmADUser</span><span class="sxs-lookup"><span data-stu-id="b3f7c-206">Remove-AzureRmADUser</span></span>
  - <span data-ttu-id="b3f7c-207">Update-AzureRmADApplication</span><span class="sxs-lookup"><span data-stu-id="b3f7c-207">Update-AzureRmADApplication</span></span>
  - <span data-ttu-id="b3f7c-208">Update-AzureRmADServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="b3f7c-208">Update-AzureRmADServicePrincipal</span></span>
  - <span data-ttu-id="b3f7c-209">Update-AzureRmADUser</span><span class="sxs-lookup"><span data-stu-id="b3f7c-209">Update-AzureRmADUser</span></span>

### <a name="azurermservicefabric"></a><span data-ttu-id="b3f7c-210">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b3f7c-210">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="b3f7c-211">기본 Linux 이미지 버전 SKU가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-211">Update default Linux image version sku</span></span>
  - <span data-ttu-id="b3f7c-212">NewAzureServiceFabricCluster.cs 기본 UbuntuServer1604 SKU가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-212">NewAzureServiceFabricCluster.cs default UbuntuServer1604 Sku update</span></span>

### <a name="azurermstorage"></a><span data-ttu-id="b3f7c-213">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="b3f7c-213">AzureRM.Storage</span></span>
* <span data-ttu-id="b3f7c-214">여러 가지 주요 변경이 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-214">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="b3f7c-215">자세한 내용은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-215">Please refer to the migration guide for more information</span></span>

### <a name="azurermwebsites"></a><span data-ttu-id="b3f7c-216">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="b3f7c-216">AzureRM.Websites</span></span>
* <span data-ttu-id="b3f7c-217">최신 버전의 Websites SDK로 업그레이드되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-217">Upgrade to latest version of the Websites SDK</span></span>
* <span data-ttu-id="b3f7c-218">Set-AzureRmWebApp 및 Set-AzureRmWebAppSlot에 대한 -AssignIdentity 및 -Httpsonly 속성이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-218">Added -AssignIdentity & -Httpsonly properties for Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
* <span data-ttu-id="b3f7c-219">추가된 새 cmdlet: Get-AzureRmWebAppSnapshots 및 Restore-AzureRmWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="b3f7c-219">Added two new cmdlets: Get-AzureRmWebAppSnapshots and Restore-AzureRmWebAppSnapshot</span></span>
