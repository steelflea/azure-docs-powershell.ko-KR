---
title: "Azure PowerShell 변경 로그 | Microsoft Docs"
description: "Azure PowerShell에 대한 최신 릴리스의 변경 내용입니다."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-resource-manager
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: 
ms.date: 05/18/2017
ms.openlocfilehash: 5c8fa2a5a8f94cd24b66f42c237749a7b89af3b3
ms.sourcegitcommit: ec0b3565264ff7c9f03315ded182f3d5cce534fc
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/13/2017
---
# <a name="release-notes"></a><span data-ttu-id="689a5-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="689a5-103">Release notes</span></span>

<span data-ttu-id="689a5-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-400"></a><span data-ttu-id="689a5-105">버전 4.0.0</span><span class="sxs-lookup"><span data-stu-id="689a5-105">Version 4.0.0</span></span>

* <span data-ttu-id="689a5-106">이 릴리스에는 주요 변경 내용인 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-106">This release contains breaking changes.</span></span> <span data-ttu-id="689a5-107">변경 세부 정보 및 기존 스크립트에 미치는 영향에 대해서는 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="689a5-107">Please see [the migration guide](https://aka.ms/azps-migration-guide) for change details and the impact on existing scripts.</span></span>
* <span data-ttu-id="689a5-108">ApiManagement</span><span class="sxs-lookup"><span data-stu-id="689a5-108">ApiManagement</span></span>
  - <span data-ttu-id="689a5-109">New-AzureRmApiManagementGroup에서 기존 그룹을 구성하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-109">Added support for configuring external groups in New-AzureRmApiManagementGroup.</span></span>
* <span data-ttu-id="689a5-110">결제</span><span class="sxs-lookup"><span data-stu-id="689a5-110">Billing</span></span>
  - <span data-ttu-id="689a5-111">새 Cmdlet Get-AzureRmBillingPeriod</span><span class="sxs-lookup"><span data-stu-id="689a5-111">New Cmdlet Get-AzureRmBillingPeriod</span></span>
    + <span data-ttu-id="689a5-112">구독의 Azure 청구 기간을 검색하기 위한 cmdlet입니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-112">cmdlet to retrieve azure billing periods of the subscription.</span></span>
  - <span data-ttu-id="689a5-113">Cmdlet Get-AzureRmBillingInvoice 업데이트</span><span class="sxs-lookup"><span data-stu-id="689a5-113">Update Cmdlet Get-AzureRmBillingInvoice</span></span>
  - <span data-ttu-id="689a5-114">새 속성 BillingPeriodNames</span><span class="sxs-lookup"><span data-stu-id="689a5-114">new property BillingPeriodNames</span></span>
  - <span data-ttu-id="689a5-115">목록 보기에서 출력</span><span class="sxs-lookup"><span data-stu-id="689a5-115">output in list view</span></span>
* <span data-ttu-id="689a5-116">계산</span><span class="sxs-lookup"><span data-stu-id="689a5-116">Compute</span></span>
  - <span data-ttu-id="689a5-117">프리미엄 Managed Disks를 지원하도록 Set-AzureRmVMAEMExtension 및 Test-AzureRmVMAEMExtension cmdlet이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-117">Updated Set-AzureRmVMAEMExtension and Test-AzureRmVMAEMExtension cmdlets to support Premium managed disks</span></span>
  - <span data-ttu-id="689a5-118">IaaS VM에 대한 암호화 설정 백업 및 실패 시 복원</span><span class="sxs-lookup"><span data-stu-id="689a5-118">Backup encryption settings for IaaS VMs and restore on failure</span></span>
  - <span data-ttu-id="689a5-119">ChefServiceInterval 옵션 이름이 ChefDaemonInterval로 바뀌었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-119">ChefServiceInterval option is renamed to ChefDaemonInterval now.</span></span> <span data-ttu-id="689a5-120">그렇지만 이전 이름도 계속 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-120">Old one will continue to work however.</span></span>
  - <span data-ttu-id="689a5-121">PS VM 개체에서 중복된 DataDiskNames 및 NetworkInterfaceIDs 속성을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-121">Remove duplicated DataDiskNames and NetworkInterfaceIDs properties from PS VM object.</span></span>
  - <span data-ttu-id="689a5-122">DataDiskNames 및 NetworkInterfaceIDs 매개 변수를 Remove-AzureRmVMDataDisk 및 Remove-AzureRmVMNetworkInterface에서 각각 옵션으로 지정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-122">Make DataDiskNames and NetworkInterfaceIDs parameters optional in Remove-AzureRmVMDataDisk and Remove-AzureRmVMNetworkInterface, respectively.</span></span>
  - <span data-ttu-id="689a5-123">Get cmdlet이 목록 개체를 반환하는 경우 Get cmdlet의 파이핑 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-123">Fix the piping issue of Get cmdlets when the Get cmdlets return a list object.</span></span>
  - <span data-ttu-id="689a5-124">RDFE cmdlet과 충돌하는 Cmdlet 이름이 바뀌었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-124">Cmdlets that conflicted with RDFE cmdlets have been renamed.</span></span> <span data-ttu-id="689a5-125">자세한 내용은 문제 https://github.com/Azure/azure-powershell/issues/2917을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="689a5-125">See issue https://github.com/Azure/azure-powershell/issues/2917 for more details</span></span>
    + <span data-ttu-id="689a5-126">`New-AzureVMSqlServerAutoBackupConfig`는 `New-AzureRmVMSqlServerAutoBackupConfig`로 이름이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-126">`New-AzureVMSqlServerAutoBackupConfig` has been renamed to `New-AzureRmVMSqlServerAutoBackupConfig`</span></span>
    + <span data-ttu-id="689a5-127">`New-AzureVMSqlServerAutoPatchingConfig`는 `New-AzureRmVMSqlServerAutoPatchingConfig`로 이름이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-127">`New-AzureVMSqlServerAutoPatchingConfig` has been renamed to `New-AzureRmVMSqlServerAutoPatchingConfig`</span></span>
    + <span data-ttu-id="689a5-128">`New-AzureVMSqlServerKeyVaultCredentialConfig`는 `New-AzureRmVMSqlServerKeyVaultCredentialConfig`로 이름이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-128">`New-AzureVMSqlServerKeyVaultCredentialConfig` has been renamed to `New-AzureRmVMSqlServerKeyVaultCredentialConfig`</span></span>
* <span data-ttu-id="689a5-129">Consumption</span><span class="sxs-lookup"><span data-stu-id="689a5-129">Consumption</span></span>
  - <span data-ttu-id="689a5-130">새 Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="689a5-130">New Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>
    + <span data-ttu-id="689a5-131">구독의 사용량 세부 정보를 검색하기 위한 cmdlet입니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-131">cmdlet to retrieve usage details of the subscription.</span></span>
* <span data-ttu-id="689a5-132">ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="689a5-132">ContainerRegistry</span></span>
  - <span data-ttu-id="689a5-133">Azure Container Registry에 대한 PowerShell cmdlet이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-133">Add PowerShell cmdlets for Azure Container Registry</span></span>
    + <span data-ttu-id="689a5-134">New-AzureRmContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="689a5-134">New-AzureRmContainerRegistry</span></span>
    + <span data-ttu-id="689a5-135">Get-AzureRmContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="689a5-135">Get-AzureRmContainerRegistry</span></span>
    + <span data-ttu-id="689a5-136">Update-AzureRmContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="689a5-136">Update-AzureRmContainerRegistry</span></span>
    + <span data-ttu-id="689a5-137">Remove-AzureRmContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="689a5-137">Remove-AzureRmContainerRegistry</span></span>
    + <span data-ttu-id="689a5-138">Get-AzureRmContainerRegistryCredential</span><span class="sxs-lookup"><span data-stu-id="689a5-138">Get-AzureRmContainerRegistryCredential</span></span>
    + <span data-ttu-id="689a5-139">Update-AzureRmContainerRegistryCredential</span><span class="sxs-lookup"><span data-stu-id="689a5-139">Update-AzureRmContainerRegistryCredential</span></span>
    + <span data-ttu-id="689a5-140">Test-AzureRmContainerRegistryNameAvailability</span><span class="sxs-lookup"><span data-stu-id="689a5-140">Test-AzureRmContainerRegistryNameAvailability</span></span>
* <span data-ttu-id="689a5-141">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="689a5-141">DataLakeAnalytics</span></span>
  - <span data-ttu-id="689a5-142">카탈로그 패키지 가져오기 및 나열에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="689a5-142">Add support for catalog package get and list</span></span>
  - <span data-ttu-id="689a5-143">좀 더 높은 수준의 상위 항목에서 다음 카탈로그 항목을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="689a5-143">Add support for listing the following catalog items from deeper ancestors:</span></span>
    + <span data-ttu-id="689a5-144">테이블</span><span class="sxs-lookup"><span data-stu-id="689a5-144">Table</span></span>
    + <span data-ttu-id="689a5-145">TVF</span><span class="sxs-lookup"><span data-stu-id="689a5-145">TVF</span></span>
    + <span data-ttu-id="689a5-146">보기</span><span class="sxs-lookup"><span data-stu-id="689a5-146">View</span></span>
    + <span data-ttu-id="689a5-147">통계</span><span class="sxs-lookup"><span data-stu-id="689a5-147">Statistics</span></span>
* <span data-ttu-id="689a5-148">DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="689a5-148">DataLakeStore</span></span>
  - <span data-ttu-id="689a5-149">`Import-AzureRMDataLakeStoreItem` 및 `Export-AzureRMDataLakeStoreItem`의 경우 성능 향상을 위해 추적 로깅이 기본적으로 사용되지 않도록 설정되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-149">For `Import-AzureRMDataLakeStoreItem` and `Export-AzureRMDataLakeStoreItem` trace logging has been disabled by default to improve performance.</span></span> <span data-ttu-id="689a5-150">추적 로깅이 필요한 경우 `-DiagnosticLogLevel` 및 `-DiagnosticLogPath` 매개 변수를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="689a5-150">If trace logging is desired please use the `-DiagnosticLogLevel` and `-DiagnosticLogPath` parameters</span></span>
  - <span data-ttu-id="689a5-151">ADLS에 많은 수의 작은 파일을 업로드하는 경우 때때로 PowerShell이 충돌하도록 하는 버그를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-151">Fixed a bug that would sometimes cause PowerShell to crash when uploading lots of small file to ADLS.</span></span>
* <span data-ttu-id="689a5-152">EventHub</span><span class="sxs-lookup"><span data-stu-id="689a5-152">EventHub</span></span>
  - <span data-ttu-id="689a5-153">버그 수정:</span><span class="sxs-lookup"><span data-stu-id="689a5-153">Bug fix :</span></span>
    + <span data-ttu-id="689a5-154">Set-AzureRmEventHubNamespace cmdlet 오류에 대한 수정 - 'Tier'가 'SkuName'이어야 하는 경우 null로 지정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-154">Fix for Set-AzureRmEventHubNamespace cmdlet error  - 'Tier' cannot be null, where it should be 'SkuName'</span></span>
    + <span data-ttu-id="689a5-155">Set-AzureRmEventHub - EventHub를 업데이트하는 동안 '개체 참조가 개체의 인스턴스로 설정되지 않았습니다.' 오류 수정</span><span class="sxs-lookup"><span data-stu-id="689a5-155">Set-AzureRmEventHub - Fix 'Object reference not set to an instance of an object' error while updating EventHub</span></span>
* <span data-ttu-id="689a5-156">자세한 정보</span><span class="sxs-lookup"><span data-stu-id="689a5-156">Insights</span></span>
  - <span data-ttu-id="689a5-157">Add-AzureRm*AlertRule</span><span class="sxs-lookup"><span data-stu-id="689a5-157">Add-AzureRm*AlertRule</span></span>
    + <span data-ttu-id="689a5-158">단일 개체 newResource, statusCode, requestId를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-158">Returns a single object: newResource, statusCode, requestId</span></span>
  - <span data-ttu-id="689a5-159">Get-AzureRmAlertRule</span><span class="sxs-lookup"><span data-stu-id="689a5-159">Get-AzureRmAlertRule</span></span>
    + <span data-ttu-id="689a5-160">이제 출력은 단일 개체로 간주되지 않고 열거됩니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-160">The output is now enumerated instead of considered a single object.</span></span> <span data-ttu-id="689a5-161">해당 형식은 변경되지 않았으므로 여전히 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-161">Its type did not change, it is still a list.</span></span>
  - <span data-ttu-id="689a5-162">Remove-AzureRmAlertRule</span><span class="sxs-lookup"><span data-stu-id="689a5-162">Remove-AzureRmAlertRule</span></span>
    + <span data-ttu-id="689a5-163">statusCode는 요청에 의해 반환된 상태 코드(항상 정상임)를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-163">The statusCode follows the status code returned by the request, before it was Ok always.</span></span>
  - <span data-ttu-id="689a5-164">Add-AzureRmAutoscaleSetting</span><span class="sxs-lookup"><span data-stu-id="689a5-164">Add-AzureRmAutoscaleSetting</span></span>
    + <span data-ttu-id="689a5-165">이제 statusCode, requestId 및 새로 생성/업데이트된 리소스를 포함하는 단일 개체(이전처럼 목록이 아님)를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-165">Returns now a single object (not a list as before) containing statusCode, requestId, and the newly created/updated resource.</span></span>
    + <span data-ttu-id="689a5-166">상태 코드는 요청에 의해 반환된 상태(항상 정상임)를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-166">The status code follows the status returned by the request, before it was always Ok.</span></span>
  - <span data-ttu-id="689a5-167">New-AzureRmAutoscaleRule</span><span class="sxs-lookup"><span data-stu-id="689a5-167">New-AzureRmAutoscaleRule</span></span>
    + <span data-ttu-id="689a5-168">매개 변수 ScaleActionType이 확장되었으며 이제 값 ChangeCount, PercentChangeCount, ExactCount를 수신합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-168">The parameter ScaleActionType has been extended, it receives the following values now: ChangeCount, PercentChangeCount, ExactCount.</span></span>
  - <span data-ttu-id="689a5-169">Remove-AzureRmAutoscaleSetting</span><span class="sxs-lookup"><span data-stu-id="689a5-169">Remove-AzureRmAutoscaleSetting</span></span>
    + <span data-ttu-id="689a5-170">출력의 statusCode는 요청에 의해 반환된 statusCode를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-170">The statusCode in the output follows the statusCode returned by the request.</span></span> <span data-ttu-id="689a5-171">이 코드가 이전에는 항상 정상이었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-171">Before it was always Ok.</span></span>
  - <span data-ttu-id="689a5-172">Get-AzureRMLogProfile</span><span class="sxs-lookup"><span data-stu-id="689a5-172">Get-AzureRMLogProfile</span></span>
    + <span data-ttu-id="689a5-173">이제 출력이 열거됩니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-173">The output is now enumerated.</span></span> <span data-ttu-id="689a5-174">이전에는 단일 개체로 간주되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-174">Before it was considered a single object.</span></span> <span data-ttu-id="689a5-175">출력의 형식은 이전처럼 목록으로 유지됩니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-175">The type of the output remains a list as before.</span></span>
  - <span data-ttu-id="689a5-176">Remove-AzureRmLogProfile</span><span class="sxs-lookup"><span data-stu-id="689a5-176">Remove-AzureRmLogProfile</span></span>
    + <span data-ttu-id="689a5-177">PassThru 매개 변수가 구현되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-177">The PassThru parameter has been implemented.</span></span>
  - <span data-ttu-id="689a5-178">Metrics API</span><span class="sxs-lookup"><span data-stu-id="689a5-178">Metrics API</span></span>
    + <span data-ttu-id="689a5-179">이 SDK는 이제 MDM에서 메트릭을 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-179">The SDK now retrieves metrics from MDM.</span></span>
  - <span data-ttu-id="689a5-180">Get-AzureRmMetricDefinition</span><span class="sxs-lookup"><span data-stu-id="689a5-180">Get-AzureRmMetricDefinition</span></span>
    + <span data-ttu-id="689a5-181">출력은 여전히 목록이지만 목록 구조가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-181">The output is still a list, but the structure of the list changed.</span></span>
  - <span data-ttu-id="689a5-182">Get-AzureRmMetric</span><span class="sxs-lookup"><span data-stu-id="689a5-182">Get-AzureRmMetric</span></span>
    + <span data-ttu-id="689a5-183">호출이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-183">The call has changed.</span></span> <span data-ttu-id="689a5-184">새 구문: Get-AzureRmMetric ResourceId [MetricNames [TimeGrain] [AggregationType] [StartTime] [EndTime]] [DetailedOutput]</span><span class="sxs-lookup"><span data-stu-id="689a5-184">This is the new syntax: Get-AzureRmMetric ResourceId [MetricNames [TimeGrain] [AggregationType] [StartTime] [EndTime]] [DetailedOutput]</span></span>
    + <span data-ttu-id="689a5-185">출력은 목록이며 해당 요소의 구조가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-185">The output is a list, and the structure of its elements has changed.</span></span>
* <span data-ttu-id="689a5-186">KeyVault</span><span class="sxs-lookup"><span data-stu-id="689a5-186">KeyVault</span></span>
  - <span data-ttu-id="689a5-187">KeyVault 비밀에 대한 백업/복원 지원 추가</span><span class="sxs-lookup"><span data-stu-id="689a5-187">Adding backup/restore support for KeyVault secrets</span></span>
    + <span data-ttu-id="689a5-188">비밀을 백업 및 복원할 수 있으며 키에 대해 현재 지원되는 기능과 일치합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-188">Secrets can be backed up and restored, matching the functionality currently supported for Keys</span></span>

  - <span data-ttu-id="689a5-189">키 및 비밀에 대한 백업 cmdlet은 이제 해당 개체를 입력 매개 변수로 수락합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-189">Backup cmdlets for Keys and Secrets now accept a corresponding object as an input parameter</span></span>
    + <span data-ttu-id="689a5-190">호출자는 검색 및 백업 작업을 연쇄적으로 진행할 수 있음: Get-AzureKeyVaultKey -VaultName myVault -Name myKey | Backup-AzureKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="689a5-190">The caller may chain retrieval and backup operations: Get-AzureKeyVaultKey -VaultName myVault -Name myKey | Backup-AzureKeyVaultKey</span></span>

  - <span data-ttu-id="689a5-191">이제 백업 cmdlet은 기존 파일을 덮어쓰기 위한 -Force 스위치를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-191">Backup cmdlets now support a -Force switch to overwrite an existing file</span></span>
    + <span data-ttu-id="689a5-192">기존 파일을 덮어쓰려고 해도 더 이상 오류가 throw되지 않으며 대신, 사용자에게 진행 방법을 선택하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-192">Note that attempting to overwrite an existing file will no longer throw, and will instead prompt the user for a choice on how to proceed.</span></span>
* <span data-ttu-id="689a5-193">LogicApp</span><span class="sxs-lookup"><span data-stu-id="689a5-193">LogicApp</span></span>
  - <span data-ttu-id="689a5-194">교환 컨트롤 번호 재해 복구 cmdlet에 대한 새 매개 변수:</span><span class="sxs-lookup"><span data-stu-id="689a5-194">New parameters for Interchange Control Number disaster recovery cmdlets:</span></span>
    + <span data-ttu-id="689a5-195">옵션 - 관련 컨트롤 번호를 지정하기 위한 AgreementType 매개 변수("X12" 또는 "Edifact")</span><span class="sxs-lookup"><span data-stu-id="689a5-195">Optional -AgreementType parameter ("X12", or "Edifact") to specify the relevant control numbers</span></span>
* <span data-ttu-id="689a5-196">MachineLearning</span><span class="sxs-lookup"><span data-stu-id="689a5-196">MachineLearning</span></span>
  - <span data-ttu-id="689a5-197">새 버전의 Azure Machine Learning .Net SDK를 사용하고 새로운 cmdlet을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-197">Consume new version of Azure Machine Learning .Net SDK and add a new cmdlet</span></span>
    + <span data-ttu-id="689a5-198">Add-AzureRmMlWebServiceRegionalProperty</span><span class="sxs-lookup"><span data-stu-id="689a5-198">Add-AzureRmMlWebServiceRegionalProperty</span></span>
  - <span data-ttu-id="689a5-199">도움말 텍스트의 일부 표현이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-199">Minor wording fixes in help text.</span></span>
* <span data-ttu-id="689a5-200">네트워크</span><span class="sxs-lookup"><span data-stu-id="689a5-200">Network</span></span>
  - <span data-ttu-id="689a5-201">Test-AzureRmNetworkWatcherConnectivity cmdlet이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-201">Added Test-AzureRmNetworkWatcherConnectivity cmdlet</span></span>
    + <span data-ttu-id="689a5-202">지정된 원본 VM 및 대상에 대한 연결 정보를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-202">Returns connectivity information for a specified source VM and a destination</span></span>
    + <span data-ttu-id="689a5-203">원본 및 대상 간에 연결을 설정할 수 없는 경우 이 cmdlet은 문제에 대한 세부 정보를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-203">If connectivity between the source and destination cannot be established, the cmdlet returns details about the issue</span></span>
* <span data-ttu-id="689a5-204">프로필</span><span class="sxs-lookup"><span data-stu-id="689a5-204">Profile</span></span>
  - <span data-ttu-id="689a5-205">\`Send-Feedback' cmdlet 추가: 사용자는 Azure PowerShell 팀에 피드백을 전송하는 일련의 메시지를 시작할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-205">Added \`Send-Feedback' cmdlet: allows a user to initiate a set of prompts which sends feedback to the Azure PowerShell team.</span></span>
  - <span data-ttu-id="689a5-206">다음 별칭은 Azure 모듈의 기존 cmdlet 이름과 충돌하므로 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-206">The following aliases have been removed as they conflicted with existing cmdlet names in the Azure module:</span></span>
    + <span data-ttu-id="689a5-207">`Enable-AzureDataCollection`(`Enable-AzureRmDataCollection`에서 지원)</span><span class="sxs-lookup"><span data-stu-id="689a5-207">`Enable-AzureDataCollection` (supported by `Enable-AzureRmDataCollection`)</span></span>
    + <span data-ttu-id="689a5-208">`Disable-AzureDataCollection`(`Disable-AzureRmDataCollection`에서 지원)</span><span class="sxs-lookup"><span data-stu-id="689a5-208">`Disable-AzureDataCollection` (supported by `Disable-AzureRmDataCollection`)</span></span>
* <span data-ttu-id="689a5-209">릴레이</span><span class="sxs-lookup"><span data-stu-id="689a5-209">Relay</span></span>
  - <span data-ttu-id="689a5-210">사용자가 모든 Azure Relay 리소스를 만들고 관리할 수 있도록 하는 Azure Relay에 대한 cmdlet을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-210">Adds cmdlets for the Azure Relay which allows users to create and manage all Azure Relay resources.</span></span>
    + `New-AzureRmRelayNamespace`
    + `Get-AzureRmRelayNamespace`
    + `Set-AzureRmRelayNamespace`
    + `Remove-AzureRmRelayNamespace`
    + `New-AzureRmWcfRelay`
    + `Get-AzureRmWcfRelay`
    + `Set-AzureRmWcfRelay`
    + `Remove-AzureRmWcfRelay`
    + `New-AzureRmRelayHybridConnection`
    + `Get-AzureRmRelayHybridConnection`
    + `Set-AzureRmRelayHybridConnection`
    + `Remove-AzureRmRelayHybridConnection`
    + `Test-AzureRmRelayName`
    + `Get-AzureRmRelayOperation`
    + `New-AzureRmRelayKey`
    + `Get-AzureRmRelayKey`
    + `New-AzureRmRelayAuthorizationRule`
    + `Get-AzureRmRelayAuthorizationRule`
    + `Set-AzureRmRelayAuthorizationRule`
    + `Remove-AzureRmRelayAuthorizationRule`
* <span data-ttu-id="689a5-211">리소스</span><span class="sxs-lookup"><span data-stu-id="689a5-211">Resources</span></span>
  - <span data-ttu-id="689a5-212">New-AzureRmResourceGroupDeployment에 대한 리소스 그룹 간 배포를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-212">Support cross-resource-group deployments for New-AzureRmResourceGroupDeployment</span></span>
    + <span data-ttu-id="689a5-213">이제 사용자는 중첩 배포를 사용하여 다른 리소스 그룹에 배포할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-213">Users can now use nested deployments to deploy to different resource groups.</span></span>
* <span data-ttu-id="689a5-214">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="689a5-214">ServiceBus</span></span>

  - <span data-ttu-id="689a5-215">버그 수정: ServiceBus 큐 개체 속성 값이 null로 설정되었으며 해당 개체는 큐 업데이트를 위해 Set-AzureRmServiceBusQueue cmdlet에서 입력 매개 변수로 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-215">Bug Fix: ServiceBus Queue object property values were set to null, the object is used as input parameter in Set-AzureRmServiceBusQueue cmdlet to update Queue.</span></span>
   - <span data-ttu-id="689a5-216">영향 받는 속성은 LockDuration, EntityAvailabilityStatus, DuplicateDetectionHistoryTimeWindow, MaxDeliveryCount 및 MessageCount입니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-216">Properties affected are LockDuration, EntityAvailabilityStatus, DuplicateDetectionHistoryTimeWindow, MaxDeliveryCount and MessageCount</span></span>
* <span data-ttu-id="689a5-217">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="689a5-217">ServiceFabric</span></span>

  - <span data-ttu-id="689a5-218">Service Fabric에 대한 cmdlet이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-218">Added cmdlets for service fabric</span></span>
    + <span data-ttu-id="689a5-219">Add-AzureRmServiceFabricApplicationCertificate       응용 프로그램 인증서로 사용할 인증서 추가</span><span class="sxs-lookup"><span data-stu-id="689a5-219">Add-AzureRmServiceFabricApplicationCertificate       Add a certificate which will be used as application certificate</span></span>
    + <span data-ttu-id="689a5-220">Add-AzureRmServiceFabricClientCertificate       클라이언트 인증을 위해 일반 이름 또는 지문을 클러스터 설정에 추가</span><span class="sxs-lookup"><span data-stu-id="689a5-220">Add-AzureRmServiceFabricClientCertificate       Add a common name or thumbprint to the cluster settings for client authentication</span></span>
    + <span data-ttu-id="689a5-221">Add-AzureRmServiceFabricClusterCertificate       기존 인증서를 롤오버하기 위해 클러스터에 보조 클러스터 인증서 추가</span><span class="sxs-lookup"><span data-stu-id="689a5-221">Add-AzureRmServiceFabricClusterCertificate       Add a secondary cluster certificate to the cluster for rolling over the existing certificate</span></span>
    + <span data-ttu-id="689a5-222">Add-AzureRmServiceFabricNodes       클러스터에 특정 노드 형식의 노드/VM 추가</span><span class="sxs-lookup"><span data-stu-id="689a5-222">Add-AzureRmServiceFabricNodes       Add nodes/VMs of a specific node type to a cluster</span></span>
    + <span data-ttu-id="689a5-223">Add-AzureRmServiceFabricNodeType       기존 클러스터에 노드 형식/VM 추가</span><span class="sxs-lookup"><span data-stu-id="689a5-223">Add-AzureRmServiceFabricNodeType       Add a node type/VMs to an existing cluster</span></span>
    + <span data-ttu-id="689a5-224">Get-AzureRmServiceFabricCluster       클러스터 리소스의 세부 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="689a5-224">Get-AzureRmServiceFabricCluster       Get the details of the cluster resource</span></span>
    + <span data-ttu-id="689a5-225">New-AzureRmServiceFabricCluster 새 ServiceFabric 클러스터를 만들기</span><span class="sxs-lookup"><span data-stu-id="689a5-225">New-AzureRmServiceFabricCluster Create a new ServiceFabric cluster.</span></span> <span data-ttu-id="689a5-226">이 명령은 다양한 시나리오에 적용되는 여러 오버로드를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-226">This command has many overloads to cover various scenarios</span></span>
    + <span data-ttu-id="689a5-227">Remove-AzureRmServiceFabricClientCertificate       클러스터에 액세스하는 데 사용되는 클라이언트 인증서 제거</span><span class="sxs-lookup"><span data-stu-id="689a5-227">Remove-AzureRmServiceFabricClientCertificate       Remove a client certificate from being used to access a cluster</span></span>
    + <span data-ttu-id="689a5-228">Remove-AzureRmServiceFabricClusterCertificate       클러스터 보안에 사용되지 않도록 클라이언트 인증서 제거</span><span class="sxs-lookup"><span data-stu-id="689a5-228">Remove-AzureRmServiceFabricClusterCertificate       Remove a cluster certificate from being used for cluster security</span></span>
    + <span data-ttu-id="689a5-229">Remove-AzureRmServiceFabricNodes       클러스터에서 특정 노드 형식의 노드 제거</span><span class="sxs-lookup"><span data-stu-id="689a5-229">Remove-AzureRmServiceFabricNodes       Remove nodes from a specific node type from a cluster</span></span>
    + <span data-ttu-id="689a5-230">Remove-AzureRmServiceFabricNodeType       클러스터에서 노드 형식 제거</span><span class="sxs-lookup"><span data-stu-id="689a5-230">Remove-AzureRmServiceFabricNodeType       Remove a node type from a cluster</span></span>
    + <span data-ttu-id="689a5-231">Remove-AzureRmServiceFabricSettings       클러스터에서 하나 이상의 ServiceFabric 설정 제거</span><span class="sxs-lookup"><span data-stu-id="689a5-231">Remove-AzureRmServiceFabricSettings       Remove one or more ServiceFabric settings from a cluster</span></span>
    + <span data-ttu-id="689a5-232">Set-AzureRmServiceFabricSettings       클러스터의 하나 이상 ServiceFabric 설정 추가 또는 업데이트</span><span class="sxs-lookup"><span data-stu-id="689a5-232">Set-AzureRmServiceFabricSettings       Add or update one or more ServiceFabric settings of a cluster</span></span>
    + <span data-ttu-id="689a5-233">Set-AzureRmServiceFabricUpgradeType       클러스터의 ServiceFabric 업그레이드 집합 변경</span><span class="sxs-lookup"><span data-stu-id="689a5-233">Set-AzureRmServiceFabricUpgradeType       Change the ServiceFabric upgrade type of a cluster</span></span>
    + <span data-ttu-id="689a5-234">Update-AzureRmServiceFabricDurability       클러스터의 지속성 계층 변경</span><span class="sxs-lookup"><span data-stu-id="689a5-234">Update-AzureRmServiceFabricDurability       Change the durability tier of a cluster</span></span>
    + <span data-ttu-id="689a5-235">Update-AzureRmServiceFabricReliability       클러스터의 안정성 계층 변경</span><span class="sxs-lookup"><span data-stu-id="689a5-235">Update-AzureRmServiceFabricReliability       Change the reliability tier of a cluster</span></span>
* <span data-ttu-id="689a5-236">Sql</span><span class="sxs-lookup"><span data-stu-id="689a5-236">Sql</span></span>
  - <span data-ttu-id="689a5-237">New-AzureRmSqlDatabase에 -SampleName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="689a5-237">Added -SampleName parameter to New-AzureRmSqlDatabase</span></span>
  - <span data-ttu-id="689a5-238">장애 조치 그룹 cmdlet에 대한 업데이트</span><span class="sxs-lookup"><span data-stu-id="689a5-238">Updates to Failover Group cmdlets</span></span>
  - <span data-ttu-id="689a5-239">'Tag' 매개 변수 제거</span><span class="sxs-lookup"><span data-stu-id="689a5-239">Remove 'Tag' parameters</span></span>
  - <span data-ttu-id="689a5-240">Remove-AzureRmSqlDatabaseFailoverGroup cmdlet에서 'PartnerResourceGroupName' 및 'PartnerServerName' 매개 변수 제거</span><span class="sxs-lookup"><span data-stu-id="689a5-240">Remove 'PartnerResourceGroupName' and 'PartnerServerName' parameters from Remove-AzureRmSqlDatabaseFailoverGroup cmdlet</span></span>
  - <span data-ttu-id="689a5-241">New- 및 Set- cmdlet에 'GracePeriodWithDataLossHours' 매개 변수가 추가되고 결과적으로 'GracePeriodWithDataLossHour' 대신 사용됨</span><span class="sxs-lookup"><span data-stu-id="689a5-241">Add 'GracePeriodWithDataLossHours' parameter to New- and Set- cmdlets, which shall eventually replace 'GracePeriodWithDataLossHour'</span></span>
  - <span data-ttu-id="689a5-242">설명서가 보완되고 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="689a5-242">Documentation has been fleshed out and updated</span></span>
  - <span data-ttu-id="689a5-243">반환된 개체의 서식 변경, 필드가 항상 채워지지는 않던 일부 버그 수정</span><span class="sxs-lookup"><span data-stu-id="689a5-243">Change formatting of returned objects and fix some bugs where fields were not always populated</span></span>
  - <span data-ttu-id="689a5-244">장애 조치(Failover) 그룹 개체에 'DatabaseNames' 및 'PartnerLocation' 속성 추가</span><span class="sxs-lookup"><span data-stu-id="689a5-244">Add 'DatabaseNames' and 'PartnerLocation' properties to Failover Group object</span></span>
  - <span data-ttu-id="689a5-245">Switch- cmdlet에서 작업이 완료되기를 기다리지 않고 즉시 반환되도록 하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="689a5-245">Fix bug causing Switch- cmdlet to return immediately rather than waiting for operation to complete</span></span>
  - <span data-ttu-id="689a5-246">높은 유예 기간 값이 사용되는 정수 오버플로 버그 수정</span><span class="sxs-lookup"><span data-stu-id="689a5-246">Fix integer overflow bug when high grace period values are used</span></span>
  - <span data-ttu-id="689a5-247">더 낮은 값이 제공될 경우 유예 기간을 최소값인 1시간으로 조정</span><span class="sxs-lookup"><span data-stu-id="689a5-247">Adjust grace period to a minimum of 1 hour if a lower one is provided</span></span>
  - <span data-ttu-id="689a5-248">Set-AzureRmSqlDatabaseThreatDetectionPolicy cmdlet 및 Set-AzureRmSqlServerThreatDetectionPolicy cmdlet의 "ExcludedDetectionType" 매개 변수에 대해 허용되는 값 중에서 "Usage_Anomaly" 제거</span><span class="sxs-lookup"><span data-stu-id="689a5-248">Remove "Usage_Anomaly" from the accepted values for "ExcludedDetectionType" parameter of Set-AzureRmSqlDatabaseThreatDetectionPolicy cmdlet and Set-AzureRmSqlServerThreatDetectionPolicy cmdlet.</span></span>
* <span data-ttu-id="689a5-249">저장소</span><span class="sxs-lookup"><span data-stu-id="689a5-249">Storage</span></span>
  - <span data-ttu-id="689a5-250">SRP SDK를 6.3.0으로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="689a5-250">Upgrade SRP SDK to 6.3.0</span></span>
  - <span data-ttu-id="689a5-251">New/Set-AzureRmStorageAccount: EnableHttpsTrafficOnly를 지원하기 위한 새 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="689a5-251">New/Set-AzureRmStorageAccount:Add a new parameter to support EnableHttpsTrafficOnly</span></span>
  - <span data-ttu-id="689a5-252">New/Set/Get-AzureRmStorageAccount: 반환된 저장소 계정에 새 특성인 EnableHttpsTrafficOnly가 포함되어 있음</span><span class="sxs-lookup"><span data-stu-id="689a5-252">New/Set/Get-AzureRmStorageAccount: Returned Storage Account contains a new attribute EnableHttpsTrafficOnly</span></span>
* <span data-ttu-id="689a5-253">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="689a5-253">Azure.Storage</span></span>
  - <span data-ttu-id="689a5-254">Azure Storage 클라이언트 라이브러리 8.1.1 및 Azure Storage DataMovement 라이브러리 0.5.1로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="689a5-254">Upgrade to Azure Storage Client Library 8.1.1 and Azure Storage DataMovement Library 0.5.1</span></span>
  - <span data-ttu-id="689a5-255">Blob 증분 복사 기능을 지원하기 위한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="689a5-255">Add a new cmdlet to support blob Incremental Copy feature</span></span>
