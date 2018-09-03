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
ms.openlocfilehash: 6043d17df1b5e91521bad31e65372c10ee6a5c6a
ms.sourcegitcommit: 9cb98f055a0525c2061f65149965d5e7c3e03ddc
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/30/2018
ms.locfileid: "43117392"
---
# <a name="release-notes"></a><span data-ttu-id="59cd0-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="59cd0-103">Release notes</span></span>

<span data-ttu-id="59cd0-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="680---august-2018"></a><span data-ttu-id="59cd0-105">6.8.0 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="59cd0-105">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="59cd0-106">일반</span><span class="sxs-lookup"><span data-stu-id="59cd0-106">General</span></span>
* <span data-ttu-id="59cd0-107">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-107">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="59cd0-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="59cd0-108">AzureRM.Profile</span></span>
* <span data-ttu-id="59cd0-109">Connect-AzureRmAccount 중에 반환된 토큰에 만료 속성 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-109">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="59cd0-110">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="59cd0-110">AzureRM.Compute</span></span>
* <span data-ttu-id="59cd0-111">오류 출력에 대상이 없는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-111">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="59cd0-112">관리 디스크를 사용하는 VM에 대한 저장소 계정 유형 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-112">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="59cd0-113">예를 들어 Azure 중국과 같이, 다른 환경에 대한 AEM 확장 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-113">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="59cd0-114">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="59cd0-114">AzureRM.IotHub</span></span>
* <span data-ttu-id="59cd0-115">New-AzureRmIotHubExportDevices 및 New-AzureRmIotHubImportDevices에 대한 예제를 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-115">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="59cd0-116">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="59cd0-116">AzureRM.Network</span></span>
* <span data-ttu-id="59cd0-117">기본 모델 표시를 테이블 뷰로 변경</span><span class="sxs-lookup"><span data-stu-id="59cd0-117">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="59cd0-118">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="59cd0-118">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="59cd0-119">일시 중지된 용량을 확장하려고 할 때 Update-AzureRmPowerBIEmbeddedCapacity 실패 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-119">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="59cd0-120">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="59cd0-120">AzureRM.Resources</span></span>
* <span data-ttu-id="59cd0-121">MarketPlace에서 관리되는 응용 프로그램 생성 시의 문제 해결.</span><span class="sxs-lookup"><span data-stu-id="59cd0-121">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="59cd0-122">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="59cd0-122">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="59cd0-123">문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-123">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="59cd0-124">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="59cd0-124">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="59cd0-125">다중값 라우팅 메서드에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="59cd0-125">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="59cd0-126">다중값 라우팅에 대한 새 매개 변수 'MaxReturn'</span><span class="sxs-lookup"><span data-stu-id="59cd0-126">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="59cd0-127">서브넷 라우팅 메서드에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="59cd0-127">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="59cd0-128">엔드포인트의 IP 주소 범위(서브넷)에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="59cd0-128">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="59cd0-129">프로필 내 사용자 지정 헤더에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="59cd0-129">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="59cd0-130">프로필 내 예상 상태 코드 범위에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="59cd0-130">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="59cd0-131">엔드포인트 내 사용자 지정 헤더에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="59cd0-131">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="59cd0-132">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="59cd0-132">AzureRM.Websites</span></span>
* <span data-ttu-id="59cd0-133">기본 리소스 그룹이 잘못 설정되는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-133">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="59cd0-134">6.7.0 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="59cd0-134">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="59cd0-135">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="59cd0-135">AzureRM.Profile</span></span>
* <span data-ttu-id="59cd0-136">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-136">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="59cd0-137">충돌을 방지하려면 기본 컨텍스트 이름으로 사용자 ID를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-137">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="59cd0-138">#6398 컨텍스트를 선택할 때 문제를 발생시킨 Clear-AzureRmContext 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-138">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="59cd0-139">'Connect-AzureRmAccount'에 대한 '-TenantId' 매개 변수에 전달할 테넌트 도메인을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="59cd0-139">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="59cd0-140">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="59cd0-140">Azure.Storage</span></span>
* <span data-ttu-id="59cd0-141">Azure 파일 공유 할당량에 대한 5TB 제한 제거</span><span class="sxs-lookup"><span data-stu-id="59cd0-141">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="59cd0-142">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="59cd0-142">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="59cd0-143">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="59cd0-143">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="59cd0-144">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-144">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="59cd0-145">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="59cd0-145">Azure.AnalysisServices</span></span>
* <span data-ttu-id="59cd0-146">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-146">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="59cd0-147">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="59cd0-147">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="59cd0-148">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-148">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="59cd0-149">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="59cd0-149">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="59cd0-150">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-150">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="59cd0-151">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="59cd0-151">AzureRM.Automation</span></span>
* <span data-ttu-id="59cd0-152">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-152">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="59cd0-153">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="59cd0-153">AzureRM.Backup</span></span>
* <span data-ttu-id="59cd0-154">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-154">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="59cd0-155">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="59cd0-155">AzureRM.Batch</span></span>
* <span data-ttu-id="59cd0-156">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-156">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="59cd0-157">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="59cd0-157">AzureRM.Billing</span></span>
* <span data-ttu-id="59cd0-158">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-158">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="59cd0-159">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="59cd0-159">AzureRM.Cdn</span></span>
* <span data-ttu-id="59cd0-160">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-160">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="59cd0-161">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="59cd0-161">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="59cd0-162">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-162">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="59cd0-163">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="59cd0-163">AzureRM.Compute</span></span>
* <span data-ttu-id="59cd0-164">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-164">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="59cd0-165">New-AzureRmVmssConfig에 EvictionPolicy 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-165">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="59cd0-166">지정된 위치가 없는 경우에 New-AzureRmVm의 DiskFileParameterSet 내의 기본 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-166">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="59cd0-167">Save-AzureRmVMImage에서 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-167">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="59cd0-168">특정 singlepass 관련 시나리오에 대해 Get-AzureRmVMDiskEncryptionStatus cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-168">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="59cd0-169">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="59cd0-169">AzureRM.Consumption</span></span>
* <span data-ttu-id="59cd0-170">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-170">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="59cd0-171">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="59cd0-171">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="59cd0-172">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-172">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="59cd0-173">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="59cd0-173">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="59cd0-174">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-174">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="59cd0-175">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="59cd0-175">AzureRM.DataFactories</span></span>
* <span data-ttu-id="59cd0-176">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-176">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="59cd0-177">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="59cd0-177">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="59cd0-178">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-178">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="59cd0-179">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="59cd0-179">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="59cd0-180">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-180">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="59cd0-181">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cd0-181">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="59cd0-182">DebugPreference가 powershell 명령줄에서 설정된 경우 디버깅 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-182">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="59cd0-183">Set-AzureRmDataLakeStoreItemAcl에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-183">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="59cd0-184">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-184">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="59cd0-185">Set-AzureRmDataLakeStoreItemAclEntry에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-185">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="59cd0-186">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="59cd0-186">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="59cd0-187">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-187">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="59cd0-188">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="59cd0-188">AzureRM.Dns</span></span>
* <span data-ttu-id="59cd0-189">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-189">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="59cd0-190">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="59cd0-190">AzureRM.EventGrid</span></span>
* <span data-ttu-id="59cd0-191">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-191">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="59cd0-192">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="59cd0-192">AzureRM.EventHub</span></span>
* <span data-ttu-id="59cd0-193">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-193">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="59cd0-194">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="59cd0-194">AzureRM.HDInsight</span></span>
* <span data-ttu-id="59cd0-195">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-195">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="59cd0-196">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="59cd0-196">AzureRM.Insights</span></span>
* <span data-ttu-id="59cd0-197">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-197">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="59cd0-198">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="59cd0-198">AzureRM.IotHub</span></span>
* <span data-ttu-id="59cd0-199">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-199">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="59cd0-200">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="59cd0-200">AzureRM.KeyVault</span></span>
* <span data-ttu-id="59cd0-201">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-201">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="59cd0-202">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="59cd0-202">AzureRM.LogicApp</span></span>
* <span data-ttu-id="59cd0-203">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-203">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="59cd0-204">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="59cd0-204">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="59cd0-205">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-205">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="59cd0-206">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="59cd0-206">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="59cd0-207">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-207">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="59cd0-208">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="59cd0-208">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="59cd0-209">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-209">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="59cd0-210">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="59cd0-210">AzureRM.Media</span></span>
* <span data-ttu-id="59cd0-211">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-211">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="59cd0-212">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="59cd0-212">AzureRM.Network</span></span>
* <span data-ttu-id="59cd0-213">Set-AzureRmLocalNetworkGateway에 대한 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-213">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="59cd0-214">Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey, New-AzureRmVirtualNetworkGatewayConnection에 대한 예제 및 설명 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-214">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="59cd0-215">Remove-AzureRmVirtualNetworkGatewayIpConfig 및 Reset-AzureRmVirtualNetworkGateway에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-215">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="59cd0-216">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-216">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="59cd0-217">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-217">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="59cd0-218">Set-AzureRmVirtualNetworkGatewayConnection에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-218">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="59cd0-219">최신 코드 생성기를 사용하여 ApplicationSecurityGroup, RouteTable 및 Usage에 대한 cmdlet을 다시 생성함</span><span class="sxs-lookup"><span data-stu-id="59cd0-219">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="59cd0-220">Exitc 하지 않는 서브넷을 얻으려고 할 때의 Get-AzureRmVirtualNetworkSubnetConfig에 대한 오류 메시지를 설명</span><span class="sxs-lookup"><span data-stu-id="59cd0-220">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="59cd0-221">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="59cd0-221">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="59cd0-222">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-222">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="59cd0-223">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="59cd0-223">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="59cd0-224">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-224">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="59cd0-225">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="59cd0-225">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="59cd0-226">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-226">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="59cd0-227">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="59cd0-227">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="59cd0-228">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-228">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="59cd0-229">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cd0-229">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="59cd0-230">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-230">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="59cd0-231">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="59cd0-231">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="59cd0-232">Get-AzureRmRecoveryServicesBackItem cmdlet에 정책 필터 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-232">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="59cd0-233">해당 명령은 지정된 정책 ID에 의해 보호되는 백업 항목의 목록을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-233">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="59cd0-234">Microsoft.Azure.Management.RecoveryServices.Backup을 버전 3.0.0-preview로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="59cd0-234">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="59cd0-235">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-235">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="59cd0-236">Restore-AzureRmRecoveryServicesBackupItem에 TargetResourceGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-236">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="59cd0-237">관리 디스크가 복원될 리소스 그룹</span><span class="sxs-lookup"><span data-stu-id="59cd0-237">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="59cd0-238">관리 디스크가 있는 VM의 백업에 적용 가능</span><span class="sxs-lookup"><span data-stu-id="59cd0-238">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="59cd0-239">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="59cd0-239">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="59cd0-240">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-240">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="59cd0-241">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="59cd0-241">AzureRM.RedisCache</span></span>
* <span data-ttu-id="59cd0-242">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-242">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="59cd0-243">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="59cd0-243">AzureRM.Relay</span></span>
* <span data-ttu-id="59cd0-244">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-244">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="59cd0-245">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="59cd0-245">AzureRM.Resources</span></span>
* <span data-ttu-id="59cd0-246">구독 범위에서 템플릿 배포를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-246">Support template deployment at subscription scope.</span></span> <span data-ttu-id="59cd0-247">새 cmdlet 추가:</span><span class="sxs-lookup"><span data-stu-id="59cd0-247">Add new Cmdlets:</span></span>
    - <span data-ttu-id="59cd0-248">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="59cd0-248">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="59cd0-249">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="59cd0-249">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="59cd0-250">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="59cd0-250">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="59cd0-251">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="59cd0-251">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="59cd0-252">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="59cd0-252">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="59cd0-253">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="59cd0-253">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="59cd0-254">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="59cd0-254">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="59cd0-255">Set-AzureRmResource에 컨텍스트를 전달할 때 오류가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-255">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="59cd0-256">New-AzureRmResourceGroupDeployment의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-256">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="59cd0-257">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-257">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="59cd0-258">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="59cd0-258">AzureRM.Scheduler</span></span>
* <span data-ttu-id="59cd0-259">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-259">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="59cd0-260">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="59cd0-260">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="59cd0-261">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-261">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="59cd0-262">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="59cd0-262">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="59cd0-263">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-263">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="59cd0-264">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="59cd0-264">AzureRM.Sql</span></span>
* <span data-ttu-id="59cd0-265">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-265">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="59cd0-266">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="59cd0-266">AzureRM.Storage</span></span>
* <span data-ttu-id="59cd0-267">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-267">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="59cd0-268">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="59cd0-268">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="59cd0-269">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-269">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="59cd0-270">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="59cd0-270">AzureRM.Tags</span></span>
* <span data-ttu-id="59cd0-271">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-271">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="59cd0-272">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="59cd0-272">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="59cd0-273">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-273">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="59cd0-274">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="59cd0-274">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="59cd0-275">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-275">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="59cd0-276">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="59cd0-276">AzureRM.Websites</span></span>
* <span data-ttu-id="59cd0-277">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-277">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="59cd0-278">6.6.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="59cd0-278">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="59cd0-279">일반</span><span class="sxs-lookup"><span data-stu-id="59cd0-279">General</span></span>
* <span data-ttu-id="59cd0-280">전체 매개 변수 형식 및 올바른 입/출력 형식을 포함하도록 모든 도움말 파일을 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-280">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="59cd0-281">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="59cd0-281">AzureRM.Profile</span></span>
* <span data-ttu-id="59cd0-282">Common.Strategy 라이브러리가 리소스에 대한 현재 구성이 대상 리소스와 호환되는지 유효성을 검사할 수 있도록 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-282">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="59cd0-283">Common.Storage에 ps1xml 형식 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-283">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="59cd0-284">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="59cd0-284">Azure.Storage</span></span>
* <span data-ttu-id="59cd0-285">DefaultProfile에서 저장소 컨텍스트를 가져오기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-285">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="59cd0-286">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-286">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="59cd0-287">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="59cd0-287">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="59cd0-288">문제 https://github.com/Azure/azure-powershell/issues/6370 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-288">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="59cd0-289">PsApiManagementApi를 ApiContract로 좌표 이동하도록 Automapper 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-289">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="59cd0-290">문제 https://github.com/Azure/azure-powershell/issues/6515 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-290">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="59cd0-291">인코딩 형식을 사용하여 오버로드하지 않도록 File.Save 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-291">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="59cd0-292">문제 https://github.com/Azure/azure-powershell/issues/6560 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-292">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="59cd0-293">apiId에서 패턴 예외를 수정하는 4.0.3 Nuget 버전으로 업그레이드됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-293">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="59cd0-294">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="59cd0-294">AzureRM.Compute</span></span>
* <span data-ttu-id="59cd0-295">PremiumLRS 저장소 계정 형식 이름 바꾸기로 인해 New-AzureRmVm에서 DiskFileParameterSet를 사용하여 vm 생성 시 실패하는 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-295">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="59cd0-296">Invoke-AzureRmVMRunCommand cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-296">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="59cd0-297">Get-AzureRmAvailabilitySet를 업데이트하여 구독에서 모든 가용성 집합 리스트를 사용하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-297">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="59cd0-298">(ResouceGroupName 매개 변수는 이제 선택적 요소입니다.)</span><span class="sxs-lookup"><span data-stu-id="59cd0-298">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="59cd0-299">vm 선별에 가속화된 네트워크를 사용하도록 'New-AzureRmVm'의 SimpleParameterSet를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-299">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="59cd0-300">New-AzureRmVmss 간단 매개 변수가 사용자 지정 LB가 이미 존재할 때 vms 생성에 실패하도록 설정하여 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-300">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="59cd0-301">New-AzureRmDisk에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-301">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="59cd0-302">'New-AzureRmVM'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-302">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="59cd0-303">Set-AzureRmVMOSDisk에 대한 설명 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-303">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="59cd0-304">Set-AzureRmVMBginfoExtension 맞춤법 및 접두사를 수정하도록 예제 1을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-304">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="59cd0-305">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="59cd0-305">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="59cd0-306">ADF.Net SDK 버전을 1.1.0으로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-306">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="59cd0-307">데이터 팩터리를 공유하는 자체 호스팅된 통합 런타임을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-307">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="59cd0-308">새 매개 변수 -SharedIntegrationRuntimeResourceId를 Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="59cd0-308">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="59cd0-309">새로운 선택적 매개 변수 -LinkedDataFactoryName을 Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="59cd0-309">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="59cd0-310">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cd0-310">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="59cd0-311">DataPlane SDK(Microsoft.Azure.DataLake.Store) 버전을 1.1.9로 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-311">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="59cd0-312">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="59cd0-312">AzureRM.EventHub</span></span>
* <span data-ttu-id="59cd0-313">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-313">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="59cd0-314">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="59cd0-314">AzureRM.Insights</span></span>
* <span data-ttu-id="59cd0-315">도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-315">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="59cd0-316">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview를 사용</span><span class="sxs-lookup"><span data-stu-id="59cd0-316">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="59cd0-317">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="59cd0-317">AzureRM.KeyVault</span></span>
* <span data-ttu-id="59cd0-318">Set-AzureRmKeyVaultAccessPolicy 내 파이핑 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-318">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="59cd0-319">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="59cd0-319">AzureRM.Network</span></span>
* <span data-ttu-id="59cd0-320">LoadBalancerInboundNatPoolConfig cmdlet에 대한 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-320">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="59cd0-321">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="59cd0-321">AzureRM.Resources</span></span>
* <span data-ttu-id="59cd0-322">'Get-AzureRmResource'에 대한 태그 이름 및 값을 제공할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-322">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="59cd0-323">'Set-AzureRmResource'를 사용하여 파이핑 시나리오 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-323">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="59cd0-324">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="59cd0-324">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="59cd0-325">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-325">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="59cd0-326">몇 가지 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-326">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="59cd0-327">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="59cd0-327">AzureRM.Sql</span></span>
* <span data-ttu-id="59cd0-328">다음 cmdlet 사용하여 서버 Advanced Threat Protection 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-328">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="59cd0-329">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="59cd0-329">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="59cd0-330">다음 cmdlet을 사용하여 취약성 평가 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-330">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="59cd0-331">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="59cd0-331">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="59cd0-332">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="59cd0-332">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="59cd0-333">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="59cd0-333">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="59cd0-334">Remove-AzureRmSqlServerFirewallRule의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-334">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="59cd0-335">Get-AzureSqlSyncGroupLog에서 미국이 아닌 문화권에서 날짜/시간을 올바르지 않게 다루는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-335">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="59cd0-336">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="59cd0-336">AzureRM.Storage</span></span>
* <span data-ttu-id="59cd0-337">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-337">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="59cd0-338">StorageAccount cmdlet 출력을 테이블 뷰로 표시</span><span class="sxs-lookup"><span data-stu-id="59cd0-338">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="59cd0-339">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cd0-339">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="59cd0-340">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cd0-340">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="59cd0-341">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cd0-341">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="59cd0-342">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="59cd0-342">AzureRM.Tags</span></span>
* <span data-ttu-id="59cd0-343">태그 cmdlet 도움말에서 잘못된 문을 제거합니다</span><span class="sxs-lookup"><span data-stu-id="59cd0-343">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="59cd0-344">6.5.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="59cd0-344">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="59cd0-345">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="59cd0-345">AzureRM.Profile</span></span>
* <span data-ttu-id="59cd0-346">'Get-AzureRmContextAutosaveSetting'에 대한 도움말이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-346">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="59cd0-347">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="59cd0-347">Azure.Storage</span></span>
* <span data-ttu-id="59cd0-348">쓰기 전용 SaS 토큰을 사용하는 Blob 또는 파일 업로드 지원</span><span class="sxs-lookup"><span data-stu-id="59cd0-348">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="59cd0-349">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="59cd0-349">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="59cd0-350">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="59cd0-350">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="59cd0-351">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="59cd0-351">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="59cd0-352">필수 속성 ResourceGroupName을 AS에 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-352">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="59cd0-353">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="59cd0-353">AzureRM.Automation</span></span>
* <span data-ttu-id="59cd0-354">도움말을 업데이트하고 'New-AzureRMAutomationSchedule'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-354">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="59cd0-355">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="59cd0-355">AzureRM.Compute</span></span>
* <span data-ttu-id="59cd0-356">-Tag 매개 변수를 Update/New-AzureRmAvailabilitySet에 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-356">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="59cd0-357">‘Add-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-357">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="59cd0-358">‘Remove-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-358">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="59cd0-359">‘Set-AzureRmVMAccessExtension’에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-359">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="59cd0-360">기본으로 SinglePlacementGroup을 false로 설정하고 단일 배치 그룹에 VMSS를 만들 수 있는 스위치 매개 변수 'SinglePlacementGroup'을 추가하도록 New-AzureRmVmss에 대한 SimpleParameterSet을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-360">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="59cd0-361">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="59cd0-361">AzureRM.EventHub</span></span>
* <span data-ttu-id="59cd0-362">PSEventHubDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="59cd0-362">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="59cd0-363">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="59cd0-363">AzureRM.KeyVault</span></span>
* <span data-ttu-id="59cd0-364">Set-AzureRmKeyVaultAccessPolicy에 대한 오류 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-364">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="59cd0-365">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="59cd0-365">AzureRM.LogicApp</span></span>
* <span data-ttu-id="59cd0-366">New-AzureRmLogicApp에서 "매개 변수 집합을 확인할 수 없습니다" 오류 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-366">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="59cd0-367">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="59cd0-367">AzureRM.Network</span></span>
* <span data-ttu-id="59cd0-368">Set/Add-AzureRmVirtualNetworkPeering에 대한 여러 테넌트의 가상 네트워크에서 피어링을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="59cd0-368">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="59cd0-369">Application Gateway에 대한 아래 cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-369">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="59cd0-370">New-AzureRmApplicationGateway: EnableFIPS 플래그 및 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-370">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="59cd0-371">New-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-371">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="59cd0-372">Set-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-372">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="59cd0-373">최신 생성기를 사용하여 RouteTable cmdlet을 재생성</span><span class="sxs-lookup"><span data-stu-id="59cd0-373">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="59cd0-374">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="59cd0-374">AzureRM.Relay</span></span>
* <span data-ttu-id="59cd0-375">markdown 파일을 업데이트하여 예제에서 매개 변수 이름 문제에 대해 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-375">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="59cd0-376">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="59cd0-376">AzureRM.Resources</span></span>
* <span data-ttu-id="59cd0-377">Roledefinition 및 Roleassignment cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-377">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="59cd0-378">페이징의 일부분으로 수행하는 추가 roledefinition 호출을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-378">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="59cd0-379">Get-AzureRmRoleAssignment cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-379">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="59cd0-380">-ExpandPrincipalGroups 명령 매개 변수 기능 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-380">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="59cd0-381">'Get-AzureRmResource'에서 '-ResourceType' 매개 변수가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-381">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="59cd0-382">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="59cd0-382">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="59cd0-383">top 및 skip 매개 변수가 cmdlet 목록을 나열하도록 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-383">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="59cd0-384">표준을 프리미엄 네임스페이스 마이그레이션 cmdlet에 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-384">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="59cd0-385">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="59cd0-385">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="59cd0-386">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="59cd0-386">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="59cd0-387">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="59cd0-387">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="59cd0-388">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="59cd0-388">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="59cd0-389">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="59cd0-389">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="59cd0-390">PSServiceBusDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="59cd0-390">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="59cd0-391">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="59cd0-391">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="59cd0-392">‘New-AzureRmServiceFabricCluster’에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-392">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="59cd0-393">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="59cd0-393">AzureRM.Sql</span></span>
* <span data-ttu-id="59cd0-394">Management.Sql에 대한 새 cmdlet을 추가하여 고객이 TDE 인증서를 SQL Server 인스턴스 또는 Managed Instance에 추가할 수 있도록 허용</span><span class="sxs-lookup"><span data-stu-id="59cd0-394">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="59cd0-395">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="59cd0-395">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="59cd0-396">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="59cd0-396">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="59cd0-397">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="59cd0-397">AzureRM.Websites</span></span>
* <span data-ttu-id="59cd0-398">`Set-AzureRmWebApp -AssignIdentity` 및 `Set-AzureRmWebAppSlot -AssignIdentity`가 false로 설정되면 사이트 개체에서 Identity 속성이 제거됩니다. 미리보기 태그도 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-398">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="59cd0-399">`Get-AzureRmWebAppMetrics`, `Get-AzureRmAppServicePlanMetrics` 예제가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-399">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="59cd0-400">`Set-AzureRmWebApp -PhpVersion`이 유효한 php 버전으로 해제 지원</span><span class="sxs-lookup"><span data-stu-id="59cd0-400">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="59cd0-401">6.4.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="59cd0-401">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="59cd0-402">일반</span><span class="sxs-lookup"><span data-stu-id="59cd0-402">General</span></span>
* <span data-ttu-id="59cd0-403">대부분의 모듈에 대한 도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-403">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="59cd0-404">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="59cd0-404">AzureRM.Profile</span></span>
* <span data-ttu-id="59cd0-405">기본 출력 형식에 추가된 Ps1Xml 특성</span><span class="sxs-lookup"><span data-stu-id="59cd0-405">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="59cd0-406">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="59cd0-406">AzureRM.Compute</span></span>
* <span data-ttu-id="59cd0-407">VMSS에 대한 IP 태그 기능</span><span class="sxs-lookup"><span data-stu-id="59cd0-407">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="59cd0-408">'New-AzureRmVmssIpTagConfig' cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-408">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="59cd0-409">New-AzureRmVmssIpConfig에 IpTag 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-409">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="59cd0-410">VMSS에 대한 자동 OS 롤백 기능</span><span class="sxs-lookup"><span data-stu-id="59cd0-410">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="59cd0-411">New-AzureRmVmssConfig 및 Update-AzureRmVmss에 DisableAutoRollback 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-411">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="59cd0-412">Vmss에 대한 OS 업그레이드 기록 기능</span><span class="sxs-lookup"><span data-stu-id="59cd0-412">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="59cd0-413">Get-AzureRmVmss에 OSUpgradeHistory 스위치 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-413">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="59cd0-414">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="59cd0-414">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="59cd0-415">다음 명령을 통해 카탈로그 액세스 제어 목록에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-415">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="59cd0-416">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="59cd0-416">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="59cd0-417">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="59cd0-417">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="59cd0-418">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="59cd0-418">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="59cd0-419">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cd0-419">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="59cd0-420">Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl에 대한 취소 지원 및 진행률 추적 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-420">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="59cd0-421">Export-AzureRmDataLakeStoreChildItemProperties에 대한 취소 지원 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-421">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="59cd0-422">재귀 작업을 수행하는 cmdlet에 대한 디버그 메시지 플러시 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-422">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="59cd0-423">DataLake cmdlet의 테스트 위치 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-423">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="59cd0-424">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="59cd0-424">AzureRM.EventHub</span></span>
* <span data-ttu-id="59cd0-425">목록 작업 cmdlet Get-AzureRmEventHub 및 Get-AzureRmEventHubConsumerGroup에 선택적 MaxCount 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-425">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="59cd0-426">새 EventHub 만드는 동안 하나 이상의 매개 변수가 필요한 New-AzureRmEventHub cmdlet 문제를 해결.</span><span class="sxs-lookup"><span data-stu-id="59cd0-426">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="59cd0-427">기본 매개 변수 집합을 제공.</span><span class="sxs-lookup"><span data-stu-id="59cd0-427">Provided Default Parameter set.</span></span>
* <span data-ttu-id="59cd0-428">선택적 매개 변수 -KeyValue를 New-AzureRmEventHubKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-428">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="59cd0-429">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="59cd0-429">AzureRM.KeyVault</span></span>
* <span data-ttu-id="59cd0-430">Get-AzureRmKeyVault -Tag 실행 시 모든 리소스가 리턴되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-430">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="59cd0-431">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="59cd0-431">AzureRM.Network</span></span>
* <span data-ttu-id="59cd0-432">영역 중복 VirtualNetworkGateways에 대한 새 Sku를 노출합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-432">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="59cd0-433">기능에 대한 새 명령이 추가됨: ARM을 통한 ExpressRoute Partner APIs</span><span class="sxs-lookup"><span data-stu-id="59cd0-433">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="59cd0-434">Get- AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-434">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="59cd0-435">Set-AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-435">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="59cd0-436">Add-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-436">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="59cd0-437">Get-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-437">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="59cd0-438">Remove-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-438">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="59cd0-439">Get-AzureRMExpressRouteCrossConnectionArpTable 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-439">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="59cd0-440">Get-AzureRMExpressRouteCrossConnectionRouteTable 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-440">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="59cd0-441">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-441">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="59cd0-442">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="59cd0-442">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="59cd0-443">Get-AzureRmRecoveryServicesBackupStatus cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-443">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="59cd0-444">이 cmdlet은 VM ID를 가져와서 VM이 구독에서 일부 자격 증명 모음으로 보호되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-444">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="59cd0-445">이러한 자격 증명 모음이 존재하는 경우 cmdlet은 자격 증명 모음 세부 정보를 출력 합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-445">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="59cd0-446">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="59cd0-446">AzureRM.Resources</span></span>
* <span data-ttu-id="59cd0-447">Get-AzureRmPolicyAssignment cmdlet을 다음과 같이 업데이트함.</span><span class="sxs-lookup"><span data-stu-id="59cd0-447">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="59cd0-448">관리 그룹 수준에서 -Scope 값 리스팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-448">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="59cd0-449">관리 그룹 수준에서 -Scope 값을 사용하여 개별 할당값을 검색하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-449">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="59cd0-450">제어 매개 변수에 -Effective 및 -All 스위치 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-450">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="59cd0-451">Get/New/Remove/Set-AzureRmPolicyDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-451">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="59cd0-452">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-452">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="59cd0-453">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-453">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="59cd0-454">Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-454">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="59cd0-455">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-455">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="59cd0-456">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-456">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="59cd0-457">'New-AzureRmResourceGroupDeployment'에서 'TemplateParameterObject'를 사용하는 경우 매개 변수에 KeyVault 비밀 참조 지원 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-457">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="59cd0-458">'New-AzureRmADAppCredential'에 대해 '-EndDate' 매개 변수가 무시되는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-458">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="59cd0-459">'Add-AzureRmADGroupMember'가 요청에 잘못된 URL을 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-459">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="59cd0-460">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="59cd0-460">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="59cd0-461">선택적 매개 변수 -KeyValue를 New-AzureRmServiceBusKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-461">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="59cd0-462">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="59cd0-462">AzureRM.Sql</span></span>
* <span data-ttu-id="59cd0-463">New-AzureRmSqlDatabaseRestorePoint 도움말에서 SQLDW에 대한 사용자 정의 복원 지점 명시</span><span class="sxs-lookup"><span data-stu-id="59cd0-463">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="59cd0-464">몇 가지 cmdlet에서-ComputeGeneration 매개 변수의 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-464">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="59cd0-465">6.3.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="59cd0-465">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="59cd0-466">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="59cd0-466">AzureRM.Profile</span></span>
* <span data-ttu-id="59cd0-467">Enable-AzureRmContextAutoSave에 대한 오류 메시지 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-467">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="59cd0-468">이전 컨텍스트 없이 'Connect-AzureRmAccount' 실행 시 각 구독에 대한 컨텍스트 생성</span><span class="sxs-lookup"><span data-stu-id="59cd0-468">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="59cd0-469">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="59cd0-469">Azure.Storage</span></span>
* <span data-ttu-id="59cd0-470">도움말 파일 내 -Permissions 매개 변수에 대한 추가 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-470">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="59cd0-471">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="59cd0-471">AzureRM.Compute</span></span>
* <span data-ttu-id="59cd0-472">'Get-AzureRmVmDiskEncryptionStatus'가 데이터 디스크가 없는 VM에 대해 관찰된 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-472">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="59cd0-473">Compute 클라이언트 라이브러리 버전을 업데이트하여 다음 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-473">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="59cd0-474">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="59cd0-474">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="59cd0-475">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="59cd0-475">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="59cd0-476">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="59cd0-476">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="59cd0-477">다음 cmdlet이 '작업 ID' 및 '작업 상태'를 올바르게 표시하도록 수정:</span><span class="sxs-lookup"><span data-stu-id="59cd0-477">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="59cd0-478">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="59cd0-478">Start-AzureRmVM</span></span>
    - <span data-ttu-id="59cd0-479">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="59cd0-479">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="59cd0-480">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="59cd0-480">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="59cd0-481">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="59cd0-481">Set-AzureRmVM</span></span>
    - <span data-ttu-id="59cd0-482">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="59cd0-482">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="59cd0-483">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="59cd0-483">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="59cd0-484">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="59cd0-484">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="59cd0-485">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="59cd0-485">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="59cd0-486">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="59cd0-486">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="59cd0-487">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="59cd0-487">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="59cd0-488">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="59cd0-488">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="59cd0-489">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="59cd0-489">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="59cd0-490">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="59cd0-490">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="59cd0-491">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="59cd0-491">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="59cd0-492">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="59cd0-492">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="59cd0-493">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="59cd0-493">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="59cd0-494">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="59cd0-494">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="59cd0-495">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="59cd0-495">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="59cd0-496">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="59cd0-496">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="59cd0-497">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="59cd0-497">AzureRM.EventGrid</span></span>
* <span data-ttu-id="59cd0-498">Update-AzureRmEventGridSubscription cmdlet의 SubjectBeginsWith/SubjectEndsWith에 대한 ValidateNotNullOrEmpty 유효성 검사 조건을 제거하여 필요에 따라 이러한 매개 변수를 빈 문자열로 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-498">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="59cd0-499">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="59cd0-499">AzureRM.KeyVault</span></span>
* <span data-ttu-id="59cd0-500">Get-AzureRmKeyVault -Tag 실행 시 태그가 리턴되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-500">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="59cd0-501">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="59cd0-501">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="59cd0-502">Policy Insights cmdlet의 공개 릴리스</span><span class="sxs-lookup"><span data-stu-id="59cd0-502">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="59cd0-503">API 버전 2018-04-04 사용</span><span class="sxs-lookup"><span data-stu-id="59cd0-503">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="59cd0-504">PolicyDefinitionReferenceId를 Get-AzureRmPolicyStateSummary의 결과 집합에 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-504">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="59cd0-505">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="59cd0-505">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="59cd0-506">-Vault 매개 변수를 RecoveryServices.Backup cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="59cd0-506">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="59cd0-507">전달되는 경우 이는 Set-AzureRmRecoveryServicesContext cmdlet을 재정의함.</span><span class="sxs-lookup"><span data-stu-id="59cd0-507">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="59cd0-508">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="59cd0-508">AzureRM.Sql</span></span>
* <span data-ttu-id="59cd0-509">Get-AzureRmSqlDatabaseExpanded에 대한 도움말 파일의 예가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-509">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="59cd0-510">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="59cd0-510">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="59cd0-511">Add-AzureRmTrafficManagerEndpointConfig에대한 도움말 파일이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-511">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="59cd0-512">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="59cd0-512">AzureRM.Websites</span></span>
* <span data-ttu-id="59cd0-513">-AssignIdentity를 사용할 때 AppSetting을 덮어쓰지 않도록 'Set-AzureRmWebApp'이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-513">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="59cd0-514">'New-AzureRmWebAppSlot'이 AppServicePlan을 옵션 매개변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-514">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="59cd0-515">6.2.1 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="59cd0-515">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="59cd0-516">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="59cd0-516">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="59cd0-517">PSWorkspace 모델이 Network 형식을 매개 변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-517">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="59cd0-518">6.2.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="59cd0-518">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="59cd0-519">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="59cd0-519">AzureRM.Profile</span></span>
* <span data-ttu-id="59cd0-520">Newtonsoft.Json의 버전 10.0.3이 모듈 가져오기에 로드되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-520">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="59cd0-521">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="59cd0-521">AzureRM.Compute</span></span>
* <span data-ttu-id="59cd0-522">VMSS VM 업데이트 기능</span><span class="sxs-lookup"><span data-stu-id="59cd0-522">VMSS VM Update feature</span></span>
    - <span data-ttu-id="59cd0-523">'Update-AzureRmVmssVM' 및 'New-AzureRmVMDataDisk' cmdlets 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-523">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="59cd0-524">데이터 디스크를 Vmss VM에 추가할 수 있도록 지원하기 위해 VirtualMachineScaleSetVM 매개변수를 'Add-AzureRmVMDataDisk' cmdlet에 추가하였습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-524">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="59cd0-525">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="59cd0-525">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="59cd0-526">ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.8.0-preview로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-526">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="59cd0-527">팩터리 리포지토리 작업 구성 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-527">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="59cd0-528">QuickBooks LinkedService가 ConsumerKey 및 consumerSecret 속성을 노출하도록 업데이트됨 </span><span class="sxs-lookup"><span data-stu-id="59cd0-528">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="59cd0-529">여러 모델 유형을 SecretBase에서 개체로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="59cd0-529">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="59cd0-530">Blob 이벤트 트리거 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-530">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="59cd0-531">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="59cd0-531">AzureRM.KeyVault</span></span>
* <span data-ttu-id="59cd0-532">예제 출력으로 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-532">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="59cd0-533">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="59cd0-533">AzureRM.Network</span></span>
* <span data-ttu-id="59cd0-534">Network Watcher cmdlet에서 트래픽 분석 매개 변수를 사용가능하도록 설정</span><span class="sxs-lookup"><span data-stu-id="59cd0-534">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="59cd0-535">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="59cd0-535">AzureRM.Resources</span></span>
* <span data-ttu-id="59cd0-536">'Get AzureRmResource'에서 반환된 'PSResource' 개체의 'Properties' 속성의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-536">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="59cd0-537">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="59cd0-537">AzureRM.Scheduler</span></span>
* <span data-ttu-id="59cd0-538">ServiceBusQueueJob 업데이트가 새 인증 값을 설정하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="59cd0-538">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="59cd0-539">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="59cd0-539">AzureRM.Sql</span></span>
* <span data-ttu-id="59cd0-540">옵션 LicenseType 매개 변수를 사용하여 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="59cd0-540">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="59cd0-541">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="59cd0-541">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="59cd0-542">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="59cd0-542">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="59cd0-543">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="59cd0-543">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="59cd0-544">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="59cd0-544">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="59cd0-545">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="59cd0-545">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="59cd0-546">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="59cd0-546">AzureRM.Websites</span></span>
* <span data-ttu-id="59cd0-547">'New-AzureRMWebApp'이 전략 라이브러리의 공통 알고리즘을 사용하도록 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-547">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="59cd0-548">6.1.0 - 2018년 5월</span><span class="sxs-lookup"><span data-stu-id="59cd0-548">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="59cd0-549">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="59cd0-549">AzureRM.Profile</span></span>
* <span data-ttu-id="59cd0-550">'Clear-AzureRmContext'를 실행하면 이전 기본 컨텍스트의 이름으로 빈 컨텍스트가 유지되어 사용자가 이전 이름으로 새 컨텍스트를 만들지 못하게 되는 문제를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-550">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="59cd0-551">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="59cd0-551">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="59cd0-552">AS에서 게이트웨이가 작업을 연결하거나 연결 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-552">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="59cd0-553">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="59cd0-553">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="59cd0-554">ApiVersions, ApiReleases 및 ApiRevisions에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-554">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="59cd0-555">ServiceFabric 백 엔드에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-555">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="59cd0-556">Application Insights 로거에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-556">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="59cd0-557">'기본' SKU를 API Management 서비스의 유효한 SKU로 인식하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-557">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="59cd0-558">개인 CA가 발급한 인증서를 루트 또는 CA로 설치하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-558">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="59cd0-559">KeyVault 및 다중 프록시 호스트 이름을 통한 사용자 정의 SSL 인증서를 수락하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-559">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="59cd0-560">MSI ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="59cd0-560">Added support for MSI identity</span></span>
* <span data-ttu-id="59cd0-561">URL을 통한 정책을 수락하는 지원 추가됨 참고: 다음 cmdlet은 이후 릴리스에서 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-561">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="59cd0-562">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="59cd0-562">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="59cd0-563">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="59cd0-563">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="59cd0-564">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="59cd0-564">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="59cd0-565">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="59cd0-565">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="59cd0-566">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="59cd0-566">AzureRM.Batch</span></span>
* <span data-ttu-id="59cd0-567">새 cmdlet Get AzureBatchPoolNodeCounts 릴리스</span><span class="sxs-lookup"><span data-stu-id="59cd0-567">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="59cd0-568">새 cmdlet Start-AzureBatchComputeNodeServiceLogUpload 릴리스</span><span class="sxs-lookup"><span data-stu-id="59cd0-568">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="59cd0-569">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="59cd0-569">AzureRM.Consumption</span></span>
* <span data-ttu-id="59cd0-570">Expand, ResourceGroup, InstanceName, InstanceId, Tags, Top on Cmdlet Get-AzureRmConsumptionUsageDetail 등 새 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="59cd0-570">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="59cd0-571">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cd0-571">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="59cd0-572">Export-AzureRmDataLakeStoreChildItemProperties에 대한 예제 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-572">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="59cd0-573">Set-AzureRmDataLakeStoreItemAclEntry에서 재귀 사례에 대한 null 매개 변수 예외 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-573">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="59cd0-574">Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry에 대한 도움말 파일 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-574">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="59cd0-575">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="59cd0-575">AzureRM.Network</span></span>
* <span data-ttu-id="59cd0-576">18.0.0-preview에서 19.0.0-preview로 네트워크 SDK 버전 업그레이드</span><span class="sxs-lookup"><span data-stu-id="59cd0-576">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="59cd0-577">프로토콜 구성을 만들기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="59cd0-577">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="59cd0-578">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="59cd0-578">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="59cd0-579">기존 Express 경로 회로에 새 회로 연결을 추가하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="59cd0-579">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="59cd0-580">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="59cd0-580">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="59cd0-581">기존 Express 경로 회로에서 회로 연결을 제거하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="59cd0-581">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="59cd0-582">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="59cd0-582">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="59cd0-583">회로 연결을 검색하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="59cd0-583">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="59cd0-584">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="59cd0-584">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="59cd0-585">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="59cd0-585">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="59cd0-586">생성된 인증서로 고정 서버 인증 사용(문제 # 5998)</span><span class="sxs-lookup"><span data-stu-id="59cd0-586">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="59cd0-587">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="59cd0-587">AzureRM.Sql</span></span>
* <span data-ttu-id="59cd0-588">AuditActions 또는 AuditActionGroups를 제거할 수 있도록 업데이트된 감사 cmdlet</span><span class="sxs-lookup"><span data-stu-id="59cd0-588">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="59cd0-589">'Azure 복구 서비스 자격 증명 모음을 사용하여 장기 보존 정책을 구성하면 정책이 더 이상 지원되지 않습니다. 새로운 유연 보유 정책으로 요청을 제출하십시오.'라는 메시지와 함께 명령이 실패하는 새로운 유연 보유 정책을 설정할 때</span><span class="sxs-lookup"><span data-stu-id="59cd0-589">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="59cd0-590">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy의 문제 수정</span><span class="sxs-lookup"><span data-stu-id="59cd0-590">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="59cd0-591">Azure SQL Database/ElasticPool Creation/Update 관련 cmdlet을 모두 업데이트하여 규모 및 계층 관련 속성에 대한 SKU 속성을 지원하는 새 데이터베이스 API를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-591">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="59cd0-592">업데이트된 cmdlet는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-592">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="59cd0-593">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="59cd0-593">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="59cd0-594">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="59cd0-594">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="59cd0-595">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="59cd0-595">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="59cd0-596">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="59cd0-596">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="59cd0-597">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="59cd0-597">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="59cd0-598">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="59cd0-598">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="59cd0-599">-Name 매개 변수를 사용할 때 -ResourceGroupName 매개 변수가 필요하도록 'Get-AzureRmTrafficManagerProfile'에 대한 매개 변수를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="59cd0-599">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
