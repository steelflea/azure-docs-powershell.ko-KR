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
ms.date: 2/20/2018
ms.openlocfilehash: 985e0fbaa2da73b398d4c574515bcbab5b1a16e0
ms.sourcegitcommit: 15bf69bf95eceb936b3a429e741add95c308826a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/28/2018
---
# <a name="release-notes"></a><span data-ttu-id="68791-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="68791-103">Release notes</span></span>

<span data-ttu-id="68791-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---

## <a name="560---march-2018"></a><span data-ttu-id="68791-105">5.6.0 - 2018년 3월</span><span class="sxs-lookup"><span data-stu-id="68791-105">5.6.0 - March 2018</span></span>

#### <a name="general"></a><span data-ttu-id="68791-106">일반</span><span class="sxs-lookup"><span data-stu-id="68791-106">General</span></span>
* <span data-ttu-id="68791-107">CloudShell의 기본 리소스 그룹 문제 수정</span><span class="sxs-lookup"><span data-stu-id="68791-107">Fix issue with Default Resource Group in CloudShell</span></span>
* <span data-ttu-id="68791-108">모듈 가져오는 중에 잘못된 시작 스크립트가 실행되는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="68791-108">Fix issue where incorrect startup scripts were being executed during module import</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="68791-109">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="68791-109">AzureRM.Profile</span></span>
* <span data-ttu-id="68791-110">지원되지 않는 시나리오에서 MSI 인증 사용</span><span class="sxs-lookup"><span data-stu-id="68791-110">Enable MSI authentication in unsupported scenarios</span></span>
* <span data-ttu-id="68791-111">사용자 정의 관리 서비스 ID 지원 추가</span><span class="sxs-lookup"><span data-stu-id="68791-111">Add support for user-defined Managed Service Identity</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="68791-112">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="68791-112">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="68791-113">빌드 시 스크립트 정리 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="68791-113">Fixed issue with cleaning up scripts in build</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="68791-114">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="68791-114">AzureRM.Cdn</span></span>
* <span data-ttu-id="68791-115">빌드 시 스크립트 정리 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="68791-115">Fixed issue with cleaning up scripts in build</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="68791-116">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="68791-116">AzureRM.Compute</span></span>
* <span data-ttu-id="68791-117">'New-AzureRmVM' 및 'New-AzureRmVMSS'가 데이터 디스크를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-117">'New-AzureRmVM' and 'New-AzureRmVMSS' support data disks.</span></span>
* <span data-ttu-id="68791-118">'New-AzureRmVM' 및 'New-AzureRmVMSS'가 이름별 또는 ID별로 사용자 지정 이미지를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-118">'New-AzureRmVM' and 'New-AzureRmVMSS' support custom image by name or by id.</span></span>
* <span data-ttu-id="68791-119">로그 분석 기능</span><span class="sxs-lookup"><span data-stu-id="68791-119">Log analytic feature</span></span>
    - <span data-ttu-id="68791-120">'Export-AzureRmLogAnalyticRequestRateByInterval' cmdlet 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-120">Added 'Export-AzureRmLogAnalyticRequestRateByInterval' cmdlet</span></span>
    - <span data-ttu-id="68791-121">'Export-AzureRmLogAnalyticThrottledRequests' cmdlet 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-121">Added 'Export-AzureRmLogAnalyticThrottledRequests' cmdlet</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="68791-122">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="68791-122">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="68791-123">컨테이너 레지스트리 및 Azure 파일 볼륨 마운트에 대한 매개 변수 세트 문제 수정</span><span class="sxs-lookup"><span data-stu-id="68791-123">Fix parameter sets issue for container registry and azure file volume mount</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="68791-124">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="68791-124">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="68791-125">ADF .Net SDK를 다음과 같은 변경 사항이 포함된 버전 0.6.0-preview로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-125">Updated the ADF .Net SDK to version 0.6.0-preview containing the following changes:</span></span>
    - <span data-ttu-id="68791-126">새로운 AzureDatabricks LinkedService 및 DatabricksNotebook Activity 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-126">Added new AzureDatabricks LinkedService and DatabricksNotebook Activity</span></span>
    - <span data-ttu-id="68791-127">HDInsightOnDemand LinkedService의 headNodeSize 및 dataNodeSize 속성 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-127">Added headNodeSize and dataNodeSize properties in HDInsightOnDemand LinkedService</span></span>
    - <span data-ttu-id="68791-128">SalesforceMarketingCloud에 대한 LinkedService, Dataset, CopySource 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-128">Added LinkedService, Dataset, CopySource for SalesforceMarketingCloud</span></span>
    - <span data-ttu-id="68791-129">모든 작업에서 SecureOutput에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-129">Added support for SecureOutput on all activities</span></span>
    - <span data-ttu-id="68791-130">ForEach 작업에서 실행될 동시 작업 수를 제어하는 새로운 BatchCount 속성 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-130">Added new BatchCount property on ForEach activity which control how many concurrent activities to run</span></span>
    - <span data-ttu-id="68791-131">새 필터 작업 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-131">Added new Filter Activity</span></span>
    - <span data-ttu-id="68791-132">연결된 서비스 매개 변수 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-132">Added Linked Service Parameters support</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="68791-133">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="68791-133">AzureRM.Dns</span></span>
* <span data-ttu-id="68791-134">사설 DNS 영역 지원(공개 미리 보기)</span><span class="sxs-lookup"><span data-stu-id="68791-134">Support for Private DNS Zones (Public Preview)</span></span>
    - <span data-ttu-id="68791-135">연결된 가상 네트워크에만 표시되는 DNS 영역을 만들 수있는 기능을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-135">Adds ability to create DNS zones that are visible only to the associated virtual networks</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="68791-136">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="68791-136">AzureRM.Network</span></span>
* <span data-ttu-id="68791-137">DNS cmdlet과의 호환성을 위해 모델 형식 업데이트.</span><span class="sxs-lookup"><span data-stu-id="68791-137">Updating model types for compatibility with DNS cmdlets.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="68791-138">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="68791-138">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="68791-139">ASR Azure-Azure Site Recovery에 대한 변경 사항(cmdlet은 현재 Enterprise-Enterprise, Enterprise-Azure, HyperV-Azure, VMware - Azure에 대한 작업을 지원)</span><span class="sxs-lookup"><span data-stu-id="68791-139">Changes for ASR Azure to Azure Site Recovery (cmdlets are currently supporting operations for Enterprise to Enterprise, Enterprise to Azure, HyperV to Azure,VMware to Azure)</span></span>
    - <span data-ttu-id="68791-140">New-AzureRmRecoveryServicesAsrProtectionContainer</span><span class="sxs-lookup"><span data-stu-id="68791-140">New-AzureRmRecoveryServicesAsrProtectionContainer</span></span>
    - <span data-ttu-id="68791-141">New-AzureRmRecoveryServicesAsrAzureToAzureDiskReplicationConfig</span><span class="sxs-lookup"><span data-stu-id="68791-141">New-AzureRmRecoveryServicesAsrAzureToAzureDiskReplicationConfig</span></span>
    - <span data-ttu-id="68791-142">Remove-AzureRmRecoveryServicesAsrProtectionContainer</span><span class="sxs-lookup"><span data-stu-id="68791-142">Remove-AzureRmRecoveryServicesAsrProtectionContainer</span></span>
    - <span data-ttu-id="68791-143">Update-AzureRmRecoveryServicesAsrProtectionDirection</span><span class="sxs-lookup"><span data-stu-id="68791-143">Update-AzureRmRecoveryServicesAsrProtectionDirection</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="68791-144">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="68791-144">AzureRM.Storage</span></span>
* <span data-ttu-id="68791-145">new 및 set Storage Account cmdlet에서 Encryption at Rest는 기본적으로 활성화되며 비활성화할 수 없으므로 EnableEncryptionService 및 DisableEncryptionService 같은 매개 변수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="68791-145">Obsolete following parameters in new and set Storage Account cmdlets: EnableEncryptionService and DisableEncryptionService, since Encryption at Rest is enabled by default and can't be disabled.</span></span>
    - <span data-ttu-id="68791-146">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="68791-146">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="68791-147">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="68791-147">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="68791-148">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="68791-148">AzureRM.Websites</span></span>
* <span data-ttu-id="68791-149">Remove-AzureRmWebAppSlot에 대한 도움말 수정됨</span><span class="sxs-lookup"><span data-stu-id="68791-149">Fixed the help for Remove-AzureRmWebAppSlot</span></span>

## <a name="550---march-2018"></a><span data-ttu-id="68791-150">5.5.0 - 2018년 3월</span><span class="sxs-lookup"><span data-stu-id="68791-150">5.5.0 - March 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="68791-151">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="68791-151">AzureRM.Profile</span></span>
* <span data-ttu-id="68791-152">별칭 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-152">Fixed issue with importing aliases</span></span>
* <span data-ttu-id="68791-153">6.0.8 버전과 병렬로 Newtonsoft.Json 버전 10.0.3 로드</span><span class="sxs-lookup"><span data-stu-id="68791-153">Load version 10.0.3 of Newtonsoft.Json side-by-side with version 6.0.8</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="68791-154">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="68791-154">Azure.Storage</span></span>
* <span data-ttu-id="68791-155">일시 삭제 기능 지원</span><span class="sxs-lookup"><span data-stu-id="68791-155">Support Soft-Delete feature</span></span>
    - <span data-ttu-id="68791-156">Enable-AzureStorageDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="68791-156">Enable-AzureStorageDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="68791-157">Enable-AzureStorageDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="68791-157">Disable-AzureStorageDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="68791-158">Get-AzureStorageBlob</span><span class="sxs-lookup"><span data-stu-id="68791-158">Get-AzureStorageBlob</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="68791-159">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="68791-159">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="68791-160">별칭 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-160">Fixed issue with importing aliases</span></span>
* <span data-ttu-id="68791-161">2017-08-01 API 버전 지원 및 방화벽과 쿼리 스케일 아웃 기능 지원 추가</span><span class="sxs-lookup"><span data-stu-id="68791-161">Add support of firewall and query scaleout feature, as well as support of 2017-08-01 api version.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="68791-162">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="68791-162">AzureRM.Automation</span></span>
* <span data-ttu-id="68791-163">별칭 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-163">Fixed issue with importing aliases</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="68791-164">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="68791-164">AzureRM.Cdn</span></span>
* <span data-ttu-id="68791-165">별칭 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-165">Fixed issue with importing aliases</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="68791-166">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="68791-166">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="68791-167">notice.txt 및 알림 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="68791-167">Update notice.txt and notice message.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="68791-168">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="68791-168">AzureRM.Compute</span></span>
* <span data-ttu-id="68791-169">'New-AzureRmVMSS'가 자세한 정보 표시 모드로 연결 문자열 인쇄</span><span class="sxs-lookup"><span data-stu-id="68791-169">'New-AzureRmVMSS' prints connection strings in verbose mode.</span></span>
* <span data-ttu-id="68791-170">'New-AzureRmVmss'가 공용 IP 주소, 부하 분산 규칙, 인바운드 NAT 규칙 지원</span><span class="sxs-lookup"><span data-stu-id="68791-170">'New-AzureRmVmss' supports public IP address, load balancing rules, inbound NAT rules.</span></span>
* <span data-ttu-id="68791-171">WriteAccelerator 기능</span><span class="sxs-lookup"><span data-stu-id="68791-171">WriteAccelerator feature</span></span>
    - <span data-ttu-id="68791-172">WriteAccelerator 스위치 매개 변수가 다음 cmdlets에 추가됨: Set-AzureRmVMOSDisk Set-AzureRmVMDataDisk Add-AzureRmVMDataDisk Add-AzureRmVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="68791-172">Added WriteAccelerator switch parameter to the following cmdlets: Set-AzureRmVMOSDisk Set-AzureRmVMDataDisk Add-AzureRmVMDataDisk Add-AzureRmVmssDataDisk</span></span>
    - <span data-ttu-id="68791-173">OsDiskWriteAccelerator 스위치 매개 변수가 다음 cmdlet에 추가됨:   Set-AzureRmVmssStorageProfile.</span><span class="sxs-lookup"><span data-stu-id="68791-173">Added OsDiskWriteAccelerator switch parameter to the following cmdlet:     Set-AzureRmVmssStorageProfile.</span></span>
    - <span data-ttu-id="68791-174">OsDiskWriteAccelerator 부울 매개 변수가 다음 cmdlet에 추가됨:     Update-AzureRmVM     Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="68791-174">Added OsDiskWriteAccelerator Boolean parameter to the following cmdlets:     Update-AzureRmVM     Update-AzureRmVmss</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="68791-175">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="68791-175">AzureRM.DataFactories</span></span>
* <span data-ttu-id="68791-176">일부 암호화 작업에 대해 의미 없는 오류를 일으키는 자격 증명 암호화 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-176">Fix credential encryption issue that caused no meaningful error for some encryption operations</span></span>
* <span data-ttu-id="68791-177">데이터 팩터리 전체에서 공유 가능하도록 통합 런타임 활성화</span><span class="sxs-lookup"><span data-stu-id="68791-177">Enable integration runtime to be shared across data factory</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="68791-178">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="68791-178">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="68791-179">"Set-AzureRmDataFactoryV2IntegrationRuntime" cmd용 매개 변수 "SetupScriptContainerSasUri" 및 "Edition"을 추가하여 사용자 지정 설치 및 버전 선택 기능 활성화</span><span class="sxs-lookup"><span data-stu-id="68791-179">Add parameter "SetupScriptContainerSasUri" and "Edition" for "Set-AzureRmDataFactoryV2IntegrationRuntime" cmd to enable custom setup and edition selection functionality</span></span>
* <span data-ttu-id="68791-180">일부 암호화 작업에 대해 의미 없는 오류를 일으키는 자격 증명 암호화 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-180">Fix credential encryption issue that caused no meaningful error for some encryption operations.</span></span>
* <span data-ttu-id="68791-181">데이터 팩터리 전체에서 공유 가능하도록 통합 런타임 활성화</span><span class="sxs-lookup"><span data-stu-id="68791-181">Enable integration runtime to be shared across data factory</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="68791-182">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="68791-182">AzureRM.HDInsight</span></span>
* <span data-ttu-id="68791-183">별칭 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-183">Fixed issue with importing aliases</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="68791-184">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="68791-184">AzureRM.KeyVault</span></span>
* <span data-ttu-id="68791-185">Set-AzureRmKeyVaultAccessPolicy용 예제 수정</span><span class="sxs-lookup"><span data-stu-id="68791-185">Fixed example for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="68791-186">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="68791-186">AzureRM.Network</span></span>
* <span data-ttu-id="68791-187">별칭 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-187">Fixed issue with importing aliases</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="68791-188">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="68791-188">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="68791-189">별칭 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-189">Fixed issue with importing aliases</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="68791-190">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="68791-190">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="68791-191">별칭 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-191">Fixed issue with importing aliases</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="68791-192">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="68791-192">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="68791-193">별칭 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-193">Fixed issue with importing aliases</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="68791-194">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="68791-194">AzureRM.Resources</span></span>
* <span data-ttu-id="68791-195">별칭 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-195">Fixed issue with importing aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="68791-196">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="68791-196">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="68791-197">큐에 EnableBatchedOperations 속성 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-197">Added EnableBatchedOperations property to Queue</span></span>
* <span data-ttu-id="68791-198">구독에 DeadLetteringOnFilterEvaluationExceptions 속성 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-198">Added DeadLetteringOnFilterEvaluationExceptions property to Subscriptions</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="68791-199">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="68791-199">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="68791-200">Service Fabric cmdlet 새로 고침</span><span class="sxs-lookup"><span data-stu-id="68791-200">Service Fabric cmdlet refresh</span></span>
  - <span data-ttu-id="68791-201">ARM 템플릿 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="68791-201">Updated ARM templates</span></span>
  - <span data-ttu-id="68791-202">실패한 작업이 더 이상 롤백되지 않음</span><span class="sxs-lookup"><span data-stu-id="68791-202">Failed operations no longer rollback</span></span>
  - <span data-ttu-id="68791-203">Add-AzureRmServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="68791-203">Add-AzureRmServiceFabricNodeType</span></span>
    - <span data-ttu-id="68791-204">관리 디스크에 대한 VM 기본값</span><span class="sxs-lookup"><span data-stu-id="68791-204">VMs default to managed disks</span></span>
    - <span data-ttu-id="68791-205">기존 VMSS 서브넷 사용됨</span><span class="sxs-lookup"><span data-stu-id="68791-205">Existing VMSS subnet used</span></span>
    - <span data-ttu-id="68791-206">모든 작업은 idempotent임</span><span class="sxs-lookup"><span data-stu-id="68791-206">All operations are idempotent</span></span>
  - <span data-ttu-id="68791-207">Remove-AzureRmServiceFabricNodeType 정리가 부분적으로 VMSS 및/또는 클러스터 노드 유형 생성</span><span class="sxs-lookup"><span data-stu-id="68791-207">Remove-AzureRmServiceFabricNodeType cleans up partially created VMSS and/or cluster node types</span></span>
  - <span data-ttu-id="68791-208">복합 속성 유형에 대한 PSCluster 개체의 출력 수정</span><span class="sxs-lookup"><span data-stu-id="68791-208">Fixed output of PSCluster object for complex property types</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="68791-209">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="68791-209">AzureRM.Sql</span></span>
* <span data-ttu-id="68791-210">별칭 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-210">Fixed issue with importing aliases</span></span>
* <span data-ttu-id="68791-211">Get-AzureRmSqlServer, New-AzureRmSqlServer 및 Remove-AzureRmSqlServer 응답이 FullyQualifiedDomainName 속성에 포함됨.</span><span class="sxs-lookup"><span data-stu-id="68791-211">Get-AzureRmSqlServer, New-AzureRmSqlServer, and Remove-AzureRmSqlServer response now includes FullyQualifiedDomainName property.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="68791-212">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="68791-212">AzureRM.Websites</span></span>
* <span data-ttu-id="68791-213">별칭 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-213">Fixed issue with importing aliases</span></span>
* <span data-ttu-id="68791-214">New-AzureRMWebApp - 로컬 Git 리포지토리 지원과 함께 간소화된 WebApp 생성을 위한 매개 변수 집합이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-214">New-AzureRMWebApp - added parameter set for simplified WebApp creation, with local git repository support.</span></span>

## <a name="540---february-2018"></a><span data-ttu-id="68791-215">5.4.0 - 2018년 2월</span><span class="sxs-lookup"><span data-stu-id="68791-215">5.4.0 - February 2018</span></span>
#### <a name="azurermautomation"></a><span data-ttu-id="68791-216">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="68791-216">AzureRM.Automation</span></span>
* <span data-ttu-id="68791-217">New-AzureRmAutomationModule의 별칭이 Import-AzureRmAutomationModule에 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-217">Added alias from New-AzureRmAutomationModule to Import-AzureRmAutomationModule</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="68791-218">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="68791-218">AzureRM.Compute</span></span>
* <span data-ttu-id="68791-219">일부 Get cmdlet에 대한 ErrorAction 문제 해결</span><span class="sxs-lookup"><span data-stu-id="68791-219">Fix ErrorAction issue for some of Get cmdlets.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="68791-220">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="68791-220">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="68791-221">Azure Container Instance SDK 2018-02-01 적용</span><span class="sxs-lookup"><span data-stu-id="68791-221">Apply Azure Container Instance SDK 2018-02-01</span></span>
    - <span data-ttu-id="68791-222">DNS 이름 레이블 지원</span><span class="sxs-lookup"><span data-stu-id="68791-222">Support DNS name label</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="68791-223">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="68791-223">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="68791-224">이전에 작동하지 않았던 모든 GET cmdlet이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-224">Fixed all of the GET cmdlets which previously weren't working.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="68791-225">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="68791-225">AzureRM.EventHub</span></span>
* <span data-ttu-id="68791-226">Get-AzureRmEventHubGeoDRConfiguration 도움말의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="68791-226">Fix bug in Get-AzureRmEventHubGeoDRConfiguration help</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="68791-227">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="68791-227">AzureRM.Network</span></span>
* <span data-ttu-id="68791-228">새 연결 모니터를 만드는 cmdlet이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-228">Added cmdlet to create a new connection monitor</span></span>
    - <span data-ttu-id="68791-229">New-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="68791-229">New-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="68791-230">연결 모니터를 업데이트하는 cmdlet이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-230">Added cmdlet to update a connection monitor</span></span>
    - <span data-ttu-id="68791-231">Set-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="68791-231">Set-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="68791-232">연결 모니터 또는 연결 모니터 목록을 가져오는 cmdlet이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-232">Added cmdlet to get connection monitor or connection monitor list</span></span>
    - <span data-ttu-id="68791-233">Get-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="68791-233">Get-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="68791-234">연결 모니터를 쿼리하는 cmdlet이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-234">Added cmdlet to query connection monitor</span></span>
    - <span data-ttu-id="68791-235">Get-AzureRmNetworkWatcherConnectionMonitorReport</span><span class="sxs-lookup"><span data-stu-id="68791-235">Get-AzureRmNetworkWatcherConnectionMonitorReport</span></span>
* <span data-ttu-id="68791-236">연결 모니터를 시작하는 cmdlet이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-236">Added cmdlet to start connection monitor</span></span>
    - <span data-ttu-id="68791-237">Start-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="68791-237">Start-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="68791-238">연결 모니터를 중지하는 cmdlet이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-238">Added cmdlet to stop connection monitor</span></span>
    - <span data-ttu-id="68791-239">Stop-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="68791-239">Stop-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="68791-240">연결 모니터를 제거하는 cmdlet이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-240">Added cmdlet to remove connection monitor</span></span>
    - <span data-ttu-id="68791-241">Remove-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="68791-241">Remove-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="68791-242">사용되지 않는 예제를 제거하기 위해 Set-AzureRmApplicationGatewayBackendAddressPool 설명서가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="68791-242">Updated Set-AzureRmApplicationGatewayBackendAddressPool documentation to remove deprecated example</span></span>
* <span data-ttu-id="68791-243">Application Gateway에 EnableHttp2 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-243">Added EnableHttp2 flag to Application Gateway</span></span>
    - <span data-ttu-id="68791-244">New-AzureRmApplicationGateway가 업데이트됨: 선택적 매개 변수 -EnableHttp2가 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-244">Updated New-AzureRmApplicationGateway: Added optional parameter -EnableHttp2</span></span>
* <span data-ttu-id="68791-245">PublicIpAddress에 IpTags 추가</span><span class="sxs-lookup"><span data-stu-id="68791-245">Add IpTags to PublicIpAddress</span></span>
    - <span data-ttu-id="68791-246">New-AzureRmPublicIpAddress가 업데이트됨: IpTags가 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-246">Updated New-AzureRmPublicIpAddress: Added IpTags</span></span>
    - <span data-ttu-id="68791-247">Iptag를 추가하는 New-AzureRmPublicIpTag</span><span class="sxs-lookup"><span data-stu-id="68791-247">New-AzureRmPublicIpTag to add Iptag</span></span>
* <span data-ttu-id="68791-248">RouteTable 및 effectiveRoute에 DisableBgpRoutePropagation 속성을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-248">Add DisableBgpRoutePropagation property in RouteTable and effectiveRoute.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="68791-249">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="68791-249">AzureRM.Resources</span></span>
* <span data-ttu-id="68791-250">Register-AzureRmProviderFeature: 문서에 누락된 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-250">Register-AzureRmProviderFeature: Added missing example in the docs</span></span>
* <span data-ttu-id="68791-251">Register-AzureRmResourceProvider: 문서에 누락된 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-251">Register-AzureRmResourceProvider: Added missing example in the docs</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="68791-252">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="68791-252">AzureRM.Storage</span></span>
* <span data-ttu-id="68791-253">new 및 set Storage Account cmdlet에서 Encryption at Rest는 기본적으로 활성화되며 비활성화할 수 없으므로 EnableEncryptionService 및 DisableEncryptionService 같은 매개 변수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="68791-253">Obsolete following parameters in new and set Storage Account cmdlets: EnableEncryptionService and DisableEncryptionService, since Encryption at Rest is enabled by default and can't be disabled.</span></span>
    - <span data-ttu-id="68791-254">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="68791-254">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="68791-255">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="68791-255">Set-AzureRmStorageAccount</span></span>


## <a name="530---february-2018"></a><span data-ttu-id="68791-256">5.3.0 - 2018년 2월</span><span class="sxs-lookup"><span data-stu-id="68791-256">5.3.0 - February 2018</span></span>
### <a name="azurermprofile"></a><span data-ttu-id="68791-257">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="68791-257">AzureRM.Profile</span></span>
* <span data-ttu-id="68791-258">PowerShell 3 및 4에 대한 사용 중단 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-258">Added deprecation warning for PowerShell 3 and 4</span></span>
* <span data-ttu-id="68791-259">`Add-AzureRmAccount`는 `Connect-AzureRmAccount`로 이름이 변경되었습니다. 이전 cmdlet 이름에 대한 별칭이 추가되었고 다른 별칭(`Login-AzAccount` 및 `Login-AzureRmAccount`)이 새 cmdlet 이름으로 리디렉션되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-259">`Add-AzureRmAccount` has been renamed as `Connect-AzureRmAccount`; an alias has been added for the old cmdlet name, and other aliases (`Login-AzAccount` and `Login-AzureRmAccount`) have been redirected to the new cmdlet name.</span></span>
* <span data-ttu-id="68791-260">`Remove-AzureRmAccount`는 `Disconnect-AzureRmAccount`로 이름이 변경되었습니다. 이전 cmdlet 이름에 대한 별칭이 추가되었고 다른 별칭(`Logout-AzAccount` 및 `Logout-AzureRmAccount`)이 새 cmdlet 이름으로 리디렉션되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-260">`Remove-AzureRmAccount` has been renamed as `Disconnect-AzureRmAccount`; an alias has been added for the old cmdlet name, and other aliases (`Logout-AzAccount` and `Logout-AzureRmAccount`) have been redirected to the new cmdlet name.</span></span>
* <span data-ttu-id="68791-261">`Login-AzureRmAccount` 대신 `Connect-AzureRmAccount`를 사용하도록 리소스 문자열이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-261">Corrected Resource Strings to use `Connect-AzureRmAccount` instead of `Login-AzureRmAccount`</span></span>
* <span data-ttu-id="68791-262">`Add-AzureRmEnvironment` 및 `Set-AzureRmEnvironment`</span><span class="sxs-lookup"><span data-stu-id="68791-262">`Add-AzureRmEnvironment` and `Set-AzureRmEnvironment`</span></span>
  - <span data-ttu-id="68791-263">OperationalInsights 데이터 평면 RP와 함께 사용할 매개 변수로 `-AzureOperationalInsightsEndpoint` 및 `-AzureOperationalInsightsEndpointResourceId`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-263">Added `-AzureOperationalInsightsEndpoint` and `-AzureOperationalInsightsEndpointResourceId` as parameters for use with OperationalInsights data plane RP.</span></span>

### <a name="azurermanalysisservices"></a><span data-ttu-id="68791-264">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="68791-264">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="68791-265">`Connect-AzureRmAccount`를 사용하도록 `Login-AzureRmAccount`의 사용법이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-265">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

### <a name="azurermcompute"></a><span data-ttu-id="68791-266">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="68791-266">AzureRM.Compute</span></span>
* <span data-ttu-id="68791-267">간소화된 매개 변수 집합 `New-AzureRmVM`에 `-AvailabilitySetName` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-267">Added `-AvailabilitySetName` parameter to the simplified parameterset of `New-AzureRmVM`.</span></span>
* <span data-ttu-id="68791-268">`Connect-AzureRmAccount`를 사용하도록 `Login-AzureRmAccount`의 사용법이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-268">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>
* <span data-ttu-id="68791-269">VM 및 VM 확장 집합에 대한 사용자 할당 ID가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="68791-269">User assigned identity support for VM and VM scale set</span></span>
    - <span data-ttu-id="68791-270">`New-AzureRmVMConfig`, `New-AzureRmVmssConfig`, `Update-AzureRmVM`, `Update-AzureRmVmss`에 `-IdentityType` 및 `-IdentityId` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-270">`-IdentityType` and `-IdentityId` parameters are added to `New-AzureRmVMConfig`, `New-AzureRmVmssConfig`, `Update-AzureRmVM` and `Update-AzureRmVmss`</span></span>
* <span data-ttu-id="68791-271">`-EnableIPForwarding` 매개 변수가 `Add-AzureRmVmssNetworkInterfaceConfig`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-271">Added `-EnableIPForwarding` parameter to `Add-AzureRmVmssNetworkInterfaceConfig`</span></span>
* <span data-ttu-id="68791-272">`-Priority` 매개 변수가 `New-AzureRmVmssConfig`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-272">Added `-Priority` parameter to `New-AzureRmVmssConfig`</span></span>

### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="68791-273">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="68791-273">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="68791-274">`Connect-AzureRmAccount`를 사용하도록 `Login-AzureRmAccount`의 사용법이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-274">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

### <a name="azurermdatalakestore"></a><span data-ttu-id="68791-275">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="68791-275">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="68791-276">`Connect-AzureRmAccount`를 사용하도록 `Login-AzureRmAccount`의 사용법이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-276">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>
* <span data-ttu-id="68791-277">`Login-AzureRmAccount`를 사용하여 로그인하지 않고 이 cmdlet을 실행하는 경우 오류 메시지 `Test-AzureRmDataLakeStoreAccount`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-277">Corrected the error message of `Test-AzureRmDataLakeStoreAccount` when running this cmdlet without having logged in with `Login-AzureRmAccount`</span></span>

### <a name="azurermeventgrid"></a><span data-ttu-id="68791-278">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="68791-278">AzureRM.EventGrid</span></span>
* <span data-ttu-id="68791-279">2018-01-01 API 버전을 사용하도록 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-279">Updated to use the 2018-01-01 API version.</span></span>

### <a name="azurermeventhub"></a><span data-ttu-id="68791-280">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="68791-280">AzureRM.EventHub</span></span>

* <span data-ttu-id="68791-281">지역 재해 복구 작업에 대한 아래의 새 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-281">Added below new commands for Geo Disaster Recovery operations.</span></span>
  - <span data-ttu-id="68791-282">새 별칭(재해 복구 구성)을 만드는 중입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-282">Creating a new Alias (Disaster Recovery configuration):</span></span>
    - `New-AzureRmEventHubGeoDRConfiguration`
  - <span data-ttu-id="68791-283">새 별칭(재해 복구 구성)을 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-283">Retrieve Alias (Disaster Recovery configuration) :</span></span>
    - `Get-AzureRmEventHubGeoDRConfiguration`
  - <span data-ttu-id="68791-284">재해 복구를 사용하지 않고 기본 네임스페이스에서 보조 네임스페이스로의 변경 사항 복제 중지</span><span class="sxs-lookup"><span data-stu-id="68791-284">Disabling the Disaster Recovery and stops replicating changes from primary to secondary namespaces</span></span>
    - `Set-AzureRmEventHubGeoDRConfigurationBreakPair`
  - <span data-ttu-id="68791-285">재해 복구 장애 조치(failover)를 호출하고 별칭이 보조 네임스페이스를 가리키도록 다시 구성</span><span class="sxs-lookup"><span data-stu-id="68791-285">Invoking Disaster Recovery failover and reconfigure the alias to point to the secondary namespace</span></span>
    - `Set-AzureRmEventHubGeoDRConfigurationFailOver`
  - <span data-ttu-id="68791-286">별칭 삭제(재해 복구 구성)</span><span class="sxs-lookup"><span data-stu-id="68791-286">Deleting an Alias(Disaster Recovery configuration)</span></span>
    - `Remove-AzureRmEventHubGeoDRConfiguration`
* <span data-ttu-id="68791-287">네임스페이스 이름 및 GeoDr 구성 이름 - 별칭 가용성을 검사하는 아래의 새 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-287">Added below new commands for checking the Namespace Name and GeoDr Configuration Name - Alias availability.</span></span>
  - <span data-ttu-id="68791-288">네임스페이스 이름의 가용성 이름 또는 별칭(재해 복구 구성) 이름을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-288">Check the Availability of Namespace name or Alias(Disaster Recovery configuration) name:</span></span>
    - `Test-AzureRmEventHubName`

### <a name="azurerminsights"></a><span data-ttu-id="68791-289">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="68791-289">AzureRM.Insights</span></span>
* <span data-ttu-id="68791-290">`Connect-AzureRmAccount`를 사용하도록 `Login-AzureRmAccount`의 사용법이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-290">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="68791-291">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="68791-291">AzureRM.KeyVault</span></span>
* <span data-ttu-id="68791-292">`Connect-AzureRmAccount`를 사용하도록 `Login-AzureRmAccount`의 사용법이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-292">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="68791-293">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="68791-293">AzureRM.Network</span></span>
* <span data-ttu-id="68791-294">'리소스를 덮어쓰시겠습니까?'라는 덮어쓰기 메시지가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-294">Fix overwrite message 'Are you sure you want to overwriteresource'</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="68791-295">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="68791-295">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="68791-296">`Invoke-AzureRmOperationalInsightsQuery`를 통해 V2 API 쿼리에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-296">Added support for V2 API querying via `Invoke-AzureRmOperationalInsightsQuery`.</span></span> <span data-ttu-id="68791-297">새로운 API에 대한 보다 자세한 내용은 [https://dev.loganalytics.io/](https://dev.loganalytics.io/)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="68791-297">See [https://dev.loganalytics.io/](https://dev.loganalytics.io/) for more info on the new API.</span></span>

### <a name="azurermresources"></a><span data-ttu-id="68791-298">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="68791-298">AzureRM.Resources</span></span>
* <span data-ttu-id="68791-299">`Get-AzureRmADServicePrincipal`: SPN 매개 변수 설정과 중복되는 기본 빈 매개 변수 설정에서 `-ServicePrincipalName`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-299">`Get-AzureRmADServicePrincipal`: Removed `-ServicePrincipalName` from the default Empty parameter set as it was redundant with the SPN parameter set</span></span>

### <a name="azurermservicebus"></a><span data-ttu-id="68791-300">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="68791-300">AzureRM.ServiceBus</span></span>

* <span data-ttu-id="68791-301">`Remove-AzureRmServiceBusRule` 및 `Get-AzureRmServiceBusKey`에 대한 기능 수정이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-301">Added functionality fix for `Remove-AzureRmServiceBusRule` and `Get-AzureRmServiceBusKey`</span></span>
* <span data-ttu-id="68791-302">지역 재해 복구 작업에 대한 아래의 새 commandlet이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-302">Added below new commandlets for Geo Disaster Recovery operations.</span></span>
  - <span data-ttu-id="68791-303">새 별칭(재해 복구 구성)을 만드는 중입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-303">Creating a new Alias (Disaster Recovery configuration):</span></span>
    - `New-AzureRmServiceBusDRConfigurations`
  - <span data-ttu-id="68791-304">새 별칭(재해 복구 구성)을 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-304">Retrieve Alias (Disaster Recovery configuration) :</span></span>
    - `Get-AzureRmServiceBusDRConfigurations`
  - <span data-ttu-id="68791-305">재해 복구를 사용하지 않고 기본 네임스페이스에서 보조 네임스페이스로의 변경 사항 복제 중지</span><span class="sxs-lookup"><span data-stu-id="68791-305">Disabling the Disaster Recovery and stops replicating changes from primary to secondary namespaces</span></span>
    - `Set-AzureRmServiceBusDRConfigurationsBreakPairing`
  - <span data-ttu-id="68791-306">재해 복구 장애 조치(failover)를 호출하고 별칭이 보조 네임스페이스를 가리키도록 다시 구성</span><span class="sxs-lookup"><span data-stu-id="68791-306">Invoking Disaster Recovery failover and reconfigure the alias to point to the secondary namespace</span></span>
    - `Set-AzureRmServiceBusDRConfigurationsFailOver`
  - <span data-ttu-id="68791-307">별칭 삭제(재해 복구 구성)</span><span class="sxs-lookup"><span data-stu-id="68791-307">Deleting an Alias(Disaster Recovery configuration)</span></span>
    - `Remove-AzureRmServiceBusDRConfigurations`
* <span data-ttu-id="68791-308">지역 재해 복구 - 별칭 이름 확인 가용성 작업을 지원하도록 `Test-AzureRmServiceBusName` commandlet이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-308">Updated `Test-AzureRmServiceBusName` commandlets to support Geo Disaster Recovery - Alias name check availability operations.</span></span>
  - <span data-ttu-id="68791-309">네임스페이스 이름의 가용성 이름 또는 별칭(재해 복구 구성) 이름을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-309">Check the Availability of Namespace name or Alias(Disaster Recovery configuration) name:</span></span>
    - `Test-AzureRmServiceBusName`

### <a name="azurermusageaggregates"></a><span data-ttu-id="68791-310">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="68791-310">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="68791-311">`Connect-AzureRmAccount`를 사용하도록 `Login-AzureRmAccount`의 사용법이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-311">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

## <a name="520---january-2018"></a><span data-ttu-id="68791-312">5.2.0 - 2018년 1월</span><span class="sxs-lookup"><span data-stu-id="68791-312">5.2.0 - January 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="68791-313">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="68791-313">AzureRM.Profile</span></span>
* <span data-ttu-id="68791-314">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-314">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-315">Add-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="68791-315">Add-AzureRmAccount</span></span>
  * <span data-ttu-id="68791-316">현재 VM/서비스에 있는 관리 서비스 ID의 자격 증명을 사용하여 인증하기 위해 -MSI 로그인을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-316">Added -MSI login for authenticationg using the credentials of the Managed Service Identity of the current VM / Service</span></span>
  * <span data-ttu-id="68791-317">사용자 제공 액세스 토큰을 사용하여 로그인할 때 KeyVault 인증을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-317">Fixed KeyVault Authentication when logging in with user-provided access tokens</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="68791-318">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="68791-318">Azure.Storage</span></span>
* <span data-ttu-id="68791-319">Storage 서비스 속성을 가져오고 설정하는 cmdlet을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-319">Add cmdlets to get and set Storage service properties</span></span>
    - <span data-ttu-id="68791-320">Get-AzureStorageServiceProperty</span><span class="sxs-lookup"><span data-stu-id="68791-320">Get-AzureStorageServiceProperty</span></span>
    - <span data-ttu-id="68791-321">Update-AzureStorageServiceProperty</span><span class="sxs-lookup"><span data-stu-id="68791-321">Update-AzureStorageServiceProperty</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="68791-322">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="68791-322">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="68791-323">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-323">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="68791-324">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="68791-324">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="68791-325">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-325">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-326">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-326">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-327">New-AzureRmApiManagementProperty, Set-AzureRmApiManagementProperty 및 New-AzureRmApiManagement에 -Tag를 사용하는 -Tags를 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-327">Obsoleted -Tags in favor of -Tag for New-AzureRmApiManagementProperty, Set-AzureRmApiManagementProperty, and New-AzureRmApiManagement</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="68791-328">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="68791-328">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="68791-329">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-329">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-330">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-330">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="68791-331">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="68791-331">AzureRM.Automation</span></span>
* <span data-ttu-id="68791-332">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-332">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-333">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-333">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-334">Set-AzureRmAutomationRunbook에 -Tag를 사용하는 -Tags를 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-334">Obsoleted -Tags in favor of -Tag for Set-AzureRmAutomationRunbook</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="68791-335">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="68791-335">AzureRM.Backup</span></span>
* <span data-ttu-id="68791-336">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-336">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-337">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-337">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="68791-338">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="68791-338">AzureRM.Batch</span></span>
* <span data-ttu-id="68791-339">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-339">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-340">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-340">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="68791-341">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="68791-341">AzureRM.Cdn</span></span>
* <span data-ttu-id="68791-342">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-342">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-343">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-343">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-344">New-AzureRmCdnEndpoint 및 New-AzureRmCdnProfile에 -Tag를 사용하는 -Tags를 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-344">Obsoleted -Tags in favor of -Tag for New-AzureRmCdnEndpoint and New-AzureRmCdnProfile</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="68791-345">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="68791-345">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="68791-346">Cognitive Services Management SDK 버전 3.0.0과 통합합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-346">Integrate with Cognitive Services Management SDK version 3.0.0.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="68791-347">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="68791-347">AzureRM.Compute</span></span>
* <span data-ttu-id="68791-348">New-AzureRmVmss에 간소화된 매개 변수 집합이 추가되었습니다. 따라서 스마트 기본값을 사용하여 Virtual Machine Scale Set과 필요한 모든 리소스가 만들어집니다.</span><span class="sxs-lookup"><span data-stu-id="68791-348">Added simplified parameter set to New-AzureRmVmss, which creates a Virtual Machine Scale Set and all required resources using smart defaults</span></span>
* <span data-ttu-id="68791-349">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-349">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-350">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-350">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-351">New-AzureRmVm 및 Update-AzureRmVm에 -Tag를 사용하는 -Tags를 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-351">Obsoleted -Tags in favor of -Tag for New-AzureRmVm and Update-AzureRmVm</span></span>
* <span data-ttu-id="68791-352">영역이 제한에 포함될 때 Get-AzureRmComputeResourceSku cmdlet을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-352">Fixed Get-AzureRmComputeResourceSku cmdlet when Zone is included in restriction.</span></span>
* <span data-ttu-id="68791-353">Azure Monitor 동기화 지원을 위해 진단 에이전트 구성 스키마를 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-353">Updated Diagnostics Agent configuration schema for Azure Monitor sink support.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="68791-354">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="68791-354">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="68791-355">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-355">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-356">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-356">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="68791-357">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="68791-357">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="68791-358">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-358">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-359">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-359">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="68791-360">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="68791-360">AzureRM.DataFactories</span></span>
* <span data-ttu-id="68791-361">모든 데이터 저장소 연결 서비스에 대해 Azure Key Vault 지원을 활성화했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-361">Enabled Azure Key Vault support for all data store linked services</span></span>
* <span data-ttu-id="68791-362">Azure SSIS 통합 런타임에 라이선스 형식 속성을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-362">Added license type property for Azure SSIS integration runtime</span></span>
* <span data-ttu-id="68791-363">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-363">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-364">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-364">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-365">New-AzureRmDataFactory에 -Tag를 사용하는 -Tags를 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-365">Obsoleted -Tags in favor of -Tag for New-AzureRmDataFactory</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="68791-366">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="68791-366">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="68791-367">모든 데이터 저장소 연결 서비스에 대해 Azure Key Vault 지원을 활성화했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-367">Enabled Azure Key Vault support for all data store linked services</span></span>
* <span data-ttu-id="68791-368">Azure SSIS 통합 런타임에 라이선스 형식 속성을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-368">Added license type property for Azure SSIS integration runtime</span></span>
* <span data-ttu-id="68791-369">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-369">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-370">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-370">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-371">AHUB 기능을 사용하도록 "Set-AzureRmDataFactoryV2IntegrationRuntime" cmd에 "LicenseType" 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-371">Add parameter "LicenseType" for "Set-AzureRmDataFactoryV2IntegrationRuntime" cmd to enable AHUB functionality</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="68791-372">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="68791-372">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="68791-373">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-373">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-374">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-374">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-375">New-AzureRmDataLakeAnalyticsAccount 및 Set-AzureRmDataLakeAnalyticsAccount에 -Tag를 사용하는 -Tags를 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-375">Obsoleted -Tags in favor of -Tag for New-AzureRmDataLakeAnalyticsAccount and Set-AzureRmDataLakeAnalyticsAccount</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="68791-376">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="68791-376">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="68791-377">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-377">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-378">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-378">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-379">New-AzureRmDataLakeStoreAccount 및 Set-AzureRmDataLakeStoreAccount에 -Tag를 사용하는 -Tags를 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-379">Obsoleted -Tags in favor of -Tag for New-AzureRmDataLakeStoreAccount and Set-AzureRmDataLakeStoreAccount</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="68791-380">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="68791-380">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="68791-381">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-381">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="68791-382">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="68791-382">AzureRM.Dns</span></span>
* <span data-ttu-id="68791-383">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-383">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="68791-384">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="68791-384">AzureRM.EventGrid</span></span>
* <span data-ttu-id="68791-385">다음과 같은 새 cmdlet을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-385">Added the following new cmdlet:</span></span>
  - <span data-ttu-id="68791-386">Update-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="68791-386">Update-AzureRmEventGridSubscription</span></span>
    - <span data-ttu-id="68791-387">Event Grid 이벤트 구독의 속성을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-387">Update the properties of an Event Grid event subscription.</span></span>
* <span data-ttu-id="68791-388">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-388">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-389">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-389">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="68791-390">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="68791-390">AzureRM.EventHub</span></span>
* <span data-ttu-id="68791-391">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-391">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-392">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-392">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="68791-393">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="68791-393">AzureRM.HDInsight</span></span>
* <span data-ttu-id="68791-394">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-394">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-395">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-395">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="68791-396">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="68791-396">AzureRM.Insights</span></span>
* <span data-ttu-id="68791-397">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-397">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-398">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-398">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="68791-399">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="68791-399">AzureRM.IotHub</span></span>
* <span data-ttu-id="68791-400">IoTHub cmdlet에 인증서 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-400">Add Certificate support for IoTHub cmdlets</span></span>
* <span data-ttu-id="68791-401">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-401">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-402">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-402">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="68791-403">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="68791-403">AzureRM.KeyVault</span></span>
* <span data-ttu-id="68791-404">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-404">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-405">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-405">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-406">장기 실행 KeyVault cmdlet에 대한 -AsJob 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-406">Added -AsJob support for long-running KeyVault cmdlets.</span></span> <span data-ttu-id="68791-407">선택된 cmdlet을 백그라운드에서 실행하고 작업을 반환하여 진행률을 추적 및 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-407">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
  * <span data-ttu-id="68791-408">영향을 받는 cmdlet은 Remove-AzureRmKeyVault입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-408">Affected cmdlet is: Remove-AzureRmKeyVault</span></span>
* <span data-ttu-id="68791-409">AAD 필터가 UPN 설정이 아닌 SPN을 제공된 UPN으로 설정하는 Set-AzureRmKeyVaultAccessPolicy에서 버그를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-409">Fixed bug in Set-AzureRmKeyVaultAccessPolicy where the AAD filter was setting SPN to the provided UPN, rather than setting the UPN</span></span>
  - <span data-ttu-id="68791-410">보다 자세한 내용은 다음 문제를 참조하세요. https://github.com/Azure/azure-powershell/issues/5201</span><span class="sxs-lookup"><span data-stu-id="68791-410">See the following issue for more information: https://github.com/Azure/azure-powershell/issues/5201</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="68791-411">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="68791-411">AzureRM.LogicApp</span></span>
* <span data-ttu-id="68791-412">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-412">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-413">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-413">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="68791-414">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="68791-414">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="68791-415">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-415">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-416">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-416">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-417">Update-AzureRmMlCommitmentPlan에 -Tag를 사용하는 -Tags를 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-417">Obsoleted -Tags in favor of -Tag for Update-AzureRmMlCommitmentPlan</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="68791-418">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="68791-418">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="68791-419">Remove-AzureRmMlOpCluster cmdlet에 IncludeAllResources 매개 변수를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-419">Add IncludeAllResources parameter to Remove-AzureRmMlOpCluster cmdlet</span></span>
  - <span data-ttu-id="68791-420">이 스위치 매개 변수를 사용하면 원래 클러스터를 사용하여 만든 모든 리소스를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-420">Using this switch parameter will remove all resources that were created with the cluster originally</span></span>
* <span data-ttu-id="68791-421">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-421">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-422">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-422">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="68791-423">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="68791-423">AzureRM.Media</span></span>
* <span data-ttu-id="68791-424">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-424">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-425">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-425">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-426">Set-AzureRmMediaService 및 New-AzureRmMediaService에 -Tag를 사용하는 -Tags를 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-426">Obsoleted -Tags in favor of -Tag for Set-AzureRmMediaService and New-AzureRmMediaService</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="68791-427">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="68791-427">AzureRM.Network</span></span>
* <span data-ttu-id="68791-428">장기 실행 Network cmdlet에 대한 -AsJob 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-428">Added -AsJob support for long-running Network cmdlets.</span></span> <span data-ttu-id="68791-429">선택된 cmdlet을 백그라운드에서 실행하고 작업을 반환하여 진행률을 추적 및 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-429">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
* <span data-ttu-id="68791-430">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-430">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-431">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-431">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="68791-432">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="68791-432">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="68791-433">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-433">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-434">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-434">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-435">New-AzureRmNotificationHubsNamespace 및 Set-AzureRmNotificationHubsNamespace에 -Tag를 사용하는 -Tags 사용하지를 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-435">Obsoleted -Tags in favor of -Tag for New-AzureRmNotificationHubsNamespace and Set-AzureRmNotificationHubsNamespace</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="68791-436">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="68791-436">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="68791-437">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-437">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-438">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-438">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-439">New-AzureRmOperationalInsightsSavedSearch, Set-AzureRmOperationalInsightsSavedSearch, New-AzureRmOperationalInsightsWorkspace 및 Set-AzureRmOperationalInsightsWorkspace에 -Tag를 사용하는 -Tags 사용하지를 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-439">Obsoleted -Tags in favor of -Tag for New-AzureRmOperationalInsightsSavedSearch, Set-AzureRmOperationalInsightsSavedSearch, New-AzureRmOperationalInsightsWorkspace, and Set-AzureRmOperationalInsightsWorkspace</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="68791-440">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="68791-440">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="68791-441">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-441">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-442">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-442">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="68791-443">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="68791-443">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="68791-444">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-444">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-445">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-445">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="68791-446">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="68791-446">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="68791-447">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-447">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-448">Restore-AzureRmRecoveryServicesBackupItem cmdlet에 -UseOriginalStorageAccount 옵션을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-448">Added -UseOriginalStorageAccount option to the Restore-AzureRmRecoveryServicesBackupItem cmdlet.</span></span>
  - <span data-ttu-id="68791-449">이 플래그를 사용하면 사용자가 원래 VM과 최대한 가까운 복원된 VM의 구성이 유지하도록 원래 저장소 계정에 디스크를 복원하게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="68791-449">Enabling this flag results in restoring disks to their original storage accounts which allows users to maintain the configuration of restored VM as close to the original VMs as possible.</span></span>
  - <span data-ttu-id="68791-450">복원 작업의 성능을 향상시키는 데에도 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="68791-450">It also helps in improving the performance of the restore operation.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="68791-451">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="68791-451">AzureRM.RedisCache</span></span>
* <span data-ttu-id="68791-452">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-452">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-453">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-453">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-454">방화벽 규칙에 대한 새로운 3개의 cmdlet을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-454">Added  3 new cmdlets for firewall rules</span></span>
* <span data-ttu-id="68791-455">지리적 복제에 대한 새로운 3개의 cmdlet을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-455">Added  3 new cmdlets for geo replication</span></span>
* <span data-ttu-id="68791-456">영역 및 태그에 대한 지원을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-456">Added support for zones and tags</span></span>
* <span data-ttu-id="68791-457">가능하면 ResourceGroup을 선택 사항으로 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="68791-457">Make ResourceGroup as optional whenever possible.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="68791-458">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="68791-458">AzureRM.Relay</span></span>
* <span data-ttu-id="68791-459">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-459">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-460">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-460">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="68791-461">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="68791-461">AzureRM.Resources</span></span>
* <span data-ttu-id="68791-462">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-462">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-463">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-463">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-464">장기 실행 Resources cmdlet에 대한 -AsJob 지원을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-464">Added -AsJob support for long-running Resources cmdlets.</span></span> <span data-ttu-id="68791-465">선택된 cmdlet을 백그라운드에서 실행하고 작업을 반환하여 진행률을 추적 및 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-465">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
* <span data-ttu-id="68791-466">명명 규칙을 준수하도록 Get-AzureRmProviderOperation에서 Get-AzureRmResourceProviderAction에 별칭을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-466">Added alias from Get-AzureRmProviderOperation to Get-AzureRmResourceProviderAction to conform with naming conventions</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="68791-467">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="68791-467">AzureRM.Scheduler</span></span>
* <span data-ttu-id="68791-468">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-468">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-469">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-469">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermservermanagement"></a><span data-ttu-id="68791-470">AzureRM.ServerManagement</span><span class="sxs-lookup"><span data-stu-id="68791-470">AzureRM.ServerManagement</span></span>
* <span data-ttu-id="68791-471">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-471">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-472">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-472">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-473">New-AzureRmServerManagementNode 및 New-AzureRmServerManagementGateway에 -Tag를 사용하는 -Tags를 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-473">Obsoleted -Tags in favor of -Tag for New-AzureRmServerManagementNode and New-AzureRmServerManagementGateway</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="68791-474">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="68791-474">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="68791-475">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-475">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-476">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-476">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="68791-477">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="68791-477">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="68791-478">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-478">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-479">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-479">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermsiterecovery"></a><span data-ttu-id="68791-480">AzureRM.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="68791-480">AzureRM.SiteRecovery</span></span>
* <span data-ttu-id="68791-481">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-481">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-482">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-482">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="68791-483">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="68791-483">AzureRM.Sql</span></span>
* <span data-ttu-id="68791-484">감사 명령 매개 변수 설명을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-484">Update the Auditing commands parameters description</span></span>
* <span data-ttu-id="68791-485">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-485">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-486">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-486">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-487">장기 실행 cmdlet에 -AsJob 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="68791-487">Added -AsJob parameter to long running cmdlets</span></span>
* <span data-ttu-id="68791-488">Get-AzureRmSqlServiceObjective에서 -DatabaseName 매개 변수를 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-488">Obsoleted -DatabaseName parameter from Get-AzureRmSqlServiceObjective</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="68791-489">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="68791-489">AzureRM.Storage</span></span>
* <span data-ttu-id="68791-490">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-490">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-491">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-491">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-492">-EnableEncryptionService None 매개 변수를 사용하여 New-AzureRMStorageAccount 실행 cmdlet의 null 참조 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-492">Fix a null reference issue of run cmdlet New-AzureRMStorageAccount with parameter -EnableEncryptionService None</span></span>
* <span data-ttu-id="68791-493">장기 실행 Storage cmdlet에 대한 -AsJob 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-493">Added -AsJob support for long-running Storage cmdlets.</span></span> <span data-ttu-id="68791-494">선택된 cmdlet을 백그라운드에서 실행하고 작업을 반환하여 진행률을 추적 및 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-494">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
    - <span data-ttu-id="68791-495">영향을 받는 cmdlet은 저장소 계정 및 네트워크 규칙에 대한 New-, Remove-, Add- 및 Update-입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-495">Affected cmdlets are New-, Remove-, Add-, and Update- for Storage Account and Storage Account Network Rule.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="68791-496">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="68791-496">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="68791-497">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-497">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-498">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-498">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="68791-499">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="68791-499">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="68791-500">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-500">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-501">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-501">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="68791-502">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="68791-502">AzureRM.Websites</span></span>
* <span data-ttu-id="68791-503">유효한 위치를 통해 탭 완성 기능을 허용하는 -Location 매개 변수에 Location Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-503">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="68791-504">현재 구독에서 리소스 그룹을 통해 탭 완성 기능을 허용하는 -ResourceGroup 매개 변수에 ResourceGroup Completer를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-504">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="68791-505">장기 실행 Websites cmdlet에 대한 -AsJob 지원을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-505">Added -AsJob support for long-running Websites cmdlets.</span></span> <span data-ttu-id="68791-506">선택된 cmdlet을 백그라운드에서 실행하고 작업을 반환하여 진행률을 추적 및 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-506">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
     - <span data-ttu-id="68791-507">영향을 받는 cmdlet은 WebApps, AppServicePlan 및 Slots에 대한 New-, Remove-, Add- 및 Set-입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-507">Affected cmdlets are New-, Remove-, Add-, and Set- for WebApps, AppServicePlan and Slots</span></span>

## <a name="2017128-version-511"></a><span data-ttu-id="68791-508">2017.12.8 버전 5.1.1</span><span class="sxs-lookup"><span data-stu-id="68791-508">2017.12.8 Version 5.1.1</span></span>
* <span data-ttu-id="68791-509">AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="68791-509">AnalysisServices</span></span>
  - <span data-ttu-id="68791-510">모든 클라우드가 지원되도록 위치 확인 집합을 동적 조회로 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-510">Change validate set of location to dynamic lookup so that all clouds are supported.</span></span>
* <span data-ttu-id="68791-511">Automation</span><span class="sxs-lookup"><span data-stu-id="68791-511">Automation</span></span>
  - <span data-ttu-id="68791-512">Import-AzureRMAutomationRunbook으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="68791-512">Update to Import-AzureRMAutomationRunbook</span></span>
    - <span data-ttu-id="68791-513">이제 Python2 Runbook에 대한 지원이 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="68791-513">Support is now being provided for Python2 runbooks</span></span>
* <span data-ttu-id="68791-514">Batch</span><span class="sxs-lookup"><span data-stu-id="68791-514">Batch</span></span>
  - <span data-ttu-id="68791-515">리소스 그룹이 없는 계정 작업으로 리소스 그룹을 자동 검색하지 못하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-515">Fixed a bug where account operations without a resource group failed to auto-detect the resource group</span></span>
* <span data-ttu-id="68791-516">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="68791-516">Compute</span></span>
  - <span data-ttu-id="68791-517">Get-AzureRmComputeResourceSku가 영역 정보를 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="68791-517">Get-AzureRmComputeResourceSku shows zone information.</span></span>
  - <span data-ttu-id="68791-518">문제 https://github.com/Azure/azure-powershell/issues/5038의 수정을 위해 Disable-AzureRmVmssDiskEncryption 업데이트</span><span class="sxs-lookup"><span data-stu-id="68791-518">Update Disable-AzureRmVmssDiskEncryption to fix issue https://github.com/Azure/azure-powershell/issues/5038</span></span>
  - <span data-ttu-id="68791-519">장기 실행 Compute cmdlet에 대한 -AsJob 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-519">Added -AsJob support for long-running Compute cmdlets.</span></span> <span data-ttu-id="68791-520">선택된 cmdlet을 백그라운드에서 실행하고 작업을 반환하여 진행률을 추적 및 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-520">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
    - <span data-ttu-id="68791-521">영향을 받는 cmdlet은 Virtual Machines 및 Virtual Machine Scale Sets에 대한 New-, Update-, Set-, Remove-, Start-, Restart-, Stop- cmdlet입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-521">Affected cmdlets include: New-, Update-, Set-, Remove-, Start-, Restart-, Stop- cmdlets for Virtual Machines and Virtual Machine Scale Sets</span></span>
    - <span data-ttu-id="68791-522">단순한 매개 변수 집합이 New-AzureRmVM에 추가되었습니다. 따라서 스마트 기본값을 사용하여 Virtual Machine과 필요한 모든 리소스가 만들어집니다.</span><span class="sxs-lookup"><span data-stu-id="68791-522">Added simplified parameter set to New-AzureRmVM, which creates a Virtual Machine and all required resources using smart defaults</span></span>
* <span data-ttu-id="68791-523">ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="68791-523">ContainerInstance</span></span>
  - <span data-ttu-id="68791-524">Azure Container Instance SDK 2017-10-01 적용</span><span class="sxs-lookup"><span data-stu-id="68791-524">Apply Azure Container Instance SDK 2017-10-01</span></span>
    - <span data-ttu-id="68791-525">컨테이너 실행 완료 지원</span><span class="sxs-lookup"><span data-stu-id="68791-525">Support container run-to-completion</span></span>
    - <span data-ttu-id="68791-526">Azure 파일 볼륨 탑재 지원</span><span class="sxs-lookup"><span data-stu-id="68791-526">Support Azure File volume mount</span></span>
    - <span data-ttu-id="68791-527">공용 IP에 대한 여러 포트 열기 지원</span><span class="sxs-lookup"><span data-stu-id="68791-527">Support opening multiple ports for public IP</span></span>
* <span data-ttu-id="68791-528">ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="68791-528">ContainerRegistry</span></span>
  - <span data-ttu-id="68791-529">지역에서 복제 및 웹후크에 대한 새로운 cmdlet</span><span class="sxs-lookup"><span data-stu-id="68791-529">New cmdlets for geo-replication and webhooks</span></span>
    - <span data-ttu-id="68791-530">Get/New/Remove-AzureRmContainerRegistryReplication</span><span class="sxs-lookup"><span data-stu-id="68791-530">Get/New/Remove-AzureRmContainerRegistryReplication</span></span>
    - <span data-ttu-id="68791-531">Get/New/Remove/Test/Update-AzureRmContainerRegistryWebhook</span><span class="sxs-lookup"><span data-stu-id="68791-531">Get/New/Remove/Test/Update-AzureRmContainerRegistryWebhook</span></span>
* <span data-ttu-id="68791-532">DataFactories</span><span class="sxs-lookup"><span data-stu-id="68791-532">DataFactories</span></span>
    - <span data-ttu-id="68791-533">이제 자격 증명 암호화 기능은 "원격 액세스"가 사용된 경우(네트워크 사용) 및 "원격 액세스"가 사용되지 않는 경우(로컬 컴퓨터) 모두에서 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-533">Credential encryption functionality now works with both "Remote Access" enabled (Over Network) and "Remote Access" disabled (Local Machine).</span></span>
* <span data-ttu-id="68791-534">DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="68791-534">DataFactoryV2</span></span>
  - <span data-ttu-id="68791-535">두 개의 새로운 cmdlet 추가: Update-AzureRmDataFactoryV2 및 Stop-AzureRmDataFactoryV2PipelineRun</span><span class="sxs-lookup"><span data-stu-id="68791-535">Added two new cmdlets: Update-AzureRmDataFactoryV2 and Stop-AzureRmDataFactoryV2PipelineRun</span></span>
* <span data-ttu-id="68791-536">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="68791-536">DataLakeAnalytics</span></span>
  - <span data-ttu-id="68791-537">Submit-AzureRmDataLakeAnalyticsJob에 ScriptParameter라는 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-537">Added a parameter called ScriptParameter to Submit-AzureRmDataLakeAnalyticsJob</span></span>
    - <span data-ttu-id="68791-538">ScriptParameter에 대한 자세한 정보는 Submit-AzureRmDataLakeAnalyticsJob에서 Get-Help를 사용하여 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-538">Detailed information about ScriptParameter can be found using Get-Help on Submit-AzureRmDataLakeAnalyticsJob</span></span>
  - <span data-ttu-id="68791-539">New-AzureRmDataLakeAnalyticsAccount의 경우 MaxDegreeOfParallelism 매개 변수가 MaxAnalyticsUnits로 변경됨</span><span class="sxs-lookup"><span data-stu-id="68791-539">For New-AzureRmDataLakeAnalyticsAccount, changed the parameter MaxDegreeOfParallelism to MaxAnalyticsUnits</span></span>
    - <span data-ttu-id="68791-540">MaxAnalyticsUnits: MaxDegreeOfParallelism 매개 변수에 대한 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-540">Added an alias for the parameter MaxAnalyticsUnits: MaxDegreeOfParallelism</span></span>
  - <span data-ttu-id="68791-541">New-AzureRmDataLakeAnalyticsComputePolicy의 경우 MaxDegreeOfParallelismPerJob 매개 변수가 MaxAnalyticsUnitsPerJob으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="68791-541">For New-AzureRmDataLakeAnalyticsComputePolicy, changed the parameter MaxDegreeOfParallelismPerJob to MaxAnalyticsUnitsPerJob</span></span>
    - <span data-ttu-id="68791-542">MaxAnalyticsUnitsPerJob: MaxDegreeOfParallelismPerJob 매개 변수에 대한 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-542">Added an alias for the parameter MaxAnalyticsUnitsPerJob: MaxDegreeOfParallelismPerJob</span></span>
  - <span data-ttu-id="68791-543">Set-AzureRmDataLakeAnalyticsAccount의 경우 MaxDegreeOfParallelism 매개 변수가 MaxAnalyticsUnits로 변경됨</span><span class="sxs-lookup"><span data-stu-id="68791-543">For Set-AzureRmDataLakeAnalyticsAccount, changed the parameter MaxDegreeOfParallelism to MaxAnalyticsUnits</span></span>
    - <span data-ttu-id="68791-544">MaxAnalyticsUnits: MaxDegreeOfParallelism 매개 변수에 대한 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-544">Added an alias for the parameter MaxAnalyticsUnits: MaxDegreeOfParallelism</span></span>
  - <span data-ttu-id="68791-545">Submit-AzureRmDataLakeAnalyticsJob의 경우 DegreeOfParallelism 매개 변수가 AnalyticsUnits로 변경됨</span><span class="sxs-lookup"><span data-stu-id="68791-545">For Submit-AzureRmDataLakeAnalyticsJob, changed the parameter DegreeOfParallelism to AnalyticsUnits</span></span>
    - <span data-ttu-id="68791-546">AnalyticsUnits: DegreeOfParallelism 매개 변수에 대한 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-546">Added an alias for the parameter AnalyticsUnits: DegreeOfParallelism</span></span>
  - <span data-ttu-id="68791-547">Update-AzureRmDataLakeAnalyticsComputePolicy의 경우 MaxDegreeOfParallelismPerJob 매개 변수가 MaxAnalyticsUnitsPerJob으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="68791-547">For Update-AzureRmDataLakeAnalyticsComputePolicy, changed the parameter MaxDegreeOfParallelismPerJob to MaxAnalyticsUnitsPerJob</span></span>
    - <span data-ttu-id="68791-548">MaxAnalyticsUnitsPerJob: MaxDegreeOfParallelismPerJob 매개 변수에 대한 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-548">Added an alias for the parameter MaxAnalyticsUnitsPerJob: MaxDegreeOfParallelismPerJob</span></span>
* <span data-ttu-id="68791-549">MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="68791-549">MachineLearningCompute</span></span>
  - <span data-ttu-id="68791-550">Set-AzureRmMlOpCluster 추가</span><span class="sxs-lookup"><span data-stu-id="68791-550">Add Set-AzureRmMlOpCluster</span></span>
    - <span data-ttu-id="68791-551">클러스터의 에이전트 개수 또는 SSL 구성 업데이트</span><span class="sxs-lookup"><span data-stu-id="68791-551">Update a cluster's agent count or SSL configuration</span></span>
  - <span data-ttu-id="68791-552">오케스트레이터 속성은 선택 사항입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-552">Orchestrator properties are optional</span></span>
    - <span data-ttu-id="68791-553">서비스에서 서비스 주체를 생성하므로(제공되지 않은 경우) 오케스트레이터 속성은 선택 사항입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-553">The service will create a service principal if not provided, so the orchestrator properties are now optional</span></span>
* <span data-ttu-id="68791-554">PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="68791-554">PowerBIEmbedded</span></span>
  - <span data-ttu-id="68791-555">Power BI Embedded Capacity cmdlet에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="68791-555">Add support for Power BI Embedded Capacity cmdlets</span></span>
  - <span data-ttu-id="68791-556">새 Cmdlet Get-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded Capacity에 대한 정보를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="68791-556">New Cmdlet Get-AzureRmPowerBIEmbeddedCapacity - Gets the details of a PowerBI Embedded Capacity.</span></span>
  - <span data-ttu-id="68791-557">새 Cmdlet New-AzureRmPowerBIEmbeddedCapacity - 새 PowerBI Embedded Capacity를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="68791-557">New Cmdlet New-AzureRmPowerBIEmbeddedCapacity - Creates a new PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="68791-558">새 Cmdlet Remove-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded Capacity의 인스턴스를 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-558">New Cmdlet Remove-AzureRmPowerBIEmbeddedCapacity - Deletes an instance of PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="68791-559">새 Cmdlet Resume-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded Capacity의 인스턴스를 다시 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-559">New Cmdlet Resume-AzureRmPowerBIEmbeddedCapacity - Resumes an instance of PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="68791-560">새 Cmdlet Suspend-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded Capacity의 인스턴스를 일시 중단합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-560">New Cmdlet Suspend-AzureRmPowerBIEmbeddedCapacity - Suspends an instance of PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="68791-561">새 Cmdlet Test-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded Capacity 인스턴스의 존재 여부를 테스트합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-561">New Cmdlet Test-AzureRmPowerBIEmbeddedCapacity - Tests the existence of an instance of PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="68791-562">새 Cmdlet Update-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded Capacity의 인스턴스를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-562">New Cmdlet Update-AzureRmPowerBIEmbeddedCapacity - Modifies an instance of PowerBI Embedded Capacity</span></span>
* <span data-ttu-id="68791-563">프로필</span><span class="sxs-lookup"><span data-stu-id="68791-563">Profile</span></span>
  - <span data-ttu-id="68791-564">USGovernmentActiveDirectoryEndpoint가 https://login.microsoftonline.us/로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="68791-564">Updated USGovernmentActiveDirectoryEndpoint to https://login.microsoftonline.us/</span></span>
    - <span data-ttu-id="68791-565">Azure Government 끝점 매핑에 대한 보다 자세한 내용은 다음을 참조하세요. https://docs.microsoft.com/en-us/azure/azure-government/documentation-government-developer-guide#endpoint-mapping</span><span class="sxs-lookup"><span data-stu-id="68791-565">For more information about the Azure Government endpoint mappings, please see the following: https://docs.microsoft.com/en-us/azure/azure-government/documentation-government-developer-guide#endpoint-mapping</span></span>
    - <span data-ttu-id="68791-566">cmdlet에 대한 -AsJob 지원이 추가됨. 선택된 cmdlet을 사용하여 백그라운드에서 실행하고 작업을 반환하여 진행률 추적 및 제어</span><span class="sxs-lookup"><span data-stu-id="68791-566">Added -AsJob support for cmdlets, enabling selected cmdlets to execute in the background and return a job to track and control progress</span></span>
    - <span data-ttu-id="68791-567">-AsJob 매개 변수가 Get-AzureRmSubscription cmdlet에 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-567">Added -AsJob parameter to Get-AzureRmSubscription cmdlet</span></span>
* <span data-ttu-id="68791-568">RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="68791-568">RecoveryServices.Backup</span></span>
  - <span data-ttu-id="68791-569">버그 수정됨 - Get-AzureRmRecoveryServicesBackupItem은 컨테이너 이름 필터에 대해 대/소문자를 구분하지 않는 비교를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-569">Fixed bug - Get-AzureRmRecoveryServicesBackupItem should do case insensitive comparison for container name filter.</span></span>
  - <span data-ttu-id="68791-570">버그 수정됨 - AzureVmItem에는 백업 작업이 마지막으로 발생한 시간(LastBackupTime)을 보여 주는 속성이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-570">Fixed bug - AzureVmItem now has a property that shows the last time a backup operation has happened - LastBackupTime.</span></span>
* <span data-ttu-id="68791-571">리소스</span><span class="sxs-lookup"><span data-stu-id="68791-571">Resources</span></span>
  - <span data-ttu-id="68791-572">Get-AzureRMRoleAssignment가 사용자 지정 역할에 대한 roledefiniton 이름 없이 할당하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-572">Fixed issue where Get-AzureRMRoleAssignment would result in a assignments without roledefiniton name for custom roles</span></span>
    - <span data-ttu-id="68791-573">이제 사용자는 역할 유형에 관계없이 roledefinition이 있는 할당으로 Get-AzureRMRoleAssignment를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-573">Users can now use Get-AzureRMRoleAssignment with assignments having roledefinition names irrespective of the type of role</span></span>
  - <span data-ttu-id="68791-574">assignablescopes에 새 범위가 있을 때 RD를 throw하는 데 사용된 Set-AzureRMRoleRoleDefinition이 오류를 찾을 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-574">Fixed issue where Set-AzureRMRoleRoleDefinition used to throw RD not found error when there was a new scope in assignablescopes</span></span>
    - <span data-ttu-id="68791-575">이제 사용자는 범위의 위치와 관계없이 새 범위를 포함하여 할당 가능한 범위로 Set-AzureRMRoleRoleDefinition을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-575">Users can now use Set-AzureRMRoleRoleDefinition with assignable scopes including new scopes irrespective of the position of the scope</span></span>
  - <span data-ttu-id="68791-576">범위를 "/"로 끝내도록 허용</span><span class="sxs-lookup"><span data-stu-id="68791-576">Allow scopes to end with "/"</span></span>
    - <span data-ttu-id="68791-577">사용자는 이제 API 및 CLI와 일치하고 범위가 "/"로 끝나는 RoleDefinition 및 RoleAssignment commandlet을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-577">Users can now use RoleDefinition and RoleAssignment commandlets with scopes ending with "/" ,consistent with API and CLI</span></span>
  - <span data-ttu-id="68791-578">사용자가 위임 플래그를 사용하여 RoleAssignment를 만들도록 허용</span><span class="sxs-lookup"><span data-stu-id="68791-578">Allow users to create RoleAssignment using delegation flag</span></span>
    - <span data-ttu-id="68791-579">사용자는 위임 플래그를 추가하는 옵션과 함께 New-AzureRMRoleAssignment를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-579">Users can now use New-AzureRMRoleAssignment with an option of adding the delegation flag</span></span>
  - <span data-ttu-id="68791-580">RoleAssignment가 범위 매개 변수를 따르도록 수정</span><span class="sxs-lookup"><span data-stu-id="68791-580">Fix RoleAssignment get to respect the scope parameter</span></span>
  - <span data-ttu-id="68791-581">New-AzureRmRoleAssignment Commandlet에서 ServicePrincipalName에 대한 별칭 추가</span><span class="sxs-lookup"><span data-stu-id="68791-581">Add an alias for ServicePrincipalName in the New-AzureRmRoleAssignment Commandlet</span></span>
    - <span data-ttu-id="68791-582">사용자가 New-AzureRmRoleAssignment Commandlet을 사용할 때 ServicePrincipalName 대신 ApplicationId를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-582">Users can now use the ApplicationId instead of the ServicePrincipalName when using the New-AzureRmRoleAssignment commandlet</span></span>
* <span data-ttu-id="68791-583">SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="68791-583">SiteRecovery</span></span>
  - <span data-ttu-id="68791-584">향후 주요 변경 릴리스에 대한 준비에서, 이 모듈의 모든 cmdlet에 대한 사용 중단 경고를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-584">Add deprecation warnings for all cmdlets in this module in preparation for the next breaking change release.</span></span>
    - <span data-ttu-id="68791-585">AzureRM에서 cmdlet을 마이그레이션하는 방법에 대한 자세한 내용은 다음 주요 변경 사항 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="68791-585">Please see the upcoming breaking changes guide for more information on how to migrate your cmdlets from AzureRM.</span></span>
* <span data-ttu-id="68791-586">Sql</span><span class="sxs-lookup"><span data-stu-id="68791-586">Sql</span></span>
  - <span data-ttu-id="68791-587">Set-AzureRmSqlDatabase를 사용하여 데이터베이스 이름을 바꾸는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-587">Added ability to rename database using Set-AzureRmSqlDatabase</span></span>
  - <span data-ttu-id="68791-588">문제 https://github.com/Azure/azure-powershell/issues/4974 해결</span><span class="sxs-lookup"><span data-stu-id="68791-588">Fixed issue https://github.com/Azure/azure-powershell/issues/4974</span></span>
    - <span data-ttu-id="68791-589">감사 cmdlet에 대해 유효하지 않은 AUDIT_CHANGED_GROUP 값을 제공하면 더 이상 오류가 발생하지 않으며 향후 릴리스에서 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="68791-589">Providing invalid AUDIT_CHANGED_GROUP value for auditing cmdlets no longer throws an error and will be removed in an upcoming release.</span></span>
  - <span data-ttu-id="68791-590">문제 https://github.com/Azure/azure-powershell/issues/5046 해결</span><span class="sxs-lookup"><span data-stu-id="68791-590">Fixed issue https://github.com/Azure/azure-powershell/issues/5046</span></span>
    - <span data-ttu-id="68791-591">감사 cmdlet의 AuditAction 매개 변수가 더 이상 무시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-591">AuditAction parameter in auditing cmdlets is no longer being ignored</span></span>
  - <span data-ttu-id="68791-592">'보조' StorageKeyType이 제공된 경우 감사 cmdlet에서 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-592">Fixed an issue in Auditing cmdlets when 'Secondary' StorageKeyType is provided</span></span>
    - <span data-ttu-id="68791-593">Blob 감사를 설정할 때, StorageKeyType 매개 변수에 '보조' 값을 제공할 때 보조 키 대신, 주 저장소 계정 키가 사용되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-593">When setting blob auditing, the primary storage account key was used instead of the secondary key when providing 'Secondary' value for StorageKeyType parameter.</span></span>
  - <span data-ttu-id="68791-594">Set-AzureRmSqlServerTransparentDataEncryptionProtector에서 확인 메시지의 문구 변경</span><span class="sxs-lookup"><span data-stu-id="68791-594">Changing the wording for confirmation message from Set-AzureRmSqlServerTransparentDataEncryptionProtector</span></span>
* <span data-ttu-id="68791-595">Azure(RDFE)</span><span class="sxs-lookup"><span data-stu-id="68791-595">Azure (RDFE)</span></span>
    - <span data-ttu-id="68791-596">모든 RemoteApp Cmdlet 제거</span><span class="sxs-lookup"><span data-stu-id="68791-596">Removed all RemoteApp Cmdles</span></span>
* <span data-ttu-id="68791-597">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="68791-597">Azure.Storage</span></span>
    - <span data-ttu-id="68791-598">Azure Storage 클라이언트 라이브러리 8.6.0 및 Azure Storage DataMovement 라이브러리 0.6.5로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="68791-598">Upgrade to Azure Storage Client Library 8.6.0 and Azure Storage DataMovement Library 0.6.5</span></span>

## <a name="20171110-version-501"></a><span data-ttu-id="68791-599">2017.11.10 버전 5.0.1</span><span class="sxs-lookup"><span data-stu-id="68791-599">2017.11.10 Version 5.0.1</span></span>
* <span data-ttu-id="68791-600">다음과 같은 모듈에서 실행할 때 몇 가지 cmdlet이 실패하는 어셈블리 로딩 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="68791-600">Fixed assembly loading issue that caused some cmdlets to fail when executing in the following modules:</span></span>
  - <span data-ttu-id="68791-601">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="68791-601">AzureRM.ApiManagement</span></span>
  - <span data-ttu-id="68791-602">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="68791-602">AzureRM.Backup</span></span>
  - <span data-ttu-id="68791-603">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="68791-603">AzureRM.Batch</span></span>
  - <span data-ttu-id="68791-604">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="68791-604">AzureRM.Compute</span></span>
  - <span data-ttu-id="68791-605">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="68791-605">AzureRM.DataFactories</span></span>
  - <span data-ttu-id="68791-606">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="68791-606">AzureRM.HDInsight</span></span>
  - <span data-ttu-id="68791-607">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="68791-607">AzureRM.KeyVault</span></span>
  - <span data-ttu-id="68791-608">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="68791-608">AzureRM.RecoveryServices</span></span>
  - <span data-ttu-id="68791-609">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="68791-609">AzureRM.RecoveryServices.Backup</span></span>
  - <span data-ttu-id="68791-610">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="68791-610">AzureRM.RecoveryServices.SiteRecovery</span></span>
  - <span data-ttu-id="68791-611">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="68791-611">AzureRM.RedisCache</span></span>
  - <span data-ttu-id="68791-612">AzureRM.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="68791-612">AzureRM.SiteRecovery</span></span>
  - <span data-ttu-id="68791-613">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="68791-613">AzureRM.Sql</span></span>
  - <span data-ttu-id="68791-614">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="68791-614">AzureRM.Storage</span></span>
  - <span data-ttu-id="68791-615">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="68791-615">AzureRM.StreamAnalytics</span></span>

## <a name="2017118---version-500"></a><span data-ttu-id="68791-616">2017.11.8 - 버전 5.0.0</span><span class="sxs-lookup"><span data-stu-id="68791-616">2017.11.8 - Version 5.0.0</span></span>
* <span data-ttu-id="68791-617">참고: 이는 중요 변경 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-617">NOTE: This is a breaking change release.</span></span> <span data-ttu-id="68791-618">중요 변경 사항의 전체 목록은 마이그레이션 가이드(https://aka.ms/azps-migration-guide))를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="68791-618">Please see the migration guide (https://aka.ms/azps-migration-guide) for a full list of introduced breaking changes.</span></span>
* <span data-ttu-id="68791-619">AzureRM의 모든 cmdlet는 이제 온라인 도움말을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-619">All cmdlets in AzureRM now support online help</span></span>
  - <span data-ttu-id="68791-620">-Online 매개 변수와 함께 Get-Help를 실행하여 기본 인터넷 브라우저에서 온라인 도움말을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="68791-620">Run Get-Help with the -Online parameter to open the online help in your default Internet browser</span></span>
* <span data-ttu-id="68791-621">AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="68791-621">AnalysisServices</span></span>
  * <span data-ttu-id="68791-622">동기화를 위해 새로운 AsAzure REST API로 작동하도록 Synchronize-AzureAsInstance 명령 수정</span><span class="sxs-lookup"><span data-stu-id="68791-622">Fixed Synchronize-AzureAsInstance command to work with new AsAzure REST API for sync</span></span>
* <span data-ttu-id="68791-623">ApiManagement</span><span class="sxs-lookup"><span data-stu-id="68791-623">ApiManagement</span></span>
  * <span data-ttu-id="68791-624">이 릴리스의 ApiManagement에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="68791-624">Please see the migration guide for breaking changes made to ApiManagement this release</span></span>
  * <span data-ttu-id="68791-625">문제 https://github.com/Azure/azure-powershell/issues/4510의 수정을 위해 Cmdlet Get-AzureRmApiManagementUser 업데이트</span><span class="sxs-lookup"><span data-stu-id="68791-625">Updated Cmdlet Get-AzureRmApiManagementUser to fix issue https://github.com/Azure/azure-powershell/issues/4510</span></span>
  * <span data-ttu-id="68791-626">https://github.com/Azure/azure-powershell/issues/4069의 경로가 비어 있는 API 생성을 위해 Cmdlet New-AzureRmApiManagementApi 업데이트</span><span class="sxs-lookup"><span data-stu-id="68791-626">Updated Cmdlet New-AzureRmApiManagementApi to create Api with Empty Path https://github.com/Azure/azure-powershell/issues/4069</span></span>
* <span data-ttu-id="68791-627">ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="68791-627">ApplicationInsights</span></span>
  * <span data-ttu-id="68791-628">applicaiton insights 리소스를 가져오기/만들기/제거하기 위해 명령 추가</span><span class="sxs-lookup"><span data-stu-id="68791-628">Add commands to get/create/remove applicaiton insights resource</span></span>
    - <span data-ttu-id="68791-629">Get AzureRmApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="68791-629">Get-AzureRmApplicationInsights</span></span>
    - <span data-ttu-id="68791-630">Get AzureRmApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="68791-630">New-AzureRmApplicationInsights</span></span>
    - <span data-ttu-id="68791-631">Get AzureRmApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="68791-631">Remove-AzureRmApplicationInsights</span></span>
  * <span data-ttu-id="68791-632">application insights 리소스의 가격 책정/일일 상한선을 가져오기/업데이트하기 위해 명령 추가</span><span class="sxs-lookup"><span data-stu-id="68791-632">Add commands to get/update pricing/daily cap of applicaiton insights resource</span></span>
    - <span data-ttu-id="68791-633">Get-AzureRmApplicationInsights -IncludeDailyCap</span><span class="sxs-lookup"><span data-stu-id="68791-633">Get-AzureRmApplicationInsights -IncludeDailyCap</span></span>
    - <span data-ttu-id="68791-634">Set-AzureRmApplicationInsightsPricingPlan</span><span class="sxs-lookup"><span data-stu-id="68791-634">Set-AzureRmApplicationInsightsPricingPlan</span></span>
    - <span data-ttu-id="68791-635">Set-AzureRmApplicationInsightsDailyCap</span><span class="sxs-lookup"><span data-stu-id="68791-635">Set-AzureRmApplicationInsightsDailyCap</span></span>
  * <span data-ttu-id="68791-636">applicaiton insights 리소스의 연속 내보내기를 가져오기/만들기/업데이트하기/제거하기 위해 명령 추가</span><span class="sxs-lookup"><span data-stu-id="68791-636">Add commands to get/create/update/remove continuous export of applicaiton insights resource</span></span>
    - <span data-ttu-id="68791-637">Get-AzureRmApplicationInsightsContinuousExport</span><span class="sxs-lookup"><span data-stu-id="68791-637">Get-AzureRmApplicationInsightsContinuousExport</span></span>
    - <span data-ttu-id="68791-638">Set-AzureRmApplicationInsightsContinuousExport</span><span class="sxs-lookup"><span data-stu-id="68791-638">Set-AzureRmApplicationInsightsContinuousExport</span></span>
    - <span data-ttu-id="68791-639">New-AzureRmApplicationInsightsContinuousExport</span><span class="sxs-lookup"><span data-stu-id="68791-639">New-AzureRmApplicationInsightsContinuousExport</span></span>
    - <span data-ttu-id="68791-640">Remove-AzureRmApplicationInsightsContinuousExport</span><span class="sxs-lookup"><span data-stu-id="68791-640">Remove-AzureRmApplicationInsightsContinuousExport</span></span>
  * <span data-ttu-id="68791-641">applicaiton insights 리소스의 api 키를 가져오기/만들기/제거하기 위해 명령 추가</span><span class="sxs-lookup"><span data-stu-id="68791-641">Add commands to get/create/remove api keys of applicaiton insights resoruce</span></span>
    - <span data-ttu-id="68791-642">Get-AzureRmApplicationInsightsApiKey</span><span class="sxs-lookup"><span data-stu-id="68791-642">Get-AzureRmApplicationInsightsApiKey</span></span>
    - <span data-ttu-id="68791-643">New-AzureRmApplicationInsightsApiKey</span><span class="sxs-lookup"><span data-stu-id="68791-643">New-AzureRmApplicationInsightsApiKey</span></span>
    - <span data-ttu-id="68791-644">Remove-AzureRmApplicationInsightsApiKey</span><span class="sxs-lookup"><span data-stu-id="68791-644">Remove-AzureRmApplicationInsightsApiKey</span></span>
* <span data-ttu-id="68791-645">AzureBatch</span><span class="sxs-lookup"><span data-stu-id="68791-645">AzureBatch</span></span>
  * <span data-ttu-id="68791-646">`New-AzureRmBatchAccount`에 새 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-646">Added new parameters to `New-AzureRmBatchAccount`.</span></span>
    - <span data-ttu-id="68791-647">`PoolAllocationMode`: 배치 계정에서 풀을 만드는 데 사용하는 할당 모드입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-647">`PoolAllocationMode`: The allocation mode to use for creating pools in the Batch account.</span></span> <span data-ttu-id="68791-648">사용자의 구독에서 풀 노드를 할당하는 배치 계정을 만들려면 이를 `UserSubscription`으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-648">To create a Batch account which allocates pool nodes in the user's subscription, set this to `UserSubscription`.</span></span>
    - <span data-ttu-id="68791-649">`KeyVaultId`: 배치 계정과 연결된 Azure Key Vault의 리소스 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-649">`KeyVaultId`: The resource ID of the Azure key vault associated with the Batch account.</span></span>
    - <span data-ttu-id="68791-650">`KeyVaultUrl`: 배치 계정과 연결된 Azure Key Vault의 URL입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-650">`KeyVaultUrl`: The URL of the Azure key vault associated with the Batch account.</span></span>
  * <span data-ttu-id="68791-651">매개 변수를 `New-AzureBatchTask`로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-651">Updated parameters to `New-AzureBatchTask`.</span></span>
    - <span data-ttu-id="68791-652">`RunElevated` 스위치를 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-652">Removed the `RunElevated` switch.</span></span> <span data-ttu-id="68791-653">`UserIdentity` 매개 변수가 `RunElevated`를 대체하기 위해 추가되었으며, 아래와 같이 `PSUserIdentity`를 구성하여 동등한 동작을 얻을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-653">The `UserIdentity` parameter has been added to replace `RunElevated`, and the equivalent behavior can be achieved by constructing a `PSUserIdentity` as shown below:</span></span>
      - <span data-ttu-id="68791-654">$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")</span><span class="sxs-lookup"><span data-stu-id="68791-654">$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")</span></span>
      - <span data-ttu-id="68791-655">$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser</span><span class="sxs-lookup"><span data-stu-id="68791-655">$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser</span></span>
    - <span data-ttu-id="68791-656">`AuthenticationTokenSettings` 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-656">Added the `AuthenticationTokenSettings` parameter.</span></span> <span data-ttu-id="68791-657">이 매개 변수를 사용하면 실행할 때 일괄 처리 서비스가 인증 토큰을 작업에 제공하도록 요청할 수 있어, 일괄 처리 서비스에 요청을 발행하기 위해 배치 계정 키를 작업에 전달할 필요가 없게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="68791-657">This parameter allows you to request the Batch service provide an authentication token to the task when it runs, avoiding the need to pass Batch account keys to the task in order to issue requests to the Batch service.</span></span>
    - <span data-ttu-id="68791-658">`ContainerSettings` 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-658">Added the `ContainerSettings` parameter.</span></span>
      - <span data-ttu-id="68791-659">이 매개 변수를 사용하면 일괄 처리 서비스가 컨테이너 내의 작업을 실행하도록 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-659">This parameter allows you to request the Batch service run the task inside a container.</span></span>
    - <span data-ttu-id="68791-660">`OutputFiles` 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-660">Added the `OutputFiles` parameter.</span></span>
      - <span data-ttu-id="68791-661">이 매개 변수를 사용하면 완료된 후 Azure Storage에 파일을 업로드하는 작업을 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-661">This parameter allows you to configure the task to upload files to Azure Storage after it has finished.</span></span>
  * <span data-ttu-id="68791-662">매개 변수를 `New-AzureBatchPool`로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-662">Updated parameters to `New-AzureBatchPool`.</span></span>
    - <span data-ttu-id="68791-663">`UserAccounts` 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-663">Added the `UserAccounts` parameter.</span></span>
      - <span data-ttu-id="68791-664">이 매개 변수는 풀의 각 노드에서 만든 사용자 계정을 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-664">This parameter defines user accounts created on each node in the pool.</span></span>
    - <span data-ttu-id="68791-665">`TargetLowPriorityComputeNodes`를 추가하고 `TargetDedicated`의 이름을 `TargetDedicatedComputeNodes`으로 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-665">Added `TargetLowPriorityComputeNodes` and renamed `TargetDedicated` to `TargetDedicatedComputeNodes`.</span></span>
      - <span data-ttu-id="68791-666">`TargetDedicatedComputeNodes` 매개 변수에 대해 `TargetDedicated` 별칭이 만들어졌습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-666">A `TargetDedicated` alias was created for the `TargetDedicatedComputeNodes` parameter.</span></span>
    - <span data-ttu-id="68791-667">`NetworkConfiguration` 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-667">Added the `NetworkConfiguration` parameter.</span></span>
      - <span data-ttu-id="68791-668">이 매개 변수를 사용하면 풀 네트워크 설정을 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-668">This parameter allows you to configure the pools network settings.</span></span>
  * <span data-ttu-id="68791-669">매개 변수를 `New-AzureBatchCertificate`로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-669">Updated parameters to `New-AzureBatchCertificate`.</span></span>
    - <span data-ttu-id="68791-670">`Password` 매개 변수가 이제 `SecureString`이 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-670">The `Password` parameter is now a `SecureString`.</span></span>
  * <span data-ttu-id="68791-671">매개 변수를 `New-AzureBatchComputeNodeUser`로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-671">Updated parameters to `New-AzureBatchComputeNodeUser`.</span></span>
    - <span data-ttu-id="68791-672">`Password` 매개 변수가 이제 `SecureString`이 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-672">The `Password` parameter is now a `SecureString`.</span></span>
  * <span data-ttu-id="68791-673">매개 변수를 `Set-AzureBatchComputeNodeUser`로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-673">Updated parameters to `Set-AzureBatchComputeNodeUser`.</span></span>
    - <span data-ttu-id="68791-674">`Password` 매개 변수가 이제 `SecureString`이 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-674">The `Password` parameter is now a `SecureString`.</span></span>
  * <span data-ttu-id="68791-675">`Get-AzureBatchNodeFile`, `Get-AzureBatchNodeFileContent`, 및 `Remove-AzureBatchNodeFile`에서 `Name` 매개 변수의 이름이 `Path`로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-675">Renamed the `Name` parameter to `Path` on `Get-AzureBatchNodeFile`, `Get-AzureBatchNodeFileContent`, and `Remove-AzureBatchNodeFile`.</span></span>
    - <span data-ttu-id="68791-676">`Path` 매개 변수에 대해 `Name` 별칭이 만들어졌습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-676">A `Name` alias was created for the `Path` parameter.</span></span>
  * <span data-ttu-id="68791-677">개체에 대한 변경 사항</span><span class="sxs-lookup"><span data-stu-id="68791-677">Changes to objects</span></span>
    - <span data-ttu-id="68791-678">전체 목록은 일괄 처리 변경 로그를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="68791-678">Please see the Batch change log for the full list</span></span>
  * <span data-ttu-id="68791-679">Azure Active Directory 기반 인증에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-679">Added support for Azure Active Directory based authentication.</span></span>
    - <span data-ttu-id="68791-680">Azure Active Directory 인증을 사용하려면 `Get-AzureRmBatchAccount` cmdlet를 사용하여 `BatchAccountContext` 개체를 검색하고 이 `BatchAccountContext`를 일괄 처리 서비스 cmdlet의 `-BatchContext` 매개 변수에 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-680">To use Azure Active Directory authentication, retrieve a `BatchAccountContext` object using the `Get-AzureRmBatchAccount` cmdlet, and supply this `BatchAccountContext` to the `-BatchContext` parameter of a Batch service cmdlet.</span></span> <span data-ttu-id="68791-681">Azure Active Directory 인증은 `PoolAllocationMode = UserSubscription`이 있는 계정에 필수입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-681">Azure Active Directory authentication is mandatory for accounts with `PoolAllocationMode = UserSubscription`.</span></span>
    - <span data-ttu-id="68791-682">기존 계정 또는 `PoolAllocationMode = BatchService`로 만든 새 계정의 경우, `Get-AzureRmBatchAccoutKeys` cmdlet를 사용하는 `BatchAccountContext` 개체를 검색하여 공유 키 인증을 계속 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-682">For existing accounts or for new accounts created with `PoolAllocationMode = BatchService`, you may continue to use shared key authentication by retrieving a `BatchAccountContext` object using the `Get-AzureRmBatchAccoutKeys` cmdlet.</span></span>
* <span data-ttu-id="68791-683">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="68791-683">Compute</span></span>
  * <span data-ttu-id="68791-684">Azure Disk Encryption 확장 명령</span><span class="sxs-lookup"><span data-stu-id="68791-684">Azure Disk Encryption Extension Commands</span></span>
    - <span data-ttu-id="68791-685">'Set-AzureRmVmDiskEncryptionExtension'에 대한 새 매개 변수': '-EncryptFormatAll' 암호화 형식 데이터 디스크</span><span class="sxs-lookup"><span data-stu-id="68791-685">New Parameter for 'Set-AzureRmVmDiskEncryptionExtension': '-EncryptFormatAll' encrypt formats data disks</span></span>
    - <span data-ttu-id="68791-686">'Set-AzureRmVmDiskEncryptionExtension'에 대한 새로운 매개 변수: '-ExtensionPublisherName' 및 '-ExtensionType'이 다른 확장 버전으로 전환 허용</span><span class="sxs-lookup"><span data-stu-id="68791-686">New Parameters for 'Set-AzureRmVmDiskEncryptionExtension': '-ExtensionPublisherName' and '-ExtensionType' allow switching to other versions of the extension</span></span>
    - <span data-ttu-id="68791-687">'Disable-AzureRmVmDiskEncryption'에 대한 새로운 매개 변수: '-ExtensionPublisherName' 및 '-ExtensionType'이 다른 확장 버전으로 전환 허용</span><span class="sxs-lookup"><span data-stu-id="68791-687">New Parameters for 'Disable-AzureRmVmDiskEncryption': '-ExtensionPublisherName' and '-ExtensionType' allow switching to other versions of the extension</span></span>
    - <span data-ttu-id="68791-688">'Get-AzureRmVmDiskEncryptionStatus'에 대한 새로운 매개 변수: '-ExtensionPublisherName' 및 '-ExtensionType'이 다른 확장 버전으로 전환 허용</span><span class="sxs-lookup"><span data-stu-id="68791-688">New Parameters for 'Get-AzureRmVmDiskEncryptionStatus': '-ExtensionPublisherName' and '-ExtensionType' allow switching to other versions of the extension</span></span>
* <span data-ttu-id="68791-689">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="68791-689">DataLakeAnalytics</span></span>
  * <span data-ttu-id="68791-690">이 릴리스의 DataLakeAnalytics에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="68791-690">Please see the migration guide for breaking changes made to DataLakeAnalytics this release</span></span>
  * <span data-ttu-id="68791-691">Get-AzureRmDataLakeAnalyticsAccount의 두 가지 OutputTypes 중 하나를 변경</span><span class="sxs-lookup"><span data-stu-id="68791-691">Changed one of the two OutputTypes of Get-AzureRmDataLakeAnalyticsAccount</span></span>
    - <span data-ttu-id="68791-692">목록\<DataLakeAnalyticsAccount> 목록\<PSDataLakeAnalyticsAccountBasic>으로</span><span class="sxs-lookup"><span data-stu-id="68791-692">List\<DataLakeAnalyticsAccount> to List\<PSDataLakeAnalyticsAccountBasic></span></span>
    - <span data-ttu-id="68791-693">PSDataLakeAnalyticsAccountBasic의 속성은 DataLakeAnalyticsAccount 속성의 엄격한 하위 집합입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-693">The properties of PSDataLakeAnalyticsAccountBasic is a strict subset of the properties of DataLakeAnalyticsAccount</span></span>
    - <span data-ttu-id="68791-694">DataLakeAnalyticsAccount에 있는 추가 속성은 서비스에 의해 반환되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-694">The additional properties that are in DataLakeAnalyticsAccount are not returned by the service.</span></span>  <span data-ttu-id="68791-695">따라서 이 변경 사항은 이를 정확하게 반영합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-695">Therefore, this change is to reflect this accurately.</span></span> <span data-ttu-id="68791-696">이러한 추가 속성은 PSDataLakeAnalyticsAccountBasic에 여전히 있지만, Obsolete로 태그가 지정됩니다.</span><span class="sxs-lookup"><span data-stu-id="68791-696">These additional properties are still in PSDataLakeAnalyticsAccountBasic, but they are tagged as Obsolete.</span></span>
  * <span data-ttu-id="68791-697">Get-AzureRmDataLakeAnalyticsJob의 두 가지 OutputTypes 중 하나를 변경</span><span class="sxs-lookup"><span data-stu-id="68791-697">Changed one of the two OutputTypes of Get-AzureRmDataLakeAnalyticsJob</span></span>
    - <span data-ttu-id="68791-698">목록\<JobInformation> 목록\<PSJobInformationBasic>으로</span><span class="sxs-lookup"><span data-stu-id="68791-698">List\<JobInformation> to List\<PSJobInformationBasic></span></span>
    - <span data-ttu-id="68791-699">PSJobInformationBasic 속성은 JobInformation 속성의 엄격한 하위 집합입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-699">The properties of PSJobInformationBasic is a strict subset of the properties of JobInformation</span></span>
    - <span data-ttu-id="68791-700">JobInformation에 있는 추가 속성은 서비스에 의해 반환되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-700">The additional properties that are in JobInformation are not returned by the service.</span></span>  <span data-ttu-id="68791-701">따라서 이 변경 사항은 이를 정확하게 반영합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-701">Therefore, this change is to reflect this accurately.</span></span> <span data-ttu-id="68791-702">이러한 추가 속성은 PSJobInformationBasic에 여전히 있지만, Obsolete로 태그가 지정됩니다.</span><span class="sxs-lookup"><span data-stu-id="68791-702">These additional properties are still in PSJobInformationBasic, but they are tagged as Obsolete.</span></span>
* <span data-ttu-id="68791-703">DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="68791-703">DataLakeStore</span></span>
  * <span data-ttu-id="68791-704">이 릴리스의 DataLakeStore에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="68791-704">Please see the migration guide for breaking changes made to DataLakeStore this release</span></span>
  * <span data-ttu-id="68791-705">Get-AzureRmDataLakeStoreAccount의 두 가지 OutputTypes 중 하나를 변경</span><span class="sxs-lookup"><span data-stu-id="68791-705">Changed one of the two OutputTypes of Get-AzureRmDataLakeStoreAccount</span></span>
    - <span data-ttu-id="68791-706">목록\<PSDataLakeStoreAccount> 목록\<PSDataLakeStoreAccountBasic>으로</span><span class="sxs-lookup"><span data-stu-id="68791-706">List\<PSDataLakeStoreAccount> to List\<PSDataLakeStoreAccountBasic></span></span>
    - <span data-ttu-id="68791-707">PSDataLakeStoreAccountBasic의 속성은 PSDataLakeStoreAccount 속성의 엄격한 하위 집합입니다.</span><span class="sxs-lookup"><span data-stu-id="68791-707">The properties of PSDataLakeStoreAccountBasic is a strict subset of the properties of PSDataLakeStoreAccount</span></span>
    - <span data-ttu-id="68791-708">PSDataLakeStoreAccount에 있는 추가 속성은 서비스에 의해 반환되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-708">The additional properties that are in PSDataLakeStoreAccount are not returned by the service.</span></span>  <span data-ttu-id="68791-709">따라서 이 변경 사항은 이를 정확하게 반영합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-709">Therefore, this change is to reflect this accurately.</span></span> <span data-ttu-id="68791-710">이러한 추가 속성은 PSDataLakeStoreAccountBasic에 여전히 있지만, Obsolete로 태그가 지정됩니다.</span><span class="sxs-lookup"><span data-stu-id="68791-710">These additional properties are still in PSDataLakeStoreAccountBasic, but they are tagged as Obsolete.</span></span>
* <span data-ttu-id="68791-711">Dns</span><span class="sxs-lookup"><span data-stu-id="68791-711">Dns</span></span>
  * <span data-ttu-id="68791-712">Azure DNS의 CAA 레코드 종류에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="68791-712">Support for CAA record types in Azure DNS</span></span>
    - <span data-ttu-id="68791-713">CAA 레코드 종류에서 모든 작업 지원</span><span class="sxs-lookup"><span data-stu-id="68791-713">Supports all operations on CAA record type</span></span>
* <span data-ttu-id="68791-714">EventHub</span><span class="sxs-lookup"><span data-stu-id="68791-714">EventHub</span></span>
  * <span data-ttu-id="68791-715">이 릴리스의 EventHub에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="68791-715">Please see the migration guide for breaking changes made to EventHub this release</span></span>
* <span data-ttu-id="68791-716">자세한 정보</span><span class="sxs-lookup"><span data-stu-id="68791-716">Insights</span></span>
  * <span data-ttu-id="68791-717">이 릴리스의 Insights에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="68791-717">Please see the migration guide for breaking changes made to Insights this release</span></span>
* <span data-ttu-id="68791-718">네트워크</span><span class="sxs-lookup"><span data-stu-id="68791-718">Network</span></span>
  * <span data-ttu-id="68791-719">이 릴리스의 Network에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="68791-719">Please see the migration guide for breaking changes made to Network this release</span></span>
  * <span data-ttu-id="68791-720">지정된 Azure 지역에 대해 사용 가능한 인터넷 서비스 공급자를 나열하는 cmdlet이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-720">Added cmdlet to list available internet service providers for a specified Azure region</span></span>
    - <span data-ttu-id="68791-721">Get-AzureRmNetworkWatcherReachabilityProvidersList</span><span class="sxs-lookup"><span data-stu-id="68791-721">Get-AzureRmNetworkWatcherReachabilityProvidersList</span></span>
  * <span data-ttu-id="68791-722">지정된 위치에서 Azure 지역까지 인터넷 서비스 공급자에 대한 상대적 대기 시간 점수를 얻기 위한 cmdlet이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-722">Added cmdlet to get the relative latency score for internet service providers from a specified location to Azure regions</span></span>
    - <span data-ttu-id="68791-723">Get-AzureRmNetworkWatcherReachabilityReport</span><span class="sxs-lookup"><span data-stu-id="68791-723">Get-AzureRmNetworkWatcherReachabilityReport</span></span>
* <span data-ttu-id="68791-724">프로필</span><span class="sxs-lookup"><span data-stu-id="68791-724">Profile</span></span>
  - <span data-ttu-id="68791-725">Set-AzureRmDefault</span><span class="sxs-lookup"><span data-stu-id="68791-725">Set-AzureRmDefault</span></span>
    - <span data-ttu-id="68791-726">이 cmdlet을 사용하여 기본 리소스 그룹을 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-726">Use this cmdlet to set a default resource group.</span></span>  <span data-ttu-id="68791-727">이렇게 하면 일부 cmdlet에 대해 -ResourceGroup 매개 변수가 선택 사항이 되고 리소스 그룹이 지정되지 않은 경우 기본값이 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="68791-727">This will make the -ResourceGroup parameter optional for some cmdlets, and will use the default when a resource group is not specified</span></span>
    - ```Set-AzureRmDefault -ResourceGroupName "ExampleResourceGroup"```
    - <span data-ttu-id="68791-728">구독에 지정된 리소스 그룹이 있으면 이 리소스 그룹은 기본값으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="68791-728">If resource group specified exists in the subscription, this resource group will be set to default.</span></span>  <span data-ttu-id="68791-729">그렇지 않은 경우 리소스 그룹이 만들어진 다음 기본값으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="68791-729">Otherwise, the resource group will be created and then set to default.</span></span>
  - <span data-ttu-id="68791-730">Get-AzureRmDefault</span><span class="sxs-lookup"><span data-stu-id="68791-730">Get-AzureRmDefault</span></span>
    - <span data-ttu-id="68791-731">이 cmdlet을 사용하여 현재 기본 리소스 그룹(및 나중의 다른 기본값)을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="68791-731">Use this cmdlet to get the current default resource group (and other defaults in the future).</span></span>
    - ```Get-AzureRmDefault -ResourceGroup```
  - <span data-ttu-id="68791-732">Clear-AzureRmDefault</span><span class="sxs-lookup"><span data-stu-id="68791-732">Clear-AzureRmDefault</span></span>
    - <span data-ttu-id="68791-733">이 cmdlet을 사용하여 현재 기본 리소스 그룹을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-733">Use this cmdlet to remove the current default resource group</span></span>
    - ```Clear-AzureRmDefault -ResourceGroup```
  - <span data-ttu-id="68791-734">Add-AzureRmEnvironment 및 Set-AzureRmEnvironment</span><span class="sxs-lookup"><span data-stu-id="68791-734">Add-AzureRmEnvironment and Set-AzureRmEnvironment</span></span>
    - <span data-ttu-id="68791-735">일괄 처리 서비스에 대한 인증 토큰을 얻을 때 사용할 Azure Batch Active Directory 대상을 지정할 수 있는 BatchAudience 매개 변수를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-735">Add the BatchAudience parameter, which allows you to specify the Azure Batch Active Directory audience to use when acquiring authentication tokens for the Batch service.</span></span>
* <span data-ttu-id="68791-736">RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="68791-736">RecoveryServices.Backup</span></span>
  * <span data-ttu-id="68791-737">즉시 파일 복구를 수행하기 위해 cmdlet을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-737">Added cmdlets to perform instant file recovery.</span></span>
    - <span data-ttu-id="68791-738">Get-AzureRmRecoveryServicesBackupRPMountScript</span><span class="sxs-lookup"><span data-stu-id="68791-738">Get-AzureRmRecoveryServicesBackupRPMountScript</span></span>
    - <span data-ttu-id="68791-739">Disable-AzureRmRecoveryServicesBackupRPMountScript</span><span class="sxs-lookup"><span data-stu-id="68791-739">Disable-AzureRmRecoveryServicesBackupRPMountScript</span></span>
  * <span data-ttu-id="68791-740">RecoveryServices.Backup SDK 버전을 최신 버전으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="68791-740">Updated RecoveryServices.Backup SDK version to the latest</span></span>
  * <span data-ttu-id="68791-741">테스트 실행에 필요한 모든 설정이 테스트 자체에서 지정되도록 Azure VM 워크로드에 대한 테스트를 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="68791-741">Updated tests for the Azure VM workload so that, all setups needed for test runs are done by the tests themselves.</span></span>
  * <span data-ttu-id="68791-742">https://github.com/Azure/azure-powershell/issues/3164 수정</span><span class="sxs-lookup"><span data-stu-id="68791-742">Fixes https://github.com/Azure/azure-powershell/issues/3164</span></span>
* <span data-ttu-id="68791-743">RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="68791-743">RecoveryServices.SiteRecovery</span></span>
  * <span data-ttu-id="68791-744">ASR VMware의 Azure Site Recovery에 대한 변경 사항(cmdlet은 현재 Enterprise-Enterprise, Enterprise-Azure, HyperV-Azure에 대한 작업을 지원)</span><span class="sxs-lookup"><span data-stu-id="68791-744">Changes for ASR VMware to Azure Site Recovery (cmdlets are currently supporting operations for Enterprise to Enterprise, Enterprise to Azure, HyperV to Azure)</span></span>
    - <span data-ttu-id="68791-745">New-AzureRmRecoveryServicesAsrPolicy</span><span class="sxs-lookup"><span data-stu-id="68791-745">New-AzureRmRecoveryServicesAsrPolicy</span></span>
    - <span data-ttu-id="68791-746">New-AzureRmRecoveryServicesAsrProtectedItem</span><span class="sxs-lookup"><span data-stu-id="68791-746">New-AzureRmRecoveryServicesAsrProtectedItem</span></span>
    - <span data-ttu-id="68791-747">Update-AzureRmRecoveryServicesAsrPolicy</span><span class="sxs-lookup"><span data-stu-id="68791-747">Update-AzureRmRecoveryServicesAsrPolicy</span></span>
    - <span data-ttu-id="68791-748">Update-AzureRmRecoveryServicesAsrProtectionDirection</span><span class="sxs-lookup"><span data-stu-id="68791-748">Update-AzureRmRecoveryServicesAsrProtectionDirection</span></span>
  * <span data-ttu-id="68791-749">AAD 기반 자격 증명 모음에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-749">Added support to AAD-based vault</span></span>
  * <span data-ttu-id="68791-750">VCenter 리소스를 관리하기 위해 cmdlet이 추가됨</span><span class="sxs-lookup"><span data-stu-id="68791-750">Added cmdlets to manage VCenter resources</span></span>
    - <span data-ttu-id="68791-751">Get-AzureRmRecoveryServicesAsrVCenter</span><span class="sxs-lookup"><span data-stu-id="68791-751">Get-AzureRmRecoveryServicesAsrVCenter</span></span>
    - <span data-ttu-id="68791-752">New-AzureRmRecoveryServicesAsrVCenter</span><span class="sxs-lookup"><span data-stu-id="68791-752">New-AzureRmRecoveryServicesAsrVCenter</span></span>
    - <span data-ttu-id="68791-753">Remove-AzureRmRecoveryServicesAsrVCenter</span><span class="sxs-lookup"><span data-stu-id="68791-753">Remove-AzureRmRecoveryServicesAsrVCenter</span></span>
    - <span data-ttu-id="68791-754">Update-AzureRmRecoveryServicesAsrVCenter</span><span class="sxs-lookup"><span data-stu-id="68791-754">Update-AzureRmRecoveryServicesAsrVCenter</span></span>
  * <span data-ttu-id="68791-755">다른 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="68791-755">Added other cmdlets</span></span>
    - <span data-ttu-id="68791-756">Get-AzureRmRecoveryServicesAsrAlertSetting</span><span class="sxs-lookup"><span data-stu-id="68791-756">Get-AzureRmRecoveryServicesAsrAlertSetting</span></span>
    - <span data-ttu-id="68791-757">Get-AzureRmRecoveryServicesAsrEvent</span><span class="sxs-lookup"><span data-stu-id="68791-757">Get-AzureRmRecoveryServicesAsrEvent</span></span>
    - <span data-ttu-id="68791-758">New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="68791-758">New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
    - <span data-ttu-id="68791-759">Set-AzureRmRecoveryServicesAsrAlertSetting</span><span class="sxs-lookup"><span data-stu-id="68791-759">Set-AzureRmRecoveryServicesAsrAlertSetting</span></span>
    - <span data-ttu-id="68791-760">Start-AzureRmRecoveryServicesAsrResynchronizeReplicationJob</span><span class="sxs-lookup"><span data-stu-id="68791-760">Start-AzureRmRecoveryServicesAsrResynchronizeReplicationJob</span></span>
    - <span data-ttu-id="68791-761">Start-AzureRmRecoveryServicesAsrSwitchProcessServerJob</span><span class="sxs-lookup"><span data-stu-id="68791-761">Start-AzureRmRecoveryServicesAsrSwitchProcessServerJob</span></span>
    - <span data-ttu-id="68791-762">Start-AzureRmRecoveryServicesAsrTestFailoverCleanupJob</span><span class="sxs-lookup"><span data-stu-id="68791-762">Start-AzureRmRecoveryServicesAsrTestFailoverCleanupJob</span></span>
    - <span data-ttu-id="68791-763">Update-AzureRmRecoveryServicesAsrMobilityService</span><span class="sxs-lookup"><span data-stu-id="68791-763">Update-AzureRmRecoveryServicesAsrMobilityService</span></span>
* <span data-ttu-id="68791-764">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="68791-764">ServiceBus</span></span>
  - <span data-ttu-id="68791-765">이 릴리스의 ServiceBus에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="68791-765">Please see the migration guide for breaking changes made to ServiceBus this release</span></span>
* <span data-ttu-id="68791-766">Sql</span><span class="sxs-lookup"><span data-stu-id="68791-766">Sql</span></span>
  * <span data-ttu-id="68791-767">목록에 대한 지원 추가 및 데이터베이스에서 비동기 updatelo 작업 취소</span><span class="sxs-lookup"><span data-stu-id="68791-767">Adding support for list and cancel the asynchronous updateslo operation on the database</span></span>
    - <span data-ttu-id="68791-768">기존 cmdlet Get-AzureRmSqlDatabaseActivity를 업데이트하여 DB updateslo를 작업 상태로 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-768">update existing cmdlet Get-AzureRmSqlDatabaseActivity to return DB updateslo operation status.</span></span>
    - <span data-ttu-id="68791-769">새 cmdlet Stop-AzureRmSqlDatabaseActivity를 추가하여 데이터베이스에서 비동기 updateslo 작업을 취소합니다.</span><span class="sxs-lookup"><span data-stu-id="68791-769">add new cmdlet Stop-AzureRmSqlDatabaseActivity for cancel the asynchronous updateslo operation on the database.</span></span>
  * <span data-ttu-id="68791-770">데이터베이스 및 탄성 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="68791-770">Adding support for Zone Redundancy for databases and elastic pools</span></span>
    - <span data-ttu-id="68791-771">New-AzureRmSqlDatabase에 ZoneRedundant 스위치 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="68791-771">Adding ZoneRedundant switch parameter to New-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="68791-772">Set-AzureRmSqlDatabase에 ZoneRedundant 스위치 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="68791-772">Adding ZoneRedundant switch parameter to Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="68791-773">New-AzureRmSqlElasticPool에 ZoneRedundant 스위치 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="68791-773">Adding ZoneRedundant switch parameter to New-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="68791-774">Set-AzureRmSqlElasticPool에 ZoneRedundant 스위치 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="68791-774">Adding ZoneRedundant switch parameter to Set-AzureRmSqlElasticPool</span></span>
  * <span data-ttu-id="68791-775">서버 DNS 별칭에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="68791-775">Adding support for Server DNS Aliases</span></span>
    - <span data-ttu-id="68791-776">서버 및 별칭 이름별 서버 DNS 별칭 또는 Azure SQL Server에 대한 서버 DNS 별칭의 목록을 가져오는 Get-AzureRmSqlServerDnsAlias cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="68791-776">Adding Get-AzureRmSqlServerDnsAlias cmdlet which gets server dns aliases by server and alias name or a list of server dns aliases for an azure Sql Server.</span></span>
    - <span data-ttu-id="68791-777">지정된 Azure SQL Server에 대한 새 서버 DNS 별칭을 만드는 New-AzureRmSqlServerDnsAlias cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="68791-777">Adding New-AzureRmSqlServerDnsAlias cmdlet which creates new server dns alias for a given Azure Sql server</span></span>
    - <span data-ttu-id="68791-778">서버 DNS 별칭이 가리키는 Azure SQL Server의 업데이트를 허용하는 Set-AzurermSqlServerDnsAlias cmlet 추가</span><span class="sxs-lookup"><span data-stu-id="68791-778">Adding Set-AzurermSqlServerDnsAlias cmlet which allows updating a Azure Sql Server to which server dns alias is pointing</span></span>
    - <span data-ttu-id="68791-779">Azure SQL Server에 대한 새 서버 DNS 별칭을 제거하는 Remove-AzureRmSqlServerDnsAlias cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="68791-779">Adding Remove-AzureRmSqlServerDnsAlias cmdlet which removes a server dns alias for a Azure Sql Server</span></span>
* <span data-ttu-id="68791-780">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="68791-780">Azure.Storage</span></span>
  * <span data-ttu-id="68791-781">Azure Storage 클라이언트 라이브러리 8.5.0 및 Azure Storage DataMovement 라이브러리 0.6.3으로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="68791-781">Upgrade to Azure Storage Client Library 8.5.0 and Azure Storage DataMovement Library 0.6.3</span></span>
  * <span data-ttu-id="68791-782">파일 공유 스냅숏 지원 기능 추가</span><span class="sxs-lookup"><span data-stu-id="68791-782">Add File Share Snapshot Support Feature</span></span>
    - <span data-ttu-id="68791-783">Get-AzureStorageShare에 'SnapshotTime' 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="68791-783">Add 'SnapshotTime' parameter to Get-AzureStorageShare</span></span>
    - <span data-ttu-id="68791-784">Remove-AzureStorageShare에 'IncludeAllSnapshot' 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="68791-784">Add 'IncludeAllSnapshot' parameter to Remove-AzureStorageShare</span></span>
