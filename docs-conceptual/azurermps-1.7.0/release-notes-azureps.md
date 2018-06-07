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
ms.date: 05/18/2017
ms.openlocfilehash: 9f31fe404cca1162d5e4898287261f1bcbfa0f3a
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/06/2018
ms.locfileid: "34821856"
---
# <a name="release-notes"></a><span data-ttu-id="012c0-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="012c0-103">Release notes</span></span>

<span data-ttu-id="012c0-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-170"></a><span data-ttu-id="012c0-105">1.7.0 버전</span><span class="sxs-lookup"><span data-stu-id="012c0-105">Version 1.7.0</span></span>

* <span data-ttu-id="012c0-106">**모든 cmdlet에 대해 -Force, -Confirm 및 $ConfirmPreference 매개 변수의 동작을 변경합니다. PowerShell 지침에 따라 이 구현을 변경하고 있습니다. 대부분의 cmdlet에 대해 Force 매개 변수를 제거하고 ShouldProcess 프롬프트를 건너뛰므로 사용자가 PowerShell 스크립트에 '-Confirm: $ false' 매개 변수를 포함해야 합니다.**</span><span class="sxs-lookup"><span data-stu-id="012c0-106">**Behavioral change for -Force, –Confirm and $ConfirmPreference parameters for all cmdlets. We are changing this implementation to be in line with PowerShell guidelines. For most cmdlets, this means removing the Force parameter and to skip the ShouldProcess prompt, users will need to include the parameter: ‘-Confirm:$false’ in their PowerShell scripts.**</span></span> <span data-ttu-id="012c0-107">이 변경 내용은 다음 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-107">This changes are addressing following issues:</span></span>
  - <span data-ttu-id="012c0-108">–WhatIf 기능의 올바른 구현 - 사용자가 실제로 변경하지 않고 cmdlet 또는 스크립트의 영향을 결정할 수 있게 합니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-108">Correct implementation of –WhatIf functionality, allowing a user to determine the effects of a cmdlet or script without making any actual changes</span></span>
  - <span data-ttu-id="012c0-109">세션 전체 $ConfirmPreference를 사용하여 메시지 표시에 대한 컨트롤 - 사용자에게 잠재적 변경의 영향을 기반으로 한 메시지가 표시됩니다(cmdlet의 ConfirmImpact 설정에서 보고됨).</span><span class="sxs-lookup"><span data-stu-id="012c0-109">Control over prompting using a session-wide $ConfirmPreference, so that the user is prompted based on the impact of a prospective change (as reported in the ConfirmImpact setting in the cmdlet)</span></span>
  - <span data-ttu-id="012c0-110">-Confirm 매개 변수를 사용하여 확인 메시지 표시에 대한 cmdlet 관련 컨트롤</span><span class="sxs-lookup"><span data-stu-id="012c0-110">Cmdlet-specific control over confirmation prompts using the –Confirm parameter</span></span>
  - <span data-ttu-id="012c0-111">cmdlet 간에 일관된 ShouldContinue 및 -Force 매개 변수 사용 - 변경의 특수한 특성(예: 숨김 파일 삭제)으로 인해 사용자에게 묻는 메시지를 표시해야 하는 작업에만 사용</span><span class="sxs-lookup"><span data-stu-id="012c0-111">Consistent use of ShouldContinue and the –Force parameter across cmdlets, for only those actions that would require prompting from the user due to the special nature of the changes (for example, deleting hidden files)</span></span>
  - <span data-ttu-id="012c0-112">다른 PowerShell cmdlet과의 일관성 - 다른 cmdlet의 PowerShell 스크립팅 지식을 Azure PowerShell cmdlet에 즉시 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-112">Consistency with other PowerShell cmdlets, so that PowerShell scripting knowledge from other cmdlets is immediately applicable to the Azure PowerShell cmdlets.</span></span>

<span data-ttu-id="012c0-113">***모든 상황에서 모든 프롬프트를 자동으로 건너뜁니다.* Azure PowerShell cmdlet에서 사용자가 다음 두 매개 변수를 제공해야 합니다.**</span><span class="sxs-lookup"><span data-stu-id="012c0-113">**Notice that now to *automatically skip all Prompts in all Circumstances* Azure PowerShell cmdlets require the user to supply two parameters:**</span></span>
```powershell
My-CmdletWithConfirmation –Confirm:$false -Force
```
* <span data-ttu-id="012c0-114">Azure Compute</span><span class="sxs-lookup"><span data-stu-id="012c0-114">Azure Compute</span></span>
  - <span data-ttu-id="012c0-115">Set-AzureRmVMADDomainExtension</span><span class="sxs-lookup"><span data-stu-id="012c0-115">Set-AzureRmVMADDomainExtension</span></span>
  - <span data-ttu-id="012c0-116">Get-AzureRmVMADDomainExtension</span><span class="sxs-lookup"><span data-stu-id="012c0-116">Get-AzureRmVMADDomainExtension</span></span>
  - <span data-ttu-id="012c0-117">Restart-AzureVM에 대한 -Redeploy 매개 변수</span><span class="sxs-lookup"><span data-stu-id="012c0-117">-Redeploy parameter for Restart-AzureVM</span></span>
  - <span data-ttu-id="012c0-118">Move-AzureService, Move-AzureStorageAccount 및 Move-AzureVirtualNetwork에 대한 -Validate 매개 변수</span><span class="sxs-lookup"><span data-stu-id="012c0-118">-Validate parameter for Move-AzureService, Move-AzureStorageAccount, and Move-AzureVirtualNetwork</span></span>
  - <span data-ttu-id="012c0-119">확장 cmdlet의 name 및 version 매개 변수는 이전과 마찬가지로 선택 사항입니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-119">Name and version parameters for extension cmdlets are optional as before.</span></span>
  - <span data-ttu-id="012c0-120">New-AzureVM은 VM 개체에서 라이선스 유형을 가져올 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-120">New-AzureVM can get a license type from VM object.</span></span>
* <span data-ttu-id="012c0-121">Azure Storage</span><span class="sxs-lookup"><span data-stu-id="012c0-121">Azure Storage</span></span>
  - <span data-ttu-id="012c0-122">Tags 매개 변수를 Tag로 변경 및 매개 변수 별칭 Tags 추가</span><span class="sxs-lookup"><span data-stu-id="012c0-122">Change Tags Parameter to Tag, and add parameter alias Tags</span></span>
    + <span data-ttu-id="012c0-123">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="012c0-123">New-AzureRmStorageAccount</span></span>
    + <span data-ttu-id="012c0-124">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="012c0-124">Set-AzureRmStorageAccount</span></span>
* <span data-ttu-id="012c0-125">Azure 네트워크</span><span class="sxs-lookup"><span data-stu-id="012c0-125">Azure Network</span></span>
  - <span data-ttu-id="012c0-126">Virtual Network 피어링에 대한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="012c0-126">New cmdlet added for Virtual Network Peering</span></span>
* <span data-ttu-id="012c0-127">Azure Redis Cache</span><span class="sxs-lookup"><span data-stu-id="012c0-127">Azure Redis Cache</span></span>
  - <span data-ttu-id="012c0-128">Reset-AzureRmRedisCache에 대한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="012c0-128">New cmdlet added for Reset-AzureRmRedisCache</span></span>
  - <span data-ttu-id="012c0-129">Export-AzureRmRedisCache에 대한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="012c0-129">New cmdlet added for Export-AzureRmRedisCache</span></span>
  - <span data-ttu-id="012c0-130">Import-AzureRmRedisCache에 대한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="012c0-130">New cmdlet added for Import-AzureRmRedisCache</span></span>
  - <span data-ttu-id="012c0-131">vNet에 대한 매개 변수 변경을 포함하도록 New-AzureRmRedisCache cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="012c0-131">Modified cmdlet New-AzureRmRedisCache to include parameter change for vNet</span></span>
* <span data-ttu-id="012c0-132">Azure SQL DB Backup/복원</span><span class="sxs-lookup"><span data-stu-id="012c0-132">Azure SQL DB Backup/Restore</span></span>
  - <span data-ttu-id="012c0-133">LTR(장기 보존) 백업 기능에 대한 cmdlet</span><span class="sxs-lookup"><span data-stu-id="012c0-133">Cmdlets for LTR (Long Term Retention) backup feature</span></span>
  - <span data-ttu-id="012c0-134">Get-AzureRmSqlServerBackupLongTermRetentionVault</span><span class="sxs-lookup"><span data-stu-id="012c0-134">Get-AzureRmSqlServerBackupLongTermRetentionVault</span></span>
  - <span data-ttu-id="012c0-135">Get-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="012c0-135">Get-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span></span>
  - <span data-ttu-id="012c0-136">Set-AzureRmSqlServerBackupLongTermRetentionVault</span><span class="sxs-lookup"><span data-stu-id="012c0-136">Set-AzureRmSqlServerBackupLongTermRetentionVault</span></span>
  - <span data-ttu-id="012c0-137">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="012c0-137">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span></span>
  - <span data-ttu-id="012c0-138">Restore-AzureRmSqlDatabase에서 이제는 삭제된 데이터베이스의 특정 시점 복원 지원</span><span class="sxs-lookup"><span data-stu-id="012c0-138">Restore-AzureRmSqlDatabase now supports point-in-time restore of a deleted database</span></span>
  - <span data-ttu-id="012c0-139">Restore-AzureRmSqlDatabase에서 이제는 장기 보존 백업의 복원 지원</span><span class="sxs-lookup"><span data-stu-id="012c0-139">Restore-AzureRmSqlDatabase now supports restoring from a Long Term Retention backup</span></span>
* <span data-ttu-id="012c0-140">Azure LogicApp</span><span class="sxs-lookup"><span data-stu-id="012c0-140">Azure LogicApp</span></span>
  - <span data-ttu-id="012c0-141">LogicApp 통합 계정 cmdlet 추가.</span><span class="sxs-lookup"><span data-stu-id="012c0-141">Added LogicApp Integration accounts cmdlets.</span></span>
  - <span data-ttu-id="012c0-142">Get-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="012c0-142">Get-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="012c0-143">Get-AzureRmIntegrationAccountCallbackUrl</span><span class="sxs-lookup"><span data-stu-id="012c0-143">Get-AzureRmIntegrationAccountCallbackUrl</span></span>
  - <span data-ttu-id="012c0-144">Get-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="012c0-144">Get-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="012c0-145">Get-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="012c0-145">Get-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="012c0-146">Get-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="012c0-146">Get-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="012c0-147">Get-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="012c0-147">Get-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="012c0-148">Get-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="012c0-148">Get-AzureRmIntegrationAccountSchema</span></span>
  - <span data-ttu-id="012c0-149">New-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="012c0-149">New-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="012c0-150">New-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="012c0-150">New-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="012c0-151">New-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="012c0-151">New-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="012c0-152">New-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="012c0-152">New-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="012c0-153">New-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="012c0-153">New-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="012c0-154">New-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="012c0-154">New-AzureRmIntegrationAccountSchema</span></span>
  - <span data-ttu-id="012c0-155">Remove-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="012c0-155">Remove-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="012c0-156">Remove-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="012c0-156">Remove-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="012c0-157">Remove-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="012c0-157">Remove-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="012c0-158">Remove-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="012c0-158">Remove-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="012c0-159">Remove-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="012c0-159">Remove-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="012c0-160">Remove-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="012c0-160">Remove-AzureRmIntegrationAccountSchema</span></span>
  - <span data-ttu-id="012c0-161">Set-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="012c0-161">Set-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="012c0-162">Set-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="012c0-162">Set-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="012c0-163">Set-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="012c0-163">Set-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="012c0-164">Set-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="012c0-164">Set-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="012c0-165">Set-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="012c0-165">Set-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="012c0-166">Set-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="012c0-166">Set-AzureRmIntegrationAccountSchema</span></span>
* <span data-ttu-id="012c0-167">Azure Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="012c0-167">Azure Data Lake Store</span></span>
  - <span data-ttu-id="012c0-168">파일과 폴더의 업로드 및 다운로드 성능을 크게 향상.</span><span class="sxs-lookup"><span data-stu-id="012c0-168">Drastically improve performance of file and folder upload and download.</span></span>
  - <span data-ttu-id="012c0-169">다운로드에 대한 매개 변수 이름을 약간 변경했고, 업로드에 대한 새로운 두 매개 변수를 포함했습니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-169">This includes a slight change to the parameter names for download and inclusion of two new parameters for upload:</span></span>
    + <span data-ttu-id="012c0-170">NumThreads -> PerFileThreadCount - 단일 파일에서 사용할 스레드 수를 나타내는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-170">NumThreads -> PerFileThreadCount, used to indicate the number of threads to use in a single file</span></span>
    + <span data-ttu-id="012c0-171">ConcurrentFileCount - 폴더 업로드/다운로드를 위해 병렬로 업로드/다운로드할 파일 수를 나타내는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-171">ConcurrentFileCount, used to indicate the number of files to upload/download in parallel for folder upload/download.</span></span>
  - <span data-ttu-id="012c0-172">기본 스레딩 값이 이제 대부분의 파일 크기에 대한 처리량을 향상시키도록 설계되었습니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-172">Default threading values are now designed to give a better all around throughput for most file sizes.</span></span> <span data-ttu-id="012c0-173">성능이 원하는 대로 수행되지 않으면 위의 값을 수정하여 요구 사항을 충족할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-173">If performance is not as desired, the values above can be modified to meet requirements.</span></span>
* <span data-ttu-id="012c0-174">Azure 데이터 레이크 분석</span><span class="sxs-lookup"><span data-stu-id="012c0-174">Azure Data Lake Analytics</span></span>
  - <span data-ttu-id="012c0-175">Get-AzureRMDataLakeAnalyticsDataSource가 이제 인수 없이 호출될 때 모든 데이터 원본 반환.</span><span class="sxs-lookup"><span data-stu-id="012c0-175">Get-AzureRMDataLakeAnalyticsDataSource now returns all data sources when called with no arguments.</span></span>
  - <span data-ttu-id="012c0-176">이 변경은 cmdlet에서 데이터 원본 형식 매개 변수도 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-176">This change also removes the data source type parameter from the cmdlet.</span></span>
  - <span data-ttu-id="012c0-177">이 변경으로 인해 다음 속성을 사용하여 목록 작업에 대해 새 개체를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-177">This change results in a new object being returned for the list operation with the following properties:</span></span>
    + <span data-ttu-id="012c0-178">Type - 데이터 원본 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-178">Type, the type of data source</span></span>
    + <span data-ttu-id="012c0-179">Name - 데이터 원본 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-179">Name, the name of the data source</span></span>
    + <span data-ttu-id="012c0-180">IsDefault - 계정에 대한 기본 데이터 원본인 경우 true로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="012c0-180">IsDefault, set to true if this is the default data source for the account</span></span>
  - <span data-ttu-id="012c0-181">submittedBefore 및 submittedAfter에서 필터링할 때 Get-AzureRMDataLakeAnalyticsJob이 특정 날짜 시간 오프셋 값 목록으로 고정.</span><span class="sxs-lookup"><span data-stu-id="012c0-181">Get-AzureRMDataLakeAnalyticsJob fixed for list for certain date time offset values when filtering on submittedBefore and submittedAfter.</span></span>
* <span data-ttu-id="012c0-182">Web Apps</span><span class="sxs-lookup"><span data-stu-id="012c0-182">Web Apps</span></span>
  - <span data-ttu-id="012c0-183">일반 교환 및 미리 보기 포함 교환에 대한 Swap-AzureRmWebAppSlot cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="012c0-183">Add Swap-AzureRmWebAppSlot cmdlet for regular swap and swap with preview</span></span>
  - <span data-ttu-id="012c0-184">자동 교환을 지원하도록 Set-AzureRmWebAppSlot cmdlet 확장</span><span class="sxs-lookup"><span data-stu-id="012c0-184">Extend Set-AzureRmWebAppSlot cmdlet to support auto swap</span></span>
* <span data-ttu-id="012c0-185">Azure API Management</span><span class="sxs-lookup"><span data-stu-id="012c0-185">Azure API Management</span></span>
  - <span data-ttu-id="012c0-186">AzureChinaCloud에 대한 Azure API Management 배포 cmdlet 수정.</span><span class="sxs-lookup"><span data-stu-id="012c0-186">Fixed Azure Api Management Deployment cmdlets for AzureChinaCloud.</span></span>
  - <span data-ttu-id="012c0-187">기본적으로 Git 액세스를 사용하도록 설정되므로 Set-AzureRmApiManagementTenantGitAccess cmdlet 제거.</span><span class="sxs-lookup"><span data-stu-id="012c0-187">Removed cmdlet Set-AzureRmApiManagementTenantGitAccess as Git Access is enabled by Default.</span></span>
* <span data-ttu-id="012c0-188">Azure Recovery Services Backup</span><span class="sxs-lookup"><span data-stu-id="012c0-188">Azure Recovery Services Backup</span></span>
  - <span data-ttu-id="012c0-189">Azure SQL 워크로드 지원 추가</span><span class="sxs-lookup"><span data-stu-id="012c0-189">Added support for the Azure SQL workload</span></span>
  - <span data-ttu-id="012c0-190">암호화된 Azure VM 백업 및 복원 지원 추가</span><span class="sxs-lookup"><span data-stu-id="012c0-190">Added support for backing up and restoring encrypted Azure VMs</span></span>
  - <span data-ttu-id="012c0-191">Backup-AzureRmRecoveryServicesBackupItem - 복구 지점에 대한 선택적 보존 시간 기능 추가</span><span class="sxs-lookup"><span data-stu-id="012c0-191">Backup-AzureRmRecoveryServicesBackupItem - Added optional retention time feature for recovery points</span></span>
  - <span data-ttu-id="012c0-192">Get-AzureRmRecoveryServicesBackupContainer 및 Get-AzureRmRecoveryServicesBackupItem cmdlet의 보조 필터 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="012c0-192">Minor filter-related bug fixes in Get-AzureRmRecoveryServicesBackupContainer and Get-AzureRmRecoveryServicesBackupItem cmdlets</span></span>
* <span data-ttu-id="012c0-193">Azure Automation</span><span class="sxs-lookup"><span data-stu-id="012c0-193">Azure Automation</span></span>
  - <span data-ttu-id="012c0-194">Get-AzureRmAutomationHybridWorkerGroup 추가</span><span class="sxs-lookup"><span data-stu-id="012c0-194">Added Get-AzureRmAutomationHybridWorkerGroup</span></span>
