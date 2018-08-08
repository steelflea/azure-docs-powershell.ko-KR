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
ms.openlocfilehash: 3961f5c37869d0dc877b85bad535f399181040db
ms.sourcegitcommit: fd11600079ee3844986552bccc4e274a231332b6
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/02/2018
ms.locfileid: "39368180"
---
# <a name="release-notes"></a><span data-ttu-id="52089-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="52089-103">Release notes</span></span>

<span data-ttu-id="52089-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="52089-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="660---july-2018"></a><span data-ttu-id="52089-105">6.6.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="52089-105">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="52089-106">일반</span><span class="sxs-lookup"><span data-stu-id="52089-106">General</span></span>
* <span data-ttu-id="52089-107">전체 매개 변수 형식 및 올바른 입/출력 형식을 포함하도록 모든 도움말 파일을 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-107">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="52089-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="52089-108">AzureRM.Profile</span></span>
* <span data-ttu-id="52089-109">Common.Strategy 라이브러리가 리소스에 대한 현재 구성이 대상 리소스와 호환되는지 유효성을 검사할 수 있도록 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-109">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span> <span data-ttu-id="52089-110">기본값은 항상 true이고, 개별 리소스이며 기본값을 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-110">Default is always true, individual resources and overridet the default.</span></span>
* <span data-ttu-id="52089-111">Common.Storage에 ps1xml 형식 추가</span><span class="sxs-lookup"><span data-stu-id="52089-111">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="52089-112">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="52089-112">Azure.Storage</span></span>
* <span data-ttu-id="52089-113">DefaulfProfile에서 저장소 컨텍스트를 가져오도록 지원</span><span class="sxs-lookup"><span data-stu-id="52089-113">Support get Storage Context from DefaulfProfile</span></span>
* <span data-ttu-id="52089-114">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="52089-114">Add Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="52089-115">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="52089-115">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="52089-116">문제 https://github.com/Azure/azure-powershell/issues/6370 해결</span><span class="sxs-lookup"><span data-stu-id="52089-116">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="52089-117">PsApiManagementApi를 ApiContract로 좌표 이동하도록 Automapper 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="52089-117">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="52089-118">문제 https://github.com/Azure/azure-powershell/issues/6515 해결</span><span class="sxs-lookup"><span data-stu-id="52089-118">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="52089-119">인코딩 형식을 사용하여 오버로드하지 않도록 File.Save 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="52089-119">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="52089-120">문제 https://github.com/Azure/azure-powershell/issues/6560 해결</span><span class="sxs-lookup"><span data-stu-id="52089-120">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="52089-121">apiId에서 패턴 예외를 수정하는 4.0.3 Nuget 버전으로 업그레이드됨</span><span class="sxs-lookup"><span data-stu-id="52089-121">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="52089-122">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="52089-122">AzureRM.Compute</span></span>
* <span data-ttu-id="52089-123">PremiumLRS 저장소 계정 형식 이름 바꾸기로 인해 New-AzureRmVm에서 DiskFileParameterSet를 사용하여 vm 생성 시 실패하는 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-123">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="52089-124">Invoke-AzureRmVMRunCommand cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="52089-124">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="52089-125">Get-AzureRmAvailabilitySet를 업데이트하여 구독에서 모든 가용성 집합 리스트를 사용하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-125">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="52089-126">(ResouceGroupName 매개 변수는 이제 선택적 요소입니다.)</span><span class="sxs-lookup"><span data-stu-id="52089-126">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="52089-127">vm 선별에 가속화된 네트워크를 사용하도록 'New-AzureRmVm'의 SimpleParameterSet를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-127">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="52089-128">New-AzureRmVmss 간단 매개 변수가 사용자 지정 LB가 이미 존재할 때 vms 생성에 실패하도록 설정하여 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-128">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="52089-129">New-AzureRmDisk에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-129">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="52089-130">'New-AzureRmVM'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="52089-130">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="52089-131">Set-AzureRmVMOSDisk에 대한 설명 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-131">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="52089-132">Set-AzureRmVMBginfoExtension 맞춤법 및 접두사를 수정하도록 예제 1을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-132">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="52089-133">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="52089-133">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="52089-134">ADF.Net SDK 버전을 1.1.0으로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-134">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="52089-135">데이터 팩터리를 공유하는 자체 호스팅된 통합 런타임을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-135">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="52089-136">새 매개 변수 -SharedIntegrationRuntimeResourceId를 Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="52089-136">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="52089-137">새로운 선택적 매개 변수 -LinkedDataFactoryName을 Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="52089-137">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="52089-138">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="52089-138">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="52089-139">DataPlane SDK(Microsoft.Azure.DataLake.Store) 버전을 1.1.9로 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-139">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="52089-140">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="52089-140">AzureRM.EventHub</span></span>
* <span data-ttu-id="52089-141">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="52089-141">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="52089-142">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="52089-142">AzureRM.Insights</span></span>
* <span data-ttu-id="52089-143">도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="52089-143">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="52089-144">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview를 사용</span><span class="sxs-lookup"><span data-stu-id="52089-144">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="52089-145">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="52089-145">AzureRM.KeyVault</span></span>
* <span data-ttu-id="52089-146">Set-AzureRmKeyVaultAccessPolicy 내 파이핑 문제 해결</span><span class="sxs-lookup"><span data-stu-id="52089-146">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="52089-147">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="52089-147">AzureRM.Network</span></span>
* <span data-ttu-id="52089-148">LoadBalancerInboundNatPoolConfig cmdlet에 대한 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-148">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="52089-149">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="52089-149">AzureRM.Resources</span></span>
* <span data-ttu-id="52089-150">'Get-AzureRmResource'에 대한 태그 이름 및 값을 제공할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="52089-150">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="52089-151">'Set-AzureRmResource'를 사용하여 파이핑 시나리오 해결</span><span class="sxs-lookup"><span data-stu-id="52089-151">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="52089-152">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="52089-152">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="52089-153">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="52089-153">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="52089-154">몇 가지 문제 해결</span><span class="sxs-lookup"><span data-stu-id="52089-154">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="52089-155">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="52089-155">AzureRM.Sql</span></span>
* <span data-ttu-id="52089-156">다음 cmdlet 사용하여 서버 Advanced Threat Protection 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-156">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="52089-157">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="52089-157">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="52089-158">다음 cmdlet을 사용하여 취약성 평가 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-158">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="52089-159">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="52089-159">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="52089-160">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="52089-160">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="52089-161">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="52089-161">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="52089-162">Remove-AzureRmSqlServerFirewallRule의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="52089-162">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="52089-163">Get-AzureSqlSyncGroupLog에서 미국이 아닌 문화권에서 날짜/시간을 올바르지 않게 다루는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="52089-163">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="52089-164">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="52089-164">AzureRM.Storage</span></span>
* <span data-ttu-id="52089-165">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="52089-165">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="52089-166">StorageAccount cmdlet 출력을 테이블 뷰로 표시</span><span class="sxs-lookup"><span data-stu-id="52089-166">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="52089-167">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="52089-167">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="52089-168">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="52089-168">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="52089-169">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="52089-169">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="52089-170">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="52089-170">AzureRM.Tags</span></span>
* <span data-ttu-id="52089-171">태그 cmdlet 도움말에서 잘못된 문을 제거합니다</span><span class="sxs-lookup"><span data-stu-id="52089-171">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="52089-172">6.5.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="52089-172">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="52089-173">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="52089-173">AzureRM.Profile</span></span>
* <span data-ttu-id="52089-174">'Get-AzureRmContextAutosaveSetting'에 대한 도움말이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="52089-174">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="52089-175">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="52089-175">Azure.Storage</span></span>
* <span data-ttu-id="52089-176">쓰기 전용 SaS 토큰을 사용하는 Blob 또는 파일 업로드 지원</span><span class="sxs-lookup"><span data-stu-id="52089-176">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="52089-177">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="52089-177">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="52089-178">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="52089-178">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="52089-179">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="52089-179">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="52089-180">필수 속성 ResourceGroupName을 AS에 추가</span><span class="sxs-lookup"><span data-stu-id="52089-180">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="52089-181">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="52089-181">AzureRM.Automation</span></span>
* <span data-ttu-id="52089-182">도움말을 업데이트하고 'New-AzureRMAutomationSchedule'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="52089-182">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="52089-183">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="52089-183">AzureRM.Compute</span></span>
* <span data-ttu-id="52089-184">-Tag 매개 변수를 Update/New-AzureRmAvailabilitySet에 추가</span><span class="sxs-lookup"><span data-stu-id="52089-184">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="52089-185">‘Add-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="52089-185">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="52089-186">‘Remove-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="52089-186">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="52089-187">‘Set-AzureRmVMAccessExtension’에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-187">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="52089-188">기본으로 SinglePlacementGroup을 false로 설정하고 단일 배치 그룹에 VMSS를 만들 수 있는 스위치 매개 변수 'SinglePlacementGroup'을 추가하도록 New-AzureRmVmss에 대한 SimpleParameterSet을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-188">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="52089-189">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="52089-189">AzureRM.EventHub</span></span>
* <span data-ttu-id="52089-190">PSEventHubDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="52089-190">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="52089-191">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="52089-191">AzureRM.KeyVault</span></span>
* <span data-ttu-id="52089-192">Set-AzureRmKeyVaultAccessPolicy에 대한 오류 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-192">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="52089-193">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="52089-193">AzureRM.LogicApp</span></span>
* <span data-ttu-id="52089-194">New-AzureRmLogicApp에서 "매개 변수 집합을 확인할 수 없습니다" 오류 해결</span><span class="sxs-lookup"><span data-stu-id="52089-194">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="52089-195">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="52089-195">AzureRM.Network</span></span>
* <span data-ttu-id="52089-196">Set/Add-AzureRmVirtualNetworkPeering에 대한 여러 테넌트의 가상 네트워크에서 피어링을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="52089-196">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="52089-197">Application Gateway에 대한 아래 cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-197">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="52089-198">New-AzureRmApplicationGateway: EnableFIPS 플래그 및 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="52089-198">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="52089-199">New-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="52089-199">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="52089-200">Set-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="52089-200">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="52089-201">최신 생성기를 사용하여 RouteTable cmdlet을 재생성</span><span class="sxs-lookup"><span data-stu-id="52089-201">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="52089-202">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="52089-202">AzureRM.Relay</span></span>
* <span data-ttu-id="52089-203">markdown 파일을 업데이트하여 예제에서 매개 변수 이름 문제에 대해 해결</span><span class="sxs-lookup"><span data-stu-id="52089-203">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="52089-204">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="52089-204">AzureRM.Resources</span></span>
* <span data-ttu-id="52089-205">Roledefinition 및 Roleassignment cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-205">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="52089-206">페이징의 일부분으로 수행하는 추가 roledefinition 호출을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-206">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="52089-207">Get-AzureRmRoleAssignment cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="52089-207">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="52089-208">-ExpandPrincipalGroups 명령 매개 변수 기능 수정</span><span class="sxs-lookup"><span data-stu-id="52089-208">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="52089-209">'Get-AzureRmResource'에서 '-ResourceType' 매개 변수가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="52089-209">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="52089-210">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="52089-210">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="52089-211">top 및 skip 매개 변수가 cmdlet 목록을 나열하도록 추가</span><span class="sxs-lookup"><span data-stu-id="52089-211">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="52089-212">표준을 프리미엄 네임스페이스 마이그레이션 cmdlet에 추가</span><span class="sxs-lookup"><span data-stu-id="52089-212">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="52089-213">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="52089-213">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="52089-214">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="52089-214">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="52089-215">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="52089-215">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="52089-216">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="52089-216">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="52089-217">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="52089-217">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="52089-218">PSServiceBusDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="52089-218">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="52089-219">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="52089-219">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="52089-220">‘New-AzureRmServiceFabricCluster’에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-220">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="52089-221">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="52089-221">AzureRM.Sql</span></span>
* <span data-ttu-id="52089-222">Management.Sql에 대한 새 cmdlet을 추가하여 고객이 TDE 인증서를 SQL Server 인스턴스 또는 Managed Instance에 추가할 수 있도록 허용</span><span class="sxs-lookup"><span data-stu-id="52089-222">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="52089-223">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="52089-223">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="52089-224">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="52089-224">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="52089-225">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="52089-225">AzureRM.Websites</span></span>
* <span data-ttu-id="52089-226">`Set-AzureRmWebApp -AssignIdentity` 및 `Set-AzureRmWebAppSlot -AssignIdentity`가 false로 설정되면 사이트 개체에서 Identity 속성이 제거됩니다. 미리보기 태그도 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="52089-226">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="52089-227">`Get-AzureRmWebAppMetrics`, `Get-AzureRmAppServicePlanMetrics` 예제가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="52089-227">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="52089-228">`Set-AzureRmWebApp -PhpVersion`이 유효한 php 버전으로 해제 지원</span><span class="sxs-lookup"><span data-stu-id="52089-228">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="52089-229">6.4.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="52089-229">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="52089-230">일반</span><span class="sxs-lookup"><span data-stu-id="52089-230">General</span></span>
* <span data-ttu-id="52089-231">대부분의 모듈에 대한 도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="52089-231">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="52089-232">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="52089-232">AzureRM.Profile</span></span>
* <span data-ttu-id="52089-233">기본 출력 형식에 추가된 Ps1Xml 특성</span><span class="sxs-lookup"><span data-stu-id="52089-233">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="52089-234">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="52089-234">AzureRM.Compute</span></span>
* <span data-ttu-id="52089-235">VMSS에 대한 IP 태그 기능</span><span class="sxs-lookup"><span data-stu-id="52089-235">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="52089-236">'New-AzureRmVmssIpTagConfig' cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="52089-236">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="52089-237">New-AzureRmVmssIpConfig에 IpTag 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="52089-237">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="52089-238">VMSS에 대한 자동 OS 롤백 기능</span><span class="sxs-lookup"><span data-stu-id="52089-238">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="52089-239">New-AzureRmVmssConfig 및 Update-AzureRmVmss에 DisableAutoRollback 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="52089-239">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="52089-240">Vmss에 대한 OS 업그레이드 기록 기능</span><span class="sxs-lookup"><span data-stu-id="52089-240">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="52089-241">Get-AzureRmVmss에 OSUpgradeHistory 스위치 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="52089-241">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="52089-242">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="52089-242">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="52089-243">다음 명령을 통해 카탈로그 액세스 제어 목록에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-243">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="52089-244">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="52089-244">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="52089-245">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="52089-245">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="52089-246">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="52089-246">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="52089-247">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="52089-247">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="52089-248">Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl에 대한 취소 지원 및 진행률 추적 추가</span><span class="sxs-lookup"><span data-stu-id="52089-248">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="52089-249">Export-AzureRmDataLakeStoreChildItemProperties에 대한 취소 지원 추가</span><span class="sxs-lookup"><span data-stu-id="52089-249">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="52089-250">재귀 작업을 수행하는 cmdlet에 대한 디버그 메시지 플러시 수정</span><span class="sxs-lookup"><span data-stu-id="52089-250">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="52089-251">DataLake cmdlet의 테스트 위치 수정</span><span class="sxs-lookup"><span data-stu-id="52089-251">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="52089-252">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="52089-252">AzureRM.EventHub</span></span>
* <span data-ttu-id="52089-253">목록 작업 cmdlet Get-AzureRmEventHub 및 Get-AzureRmEventHubConsumerGroup에 선택적 MaxCount 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="52089-253">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="52089-254">새 EventHub 만드는 동안 하나 이상의 매개 변수가 필요한 New-AzureRmEventHub cmdlet 문제를 해결.</span><span class="sxs-lookup"><span data-stu-id="52089-254">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="52089-255">기본 매개 변수 집합을 제공.</span><span class="sxs-lookup"><span data-stu-id="52089-255">Provided Default Parameter set.</span></span>
* <span data-ttu-id="52089-256">선택적 매개 변수 -KeyValue를 New-AzureRmEventHubKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-256">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="52089-257">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="52089-257">AzureRM.KeyVault</span></span>
* <span data-ttu-id="52089-258">Get-AzureRmKeyVault -Tag 실행 시 모든 리소스가 리턴되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="52089-258">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="52089-259">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="52089-259">AzureRM.Network</span></span>
* <span data-ttu-id="52089-260">영역 중복 VirtualNetworkGateways에 대한 새 Sku를 노출합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-260">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="52089-261">기능에 대한 새 명령이 추가됨: ARM을 통한 ExpressRoute Partner APIs</span><span class="sxs-lookup"><span data-stu-id="52089-261">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="52089-262">Get- AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="52089-262">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="52089-263">Set-AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="52089-263">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="52089-264">Add-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="52089-264">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="52089-265">Get-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="52089-265">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="52089-266">Remove-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="52089-266">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="52089-267">Get-AzureRMExpressRouteCrossConnectionArpTable 추가</span><span class="sxs-lookup"><span data-stu-id="52089-267">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="52089-268">Get-AzureRMExpressRouteCrossConnectionRouteTable 추가</span><span class="sxs-lookup"><span data-stu-id="52089-268">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="52089-269">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary 추가</span><span class="sxs-lookup"><span data-stu-id="52089-269">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="52089-270">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="52089-270">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="52089-271">Get-AzureRmRecoveryServicesBackupStatus cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="52089-271">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="52089-272">이 cmdlet은 VM ID를 가져와서 VM이 구독에서 일부 자격 증명 모음으로 보호되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-272">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="52089-273">이러한 자격 증명 모음이 존재하는 경우 cmdlet은 자격 증명 모음 세부 정보를 출력 합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-273">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="52089-274">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="52089-274">AzureRM.Resources</span></span>
* <span data-ttu-id="52089-275">Get-AzureRmPolicyAssignment cmdlet을 다음과 같이 업데이트함.</span><span class="sxs-lookup"><span data-stu-id="52089-275">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="52089-276">관리 그룹 수준에서 -Scope 값 리스팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="52089-276">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="52089-277">관리 그룹 수준에서 -Scope 값을 사용하여 개별 할당값을 검색하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="52089-277">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="52089-278">제어 매개 변수에 -Effective 및 -All 스위치 추가</span><span class="sxs-lookup"><span data-stu-id="52089-278">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="52089-279">Get/New/Remove/Set-AzureRmPolicyDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-279">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="52089-280">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="52089-280">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="52089-281">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="52089-281">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="52089-282">Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-282">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="52089-283">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="52089-283">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="52089-284">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="52089-284">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="52089-285">'New-AzureRmResourceGroupDeployment'에서 'TemplateParameterObject'를 사용하는 경우 매개 변수에 KeyVault 비밀 참조 지원 추가</span><span class="sxs-lookup"><span data-stu-id="52089-285">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="52089-286">'New-AzureRmADAppCredential'에 대해 '-EndDate' 매개 변수가 무시되는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="52089-286">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="52089-287">'Add-AzureRmADGroupMember'가 요청에 잘못된 URL을 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="52089-287">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="52089-288">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="52089-288">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="52089-289">선택적 매개 변수 -KeyValue를 New-AzureRmServiceBusKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-289">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="52089-290">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="52089-290">AzureRM.Sql</span></span>
* <span data-ttu-id="52089-291">New-AzureRmSqlDatabaseRestorePoint 도움말에서 SQLDW에 대한 사용자 정의 복원 지점 명시</span><span class="sxs-lookup"><span data-stu-id="52089-291">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="52089-292">몇 가지 cmdlet에서-ComputeGeneration 매개 변수의 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-292">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="52089-293">6.3.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="52089-293">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="52089-294">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="52089-294">AzureRM.Profile</span></span>
* <span data-ttu-id="52089-295">Enable-AzureRmContextAutoSave에 대한 오류 메시지 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="52089-295">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="52089-296">이전 컨텍스트 없이 'Connect-AzureRmAccount' 실행 시 각 구독에 대한 컨텍스트 생성</span><span class="sxs-lookup"><span data-stu-id="52089-296">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="52089-297">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="52089-297">Azure.Storage</span></span>
* <span data-ttu-id="52089-298">도움말 파일 내 -Permissions 매개 변수에 대한 추가 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="52089-298">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="52089-299">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="52089-299">AzureRM.Compute</span></span>
* <span data-ttu-id="52089-300">'Get-AzureRmVmDiskEncryptionStatus'가 데이터 디스크가 없는 VM에 대해 관찰된 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="52089-300">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="52089-301">Compute 클라이언트 라이브러리 버전을 업데이트하여 다음 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="52089-301">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="52089-302">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="52089-302">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="52089-303">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="52089-303">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="52089-304">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="52089-304">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="52089-305">다음 cmdlet이 '작업 ID' 및 '작업 상태'를 올바르게 표시하도록 수정:</span><span class="sxs-lookup"><span data-stu-id="52089-305">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="52089-306">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="52089-306">Start-AzureRmVM</span></span>
    - <span data-ttu-id="52089-307">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="52089-307">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="52089-308">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="52089-308">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="52089-309">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="52089-309">Set-AzureRmVM</span></span>
    - <span data-ttu-id="52089-310">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="52089-310">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="52089-311">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="52089-311">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="52089-312">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="52089-312">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="52089-313">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="52089-313">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="52089-314">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="52089-314">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="52089-315">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="52089-315">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="52089-316">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="52089-316">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="52089-317">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="52089-317">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="52089-318">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="52089-318">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="52089-319">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="52089-319">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="52089-320">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="52089-320">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="52089-321">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="52089-321">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="52089-322">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="52089-322">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="52089-323">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="52089-323">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="52089-324">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="52089-324">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="52089-325">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="52089-325">AzureRM.EventGrid</span></span>
* <span data-ttu-id="52089-326">Update-AzureRmEventGridSubscription cmdlet의 SubjectBeginsWith/SubjectEndsWith에 대한 ValidateNotNullOrEmpty 유효성 검사 조건을 제거하여 필요에 따라 이러한 매개 변수를 빈 문자열로 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-326">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="52089-327">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="52089-327">AzureRM.KeyVault</span></span>
* <span data-ttu-id="52089-328">Get-AzureRmKeyVault -Tag 실행 시 태그가 리턴되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="52089-328">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="52089-329">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="52089-329">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="52089-330">Policy Insights cmdlet의 공개 릴리스</span><span class="sxs-lookup"><span data-stu-id="52089-330">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="52089-331">API 버전 2018-04-04 사용</span><span class="sxs-lookup"><span data-stu-id="52089-331">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="52089-332">PolicyDefinitionReferenceId를 Get-AzureRmPolicyStateSummary의 결과 집합에 추가</span><span class="sxs-lookup"><span data-stu-id="52089-332">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="52089-333">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="52089-333">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="52089-334">-Vault 매개 변수를 RecoveryServices.Backup cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="52089-334">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="52089-335">전달되는 경우 이는 Set-AzureRmRecoveryServicesContext cmdlet을 재정의함.</span><span class="sxs-lookup"><span data-stu-id="52089-335">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="52089-336">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="52089-336">AzureRM.Sql</span></span>
* <span data-ttu-id="52089-337">Get-AzureRmSqlDatabaseExpanded에 대한 도움말 파일의 예가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="52089-337">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="52089-338">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="52089-338">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="52089-339">Add-AzureRmTrafficManagerEndpointConfig에대한 도움말 파일이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="52089-339">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="52089-340">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="52089-340">AzureRM.Websites</span></span>
* <span data-ttu-id="52089-341">-AssignIdentity를 사용할 때 AppSetting을 덮어쓰지 않도록 'Set-AzureRmWebApp'이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="52089-341">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="52089-342">'New-AzureRmWebAppSlot'이 AppServicePlan을 옵션 매개변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="52089-342">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="52089-343">6.2.1 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="52089-343">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="52089-344">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="52089-344">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="52089-345">PSWorkspace 모델이 Network 형식을 매개 변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="52089-345">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="52089-346">6.2.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="52089-346">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="52089-347">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="52089-347">AzureRM.Profile</span></span>
* <span data-ttu-id="52089-348">Newtonsoft.Json의 버전 10.0.3이 모듈 가져오기에 로드되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="52089-348">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="52089-349">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="52089-349">AzureRM.Compute</span></span>
* <span data-ttu-id="52089-350">VMSS VM 업데이트 기능</span><span class="sxs-lookup"><span data-stu-id="52089-350">VMSS VM Update feature</span></span>
    - <span data-ttu-id="52089-351">'Update-AzureRmVmssVM' 및 'New-AzureRmVMDataDisk' cmdlets 추가</span><span class="sxs-lookup"><span data-stu-id="52089-351">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="52089-352">데이터 디스크를 Vmss VM에 추가할 수 있도록 지원하기 위해 VirtualMachineScaleSetVM 매개변수를 'Add-AzureRmVMDataDisk' cmdlet에 추가하였습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-352">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="52089-353">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="52089-353">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="52089-354">ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.8.0-preview로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-354">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="52089-355">팩터리 리포지토리 작업 구성 추가</span><span class="sxs-lookup"><span data-stu-id="52089-355">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="52089-356">QuickBooks LinkedService가 ConsumerKey 및 consumerSecret 속성을 노출하도록 업데이트됨 </span><span class="sxs-lookup"><span data-stu-id="52089-356">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="52089-357">여러 모델 유형을 SecretBase에서 개체로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="52089-357">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="52089-358">Blob 이벤트 트리거 추가</span><span class="sxs-lookup"><span data-stu-id="52089-358">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="52089-359">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="52089-359">AzureRM.KeyVault</span></span>
* <span data-ttu-id="52089-360">예제 출력으로 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-360">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="52089-361">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="52089-361">AzureRM.Network</span></span>
* <span data-ttu-id="52089-362">Network Watcher cmdlet에서 트래픽 분석 매개 변수를 사용가능하도록 설정</span><span class="sxs-lookup"><span data-stu-id="52089-362">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="52089-363">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="52089-363">AzureRM.Resources</span></span>
* <span data-ttu-id="52089-364">'Get AzureRmResource'에서 반환된 'PSResource' 개체의 'Properties' 속성의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="52089-364">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="52089-365">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="52089-365">AzureRM.Scheduler</span></span>
* <span data-ttu-id="52089-366">ServiceBusQueueJob 업데이트가 새 인증 값을 설정하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="52089-366">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="52089-367">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="52089-367">AzureRM.Sql</span></span>
* <span data-ttu-id="52089-368">옵션 LicenseType 매개 변수를 사용하여 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="52089-368">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="52089-369">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="52089-369">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="52089-370">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="52089-370">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="52089-371">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="52089-371">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="52089-372">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="52089-372">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="52089-373">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="52089-373">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="52089-374">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="52089-374">AzureRM.Websites</span></span>
* <span data-ttu-id="52089-375">'New-AzureRMWebApp'이 전략 라이브러리의 공통 알고리즘을 사용하도록 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-375">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="52089-376">6.1.0 - 2018년 5월</span><span class="sxs-lookup"><span data-stu-id="52089-376">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="52089-377">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="52089-377">AzureRM.Profile</span></span>
* <span data-ttu-id="52089-378">'Clear-AzureRmContext'를 실행하면 이전 기본 컨텍스트의 이름으로 빈 컨텍스트가 유지되어 사용자가 이전 이름으로 새 컨텍스트를 만들지 못하게 되는 문제를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-378">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="52089-379">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="52089-379">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="52089-380">AS에서 게이트웨이가 작업을 연결하거나 연결 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-380">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="52089-381">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="52089-381">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="52089-382">ApiVersions, ApiReleases 및 ApiRevisions에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="52089-382">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="52089-383">ServiceFabric 백 엔드에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="52089-383">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="52089-384">Application Insights 로거에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="52089-384">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="52089-385">'기본' SKU를 API Management 서비스의 유효한 SKU로 인식하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="52089-385">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="52089-386">개인 CA가 발급한 인증서를 루트 또는 CA로 설치하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="52089-386">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="52089-387">KeyVault 및 다중 프록시 호스트 이름을 통한 사용자 정의 SSL 인증서를 수락하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="52089-387">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="52089-388">MSI ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="52089-388">Added support for MSI identity</span></span>
* <span data-ttu-id="52089-389">URL을 통한 정책을 수락하는 지원 추가됨 참고: 다음 cmdlet은 이후 릴리스에서 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-389">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="52089-390">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="52089-390">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="52089-391">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="52089-391">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="52089-392">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="52089-392">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="52089-393">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="52089-393">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="52089-394">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="52089-394">AzureRM.Batch</span></span>
* <span data-ttu-id="52089-395">새 cmdlet Get AzureBatchPoolNodeCounts 릴리스</span><span class="sxs-lookup"><span data-stu-id="52089-395">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="52089-396">새 cmdlet Start-AzureBatchComputeNodeServiceLogUpload 릴리스</span><span class="sxs-lookup"><span data-stu-id="52089-396">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="52089-397">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="52089-397">AzureRM.Consumption</span></span>
* <span data-ttu-id="52089-398">Expand, ResourceGroup, InstanceName, InstanceId, Tags, Top on Cmdlet Get-AzureRmConsumptionUsageDetail 등 새 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="52089-398">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="52089-399">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="52089-399">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="52089-400">Export-AzureRmDataLakeStoreChildItemProperties에 대한 예제 수정</span><span class="sxs-lookup"><span data-stu-id="52089-400">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="52089-401">Set-AzureRmDataLakeStoreItemAclEntry에서 재귀 사례에 대한 null 매개 변수 예외 수정</span><span class="sxs-lookup"><span data-stu-id="52089-401">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="52089-402">Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry에 대한 도움말 파일 수정</span><span class="sxs-lookup"><span data-stu-id="52089-402">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="52089-403">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="52089-403">AzureRM.Network</span></span>
* <span data-ttu-id="52089-404">18.0.0-preview에서 19.0.0-preview로 네트워크 SDK 버전 업그레이드</span><span class="sxs-lookup"><span data-stu-id="52089-404">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="52089-405">프로토콜 구성을 만들기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="52089-405">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="52089-406">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="52089-406">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="52089-407">기존 Express 경로 회로에 새 회로 연결을 추가하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="52089-407">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="52089-408">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="52089-408">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="52089-409">기존 Express 경로 회로에서 회로 연결을 제거하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="52089-409">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="52089-410">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="52089-410">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="52089-411">회로 연결을 검색하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="52089-411">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="52089-412">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="52089-412">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="52089-413">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="52089-413">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="52089-414">생성된 인증서로 고정 서버 인증 사용(문제 # 5998)</span><span class="sxs-lookup"><span data-stu-id="52089-414">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="52089-415">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="52089-415">AzureRM.Sql</span></span>
* <span data-ttu-id="52089-416">AuditActions 또는 AuditActionGroups를 제거할 수 있도록 업데이트된 감사 cmdlet</span><span class="sxs-lookup"><span data-stu-id="52089-416">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="52089-417">'Azure 복구 서비스 자격 증명 모음을 사용하여 장기 보존 정책을 구성하면 정책이 더 이상 지원되지 않습니다. 새로운 유연 보유 정책으로 요청을 제출하십시오.'라는 메시지와 함께 명령이 실패하는 새로운 유연 보유 정책을 설정할 때</span><span class="sxs-lookup"><span data-stu-id="52089-417">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="52089-418">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy의 문제 수정</span><span class="sxs-lookup"><span data-stu-id="52089-418">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="52089-419">Azure SQL Database/ElasticPool Creation/Update 관련 cmdlet을 모두 업데이트하여 규모 및 계층 관련 속성에 대한 SKU 속성을 지원하는 새 데이터베이스 API를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-419">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="52089-420">업데이트된 cmdlet는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="52089-420">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="52089-421">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="52089-421">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="52089-422">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="52089-422">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="52089-423">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="52089-423">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="52089-424">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="52089-424">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="52089-425">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="52089-425">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="52089-426">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="52089-426">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="52089-427">-Name 매개 변수를 사용할 때 -ResourceGroupName 매개 변수가 필요하도록 'Get-AzureRmTrafficManagerProfile'에 대한 매개 변수를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="52089-427">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>