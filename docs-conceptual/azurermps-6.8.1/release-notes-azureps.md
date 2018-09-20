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
ms.openlocfilehash: f4f3141998be14f0b5b223aed1af283534bf061d
ms.sourcegitcommit: bc88e64c494337821274d6a66c1edad656c119c5
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/20/2018
ms.locfileid: "46300836"
---
# <a name="release-notes"></a><span data-ttu-id="ac49b-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="ac49b-103">Release notes</span></span>

<span data-ttu-id="ac49b-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="681---august-2018"></a><span data-ttu-id="ac49b-105">6.8.1 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="ac49b-105">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="ac49b-106">일반</span><span class="sxs-lookup"><span data-stu-id="ac49b-106">General</span></span>
* <span data-ttu-id="ac49b-107">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-107">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="ac49b-108">공용 런타임 어셈블리가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-108">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="ac49b-109">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ac49b-109">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="ac49b-110">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-110">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="ac49b-111">문제 https://github.com/Azure/azure-powershell/issues/6603 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-111">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="ac49b-112">Import-AzureRmApiManagementApi 및 \*-AzureRmApiManagementCertificate cmdlet은 이제 상대 경로를 처리합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-112">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="ac49b-113">문제 https://github.com/Azure/azure-powershell/issues/6879 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-113">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="ac49b-114">CertificateInformation은 Set-AzureRmApiManagement cmdlet이 제대로 작동 하게 하는 설정 가능한 속성입니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-114">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="ac49b-115">4.0.4-preview nuget으로 업그레이드하여 해결됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-115">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="ac49b-116">문제 https://github.com/Azure/azure-powershell/issues/6853 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-116">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="ac49b-117">제품에서 이름별 검색에 대해 Odata 필터가 수정됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-117">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="ac49b-118">문제 https://github.com/Azure/azure-powershell/issues/6814 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-118">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="ac49b-119">API에서 이름별 검색에 대해 Odata 필터가 수정됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-119">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="ac49b-120">AzureMonitor 로거에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-120">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="ac49b-121">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="ac49b-121">AzureRM.Compute</span></span>
* <span data-ttu-id="ac49b-122">오류 출력에 대상이 없는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-122">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="ac49b-123">관리 디스크를 사용하는 VM에 대한 저장소 계정 유형 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-123">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="ac49b-124">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-124">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="ac49b-125">예를 들어 Azure 중국과 같이, 다른 환경에 대한 AEM 확장 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-125">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="ac49b-126">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="ac49b-126">AzureRM.Network</span></span>
* <span data-ttu-id="ac49b-127">기본 cmdlet 출력 표시를 테이블 뷰로 변경</span><span class="sxs-lookup"><span data-stu-id="ac49b-127">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="ac49b-128">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="ac49b-128">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="ac49b-129">일시 중지된 용량을 확장하려고 할 때 Update-AzureRmPowerBIEmbeddedCapacity 실패 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-129">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="ac49b-130">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="ac49b-130">AzureRM.Resources</span></span>
* <span data-ttu-id="ac49b-131">MarketPlace에서 관리되는 응용 프로그램 생성 시의 문제 해결.</span><span class="sxs-lookup"><span data-stu-id="ac49b-131">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="ac49b-132">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ac49b-132">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="ac49b-133">해결된 문제</span><span class="sxs-lookup"><span data-stu-id="ac49b-133">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="ac49b-134">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ac49b-134">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="ac49b-135">다중값 라우팅 메서드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-135">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="ac49b-136">다중값 라우팅에 대한 새 매개 변수 'MaxReturn'</span><span class="sxs-lookup"><span data-stu-id="ac49b-136">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="ac49b-137">서브넷 라우팅 메서드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-137">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="ac49b-138">엔드포인트의 IP 주소 범위(서브넷)에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="ac49b-138">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="ac49b-139">프로필 내 사용자 지정 헤더에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-139">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="ac49b-140">프로필 내 예상 상태 코드 범위에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-140">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="ac49b-141">엔드포인트 내 사용자 지정 헤더에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-141">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="ac49b-142">6.8.0 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="ac49b-142">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="ac49b-143">일반</span><span class="sxs-lookup"><span data-stu-id="ac49b-143">General</span></span>
* <span data-ttu-id="ac49b-144">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-144">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="ac49b-145">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="ac49b-145">AzureRM.Profile</span></span>
* <span data-ttu-id="ac49b-146">Connect-AzureRmAccount 중에 반환된 토큰에 만료 속성 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-146">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="ac49b-147">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="ac49b-147">AzureRM.Compute</span></span>
* <span data-ttu-id="ac49b-148">오류 출력에 대상이 없는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-148">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="ac49b-149">관리 디스크를 사용하는 VM에 대한 저장소 계정 유형 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-149">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="ac49b-150">예를 들어 Azure 중국과 같이, 다른 환경에 대한 AEM 확장 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-150">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="ac49b-151">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="ac49b-151">AzureRM.IotHub</span></span>
* <span data-ttu-id="ac49b-152">New-AzureRmIotHubExportDevices 및 New-AzureRmIotHubImportDevices에 대한 예제를 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-152">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="ac49b-153">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="ac49b-153">AzureRM.Network</span></span>
* <span data-ttu-id="ac49b-154">기본 모델 표시를 테이블 뷰로 변경</span><span class="sxs-lookup"><span data-stu-id="ac49b-154">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="ac49b-155">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="ac49b-155">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="ac49b-156">일시 중지된 용량을 확장하려고 할 때 Update-AzureRmPowerBIEmbeddedCapacity 실패 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-156">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="ac49b-157">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="ac49b-157">AzureRM.Resources</span></span>
* <span data-ttu-id="ac49b-158">MarketPlace에서 관리되는 응용 프로그램 생성 시의 문제 해결.</span><span class="sxs-lookup"><span data-stu-id="ac49b-158">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="ac49b-159">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ac49b-159">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="ac49b-160">문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-160">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="ac49b-161">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ac49b-161">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="ac49b-162">다중값 라우팅 메서드에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="ac49b-162">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="ac49b-163">다중값 라우팅에 대한 새 매개 변수 'MaxReturn'</span><span class="sxs-lookup"><span data-stu-id="ac49b-163">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="ac49b-164">서브넷 라우팅 메서드에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="ac49b-164">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="ac49b-165">엔드포인트의 IP 주소 범위(서브넷)에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="ac49b-165">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="ac49b-166">프로필 내 사용자 지정 헤더에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="ac49b-166">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="ac49b-167">프로필 내 예상 상태 코드 범위에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="ac49b-167">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="ac49b-168">엔드포인트 내 사용자 지정 헤더에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="ac49b-168">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="ac49b-169">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="ac49b-169">AzureRM.Websites</span></span>
* <span data-ttu-id="ac49b-170">기본 리소스 그룹이 잘못 설정되는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-170">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="ac49b-171">6.7.0 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="ac49b-171">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="ac49b-172">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="ac49b-172">AzureRM.Profile</span></span>
* <span data-ttu-id="ac49b-173">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-173">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="ac49b-174">충돌을 방지하려면 기본 컨텍스트 이름으로 사용자 ID를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-174">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="ac49b-175">#6398 컨텍스트를 선택할 때 문제를 발생시킨 Clear-AzureRmContext 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-175">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="ac49b-176">'Connect-AzureRmAccount'에 대한 '-TenantId' 매개 변수에 전달할 테넌트 도메인을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="ac49b-176">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="ac49b-177">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="ac49b-177">Azure.Storage</span></span>
* <span data-ttu-id="ac49b-178">Azure 파일 공유 할당량에 대한 5TB 제한 제거</span><span class="sxs-lookup"><span data-stu-id="ac49b-178">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="ac49b-179">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="ac49b-179">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="ac49b-180">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ac49b-180">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="ac49b-181">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-181">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="ac49b-182">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ac49b-182">Azure.AnalysisServices</span></span>
* <span data-ttu-id="ac49b-183">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-183">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="ac49b-184">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ac49b-184">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="ac49b-185">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-185">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="ac49b-186">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="ac49b-186">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="ac49b-187">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-187">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="ac49b-188">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="ac49b-188">AzureRM.Automation</span></span>
* <span data-ttu-id="ac49b-189">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-189">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="ac49b-190">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="ac49b-190">AzureRM.Backup</span></span>
* <span data-ttu-id="ac49b-191">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-191">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="ac49b-192">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="ac49b-192">AzureRM.Batch</span></span>
* <span data-ttu-id="ac49b-193">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-193">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="ac49b-194">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="ac49b-194">AzureRM.Billing</span></span>
* <span data-ttu-id="ac49b-195">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-195">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="ac49b-196">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="ac49b-196">AzureRM.Cdn</span></span>
* <span data-ttu-id="ac49b-197">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-197">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="ac49b-198">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ac49b-198">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="ac49b-199">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-199">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="ac49b-200">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="ac49b-200">AzureRM.Compute</span></span>
* <span data-ttu-id="ac49b-201">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-201">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="ac49b-202">New-AzureRmVmssConfig에 EvictionPolicy 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-202">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="ac49b-203">지정된 위치가 없는 경우에 New-AzureRmVm의 DiskFileParameterSet 내의 기본 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-203">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="ac49b-204">Save-AzureRmVMImage에서 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-204">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="ac49b-205">특정 singlepass 관련 시나리오에 대해 Get-AzureRmVMDiskEncryptionStatus cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-205">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="ac49b-206">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="ac49b-206">AzureRM.Consumption</span></span>
* <span data-ttu-id="ac49b-207">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-207">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="ac49b-208">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="ac49b-208">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="ac49b-209">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-209">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="ac49b-210">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="ac49b-210">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="ac49b-211">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-211">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="ac49b-212">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="ac49b-212">AzureRM.DataFactories</span></span>
* <span data-ttu-id="ac49b-213">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-213">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="ac49b-214">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="ac49b-214">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="ac49b-215">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-215">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="ac49b-216">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="ac49b-216">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="ac49b-217">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-217">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="ac49b-218">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ac49b-218">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="ac49b-219">DebugPreference가 powershell 명령줄에서 설정된 경우 디버깅 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-219">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="ac49b-220">Set-AzureRmDataLakeStoreItemAcl에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-220">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="ac49b-221">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-221">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="ac49b-222">Set-AzureRmDataLakeStoreItemAclEntry에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-222">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="ac49b-223">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="ac49b-223">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="ac49b-224">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-224">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="ac49b-225">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="ac49b-225">AzureRM.Dns</span></span>
* <span data-ttu-id="ac49b-226">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-226">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="ac49b-227">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ac49b-227">AzureRM.EventGrid</span></span>
* <span data-ttu-id="ac49b-228">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-228">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="ac49b-229">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="ac49b-229">AzureRM.EventHub</span></span>
* <span data-ttu-id="ac49b-230">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-230">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="ac49b-231">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="ac49b-231">AzureRM.HDInsight</span></span>
* <span data-ttu-id="ac49b-232">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-232">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="ac49b-233">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="ac49b-233">AzureRM.Insights</span></span>
* <span data-ttu-id="ac49b-234">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-234">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="ac49b-235">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="ac49b-235">AzureRM.IotHub</span></span>
* <span data-ttu-id="ac49b-236">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-236">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="ac49b-237">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ac49b-237">AzureRM.KeyVault</span></span>
* <span data-ttu-id="ac49b-238">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-238">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="ac49b-239">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ac49b-239">AzureRM.LogicApp</span></span>
* <span data-ttu-id="ac49b-240">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-240">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="ac49b-241">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="ac49b-241">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="ac49b-242">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-242">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="ac49b-243">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="ac49b-243">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="ac49b-244">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-244">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="ac49b-245">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="ac49b-245">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="ac49b-246">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-246">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="ac49b-247">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="ac49b-247">AzureRM.Media</span></span>
* <span data-ttu-id="ac49b-248">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-248">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="ac49b-249">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="ac49b-249">AzureRM.Network</span></span>
* <span data-ttu-id="ac49b-250">Set-AzureRmLocalNetworkGateway에 대한 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-250">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="ac49b-251">Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey, New-AzureRmVirtualNetworkGatewayConnection에 대한 예제 및 설명 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-251">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="ac49b-252">Remove-AzureRmVirtualNetworkGatewayIpConfig 및 Reset-AzureRmVirtualNetworkGateway에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-252">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="ac49b-253">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-253">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="ac49b-254">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-254">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="ac49b-255">Set-AzureRmVirtualNetworkGatewayConnection에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-255">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="ac49b-256">최신 코드 생성기를 사용하여 ApplicationSecurityGroup, RouteTable 및 Usage에 대한 cmdlet을 다시 생성함</span><span class="sxs-lookup"><span data-stu-id="ac49b-256">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="ac49b-257">Exitc 하지 않는 서브넷을 얻으려고 할 때의 Get-AzureRmVirtualNetworkSubnetConfig에 대한 오류 메시지를 설명</span><span class="sxs-lookup"><span data-stu-id="ac49b-257">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="ac49b-258">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="ac49b-258">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="ac49b-259">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-259">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="ac49b-260">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ac49b-260">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="ac49b-261">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-261">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="ac49b-262">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ac49b-262">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="ac49b-263">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-263">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="ac49b-264">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="ac49b-264">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="ac49b-265">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-265">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="ac49b-266">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ac49b-266">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="ac49b-267">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-267">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="ac49b-268">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="ac49b-268">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="ac49b-269">Get-AzureRmRecoveryServicesBackItem cmdlet에 정책 필터 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-269">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="ac49b-270">해당 명령은 지정된 정책 ID에 의해 보호되는 백업 항목의 목록을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-270">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="ac49b-271">Microsoft.Azure.Management.RecoveryServices.Backup을 버전 3.0.0-preview로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="ac49b-271">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="ac49b-272">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-272">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="ac49b-273">Restore-AzureRmRecoveryServicesBackupItem에 TargetResourceGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-273">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="ac49b-274">관리 디스크가 복원될 리소스 그룹</span><span class="sxs-lookup"><span data-stu-id="ac49b-274">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="ac49b-275">관리 디스크가 있는 VM의 백업에 적용 가능</span><span class="sxs-lookup"><span data-stu-id="ac49b-275">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="ac49b-276">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="ac49b-276">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="ac49b-277">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-277">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="ac49b-278">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="ac49b-278">AzureRM.RedisCache</span></span>
* <span data-ttu-id="ac49b-279">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-279">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="ac49b-280">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="ac49b-280">AzureRM.Relay</span></span>
* <span data-ttu-id="ac49b-281">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-281">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="ac49b-282">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="ac49b-282">AzureRM.Resources</span></span>
* <span data-ttu-id="ac49b-283">구독 범위에서 템플릿 배포를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-283">Support template deployment at subscription scope.</span></span> <span data-ttu-id="ac49b-284">새 cmdlet 추가:</span><span class="sxs-lookup"><span data-stu-id="ac49b-284">Add new Cmdlets:</span></span>
    - <span data-ttu-id="ac49b-285">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="ac49b-285">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="ac49b-286">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="ac49b-286">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="ac49b-287">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="ac49b-287">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="ac49b-288">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="ac49b-288">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="ac49b-289">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="ac49b-289">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="ac49b-290">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="ac49b-290">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="ac49b-291">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="ac49b-291">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="ac49b-292">Set-AzureRmResource에 컨텍스트를 전달할 때 오류가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-292">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="ac49b-293">New-AzureRmResourceGroupDeployment의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-293">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="ac49b-294">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-294">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="ac49b-295">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="ac49b-295">AzureRM.Scheduler</span></span>
* <span data-ttu-id="ac49b-296">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-296">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="ac49b-297">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ac49b-297">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="ac49b-298">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-298">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="ac49b-299">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ac49b-299">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="ac49b-300">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-300">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="ac49b-301">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="ac49b-301">AzureRM.Sql</span></span>
* <span data-ttu-id="ac49b-302">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-302">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="ac49b-303">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="ac49b-303">AzureRM.Storage</span></span>
* <span data-ttu-id="ac49b-304">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-304">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="ac49b-305">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="ac49b-305">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="ac49b-306">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-306">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="ac49b-307">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="ac49b-307">AzureRM.Tags</span></span>
* <span data-ttu-id="ac49b-308">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-308">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="ac49b-309">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ac49b-309">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="ac49b-310">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-310">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="ac49b-311">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="ac49b-311">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="ac49b-312">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-312">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="ac49b-313">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="ac49b-313">AzureRM.Websites</span></span>
* <span data-ttu-id="ac49b-314">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-314">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="ac49b-315">6.6.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="ac49b-315">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="ac49b-316">일반</span><span class="sxs-lookup"><span data-stu-id="ac49b-316">General</span></span>
* <span data-ttu-id="ac49b-317">전체 매개 변수 형식 및 올바른 입/출력 형식을 포함하도록 모든 도움말 파일을 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-317">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="ac49b-318">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="ac49b-318">AzureRM.Profile</span></span>
* <span data-ttu-id="ac49b-319">Common.Strategy 라이브러리가 리소스에 대한 현재 구성이 대상 리소스와 호환되는지 유효성을 검사할 수 있도록 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-319">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="ac49b-320">Common.Storage에 ps1xml 형식 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-320">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="ac49b-321">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="ac49b-321">Azure.Storage</span></span>
* <span data-ttu-id="ac49b-322">DefaultProfile에서 저장소 컨텍스트를 가져오기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-322">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="ac49b-323">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-323">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="ac49b-324">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ac49b-324">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="ac49b-325">문제 https://github.com/Azure/azure-powershell/issues/6370 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-325">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="ac49b-326">PsApiManagementApi를 ApiContract로 좌표 이동하도록 Automapper 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-326">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="ac49b-327">문제 https://github.com/Azure/azure-powershell/issues/6515 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-327">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="ac49b-328">인코딩 형식을 사용하여 오버로드하지 않도록 File.Save 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-328">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="ac49b-329">문제 https://github.com/Azure/azure-powershell/issues/6560 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-329">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="ac49b-330">apiId에서 패턴 예외를 수정하는 4.0.3 Nuget 버전으로 업그레이드됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-330">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="ac49b-331">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="ac49b-331">AzureRM.Compute</span></span>
* <span data-ttu-id="ac49b-332">PremiumLRS 저장소 계정 형식 이름 바꾸기로 인해 New-AzureRmVm에서 DiskFileParameterSet를 사용하여 vm 생성 시 실패하는 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-332">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="ac49b-333">Invoke-AzureRmVMRunCommand cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-333">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="ac49b-334">Get-AzureRmAvailabilitySet를 업데이트하여 구독에서 모든 가용성 집합 리스트를 사용하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-334">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="ac49b-335">(ResouceGroupName 매개 변수는 이제 선택적 요소입니다.)</span><span class="sxs-lookup"><span data-stu-id="ac49b-335">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="ac49b-336">vm 선별에 가속화된 네트워크를 사용하도록 'New-AzureRmVm'의 SimpleParameterSet를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-336">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="ac49b-337">New-AzureRmVmss 간단 매개 변수가 사용자 지정 LB가 이미 존재할 때 vms 생성에 실패하도록 설정하여 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-337">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="ac49b-338">New-AzureRmDisk에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-338">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="ac49b-339">'New-AzureRmVM'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-339">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="ac49b-340">Set-AzureRmVMOSDisk에 대한 설명 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-340">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="ac49b-341">Set-AzureRmVMBginfoExtension 맞춤법 및 접두사를 수정하도록 예제 1을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-341">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="ac49b-342">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="ac49b-342">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="ac49b-343">ADF.Net SDK 버전을 1.1.0으로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-343">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="ac49b-344">데이터 팩터리를 공유하는 자체 호스팅된 통합 런타임을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-344">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="ac49b-345">새 매개 변수 -SharedIntegrationRuntimeResourceId를 Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="ac49b-345">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="ac49b-346">새로운 선택적 매개 변수 -LinkedDataFactoryName을 Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="ac49b-346">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="ac49b-347">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ac49b-347">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="ac49b-348">DataPlane SDK(Microsoft.Azure.DataLake.Store) 버전을 1.1.9로 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-348">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="ac49b-349">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="ac49b-349">AzureRM.EventHub</span></span>
* <span data-ttu-id="ac49b-350">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-350">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="ac49b-351">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="ac49b-351">AzureRM.Insights</span></span>
* <span data-ttu-id="ac49b-352">도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-352">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="ac49b-353">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview를 사용</span><span class="sxs-lookup"><span data-stu-id="ac49b-353">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="ac49b-354">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ac49b-354">AzureRM.KeyVault</span></span>
* <span data-ttu-id="ac49b-355">Set-AzureRmKeyVaultAccessPolicy 내 파이핑 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-355">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="ac49b-356">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="ac49b-356">AzureRM.Network</span></span>
* <span data-ttu-id="ac49b-357">LoadBalancerInboundNatPoolConfig cmdlet에 대한 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-357">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="ac49b-358">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="ac49b-358">AzureRM.Resources</span></span>
* <span data-ttu-id="ac49b-359">'Get-AzureRmResource'에 대한 태그 이름 및 값을 제공할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-359">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="ac49b-360">'Set-AzureRmResource'를 사용하여 파이핑 시나리오 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-360">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="ac49b-361">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ac49b-361">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="ac49b-362">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-362">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="ac49b-363">몇 가지 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-363">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="ac49b-364">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="ac49b-364">AzureRM.Sql</span></span>
* <span data-ttu-id="ac49b-365">다음 cmdlet 사용하여 서버 Advanced Threat Protection 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-365">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="ac49b-366">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="ac49b-366">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="ac49b-367">다음 cmdlet을 사용하여 취약성 평가 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-367">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="ac49b-368">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="ac49b-368">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="ac49b-369">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="ac49b-369">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="ac49b-370">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="ac49b-370">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="ac49b-371">Remove-AzureRmSqlServerFirewallRule의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-371">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="ac49b-372">Get-AzureSqlSyncGroupLog에서 미국이 아닌 문화권에서 날짜/시간을 올바르지 않게 다루는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-372">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="ac49b-373">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="ac49b-373">AzureRM.Storage</span></span>
* <span data-ttu-id="ac49b-374">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-374">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="ac49b-375">StorageAccount cmdlet 출력을 테이블 뷰로 표시</span><span class="sxs-lookup"><span data-stu-id="ac49b-375">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="ac49b-376">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ac49b-376">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="ac49b-377">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ac49b-377">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="ac49b-378">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ac49b-378">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="ac49b-379">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="ac49b-379">AzureRM.Tags</span></span>
* <span data-ttu-id="ac49b-380">태그 cmdlet 도움말에서 잘못된 문을 제거합니다</span><span class="sxs-lookup"><span data-stu-id="ac49b-380">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="ac49b-381">6.5.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="ac49b-381">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="ac49b-382">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="ac49b-382">AzureRM.Profile</span></span>
* <span data-ttu-id="ac49b-383">'Get-AzureRmContextAutosaveSetting'에 대한 도움말이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-383">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="ac49b-384">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="ac49b-384">Azure.Storage</span></span>
* <span data-ttu-id="ac49b-385">쓰기 전용 SaS 토큰을 사용하는 Blob 또는 파일 업로드 지원</span><span class="sxs-lookup"><span data-stu-id="ac49b-385">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="ac49b-386">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ac49b-386">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="ac49b-387">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ac49b-387">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="ac49b-388">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ac49b-388">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="ac49b-389">필수 속성 ResourceGroupName을 AS에 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-389">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="ac49b-390">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="ac49b-390">AzureRM.Automation</span></span>
* <span data-ttu-id="ac49b-391">도움말을 업데이트하고 'New-AzureRMAutomationSchedule'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-391">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="ac49b-392">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="ac49b-392">AzureRM.Compute</span></span>
* <span data-ttu-id="ac49b-393">-Tag 매개 변수를 Update/New-AzureRmAvailabilitySet에 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-393">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="ac49b-394">‘Add-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-394">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="ac49b-395">‘Remove-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-395">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="ac49b-396">‘Set-AzureRmVMAccessExtension’에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-396">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="ac49b-397">기본으로 SinglePlacementGroup을 false로 설정하고 단일 배치 그룹에 VMSS를 만들 수 있는 스위치 매개 변수 'SinglePlacementGroup'을 추가하도록 New-AzureRmVmss에 대한 SimpleParameterSet을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-397">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="ac49b-398">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="ac49b-398">AzureRM.EventHub</span></span>
* <span data-ttu-id="ac49b-399">PSEventHubDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="ac49b-399">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="ac49b-400">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ac49b-400">AzureRM.KeyVault</span></span>
* <span data-ttu-id="ac49b-401">Set-AzureRmKeyVaultAccessPolicy에 대한 오류 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-401">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="ac49b-402">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ac49b-402">AzureRM.LogicApp</span></span>
* <span data-ttu-id="ac49b-403">New-AzureRmLogicApp에서 "매개 변수 집합을 확인할 수 없습니다" 오류 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-403">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="ac49b-404">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="ac49b-404">AzureRM.Network</span></span>
* <span data-ttu-id="ac49b-405">Set/Add-AzureRmVirtualNetworkPeering에 대한 여러 테넌트의 가상 네트워크에서 피어링을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="ac49b-405">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="ac49b-406">Application Gateway에 대한 아래 cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-406">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="ac49b-407">New-AzureRmApplicationGateway: EnableFIPS 플래그 및 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-407">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="ac49b-408">New-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-408">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="ac49b-409">Set-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-409">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="ac49b-410">최신 생성기를 사용하여 RouteTable cmdlet을 재생성</span><span class="sxs-lookup"><span data-stu-id="ac49b-410">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="ac49b-411">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="ac49b-411">AzureRM.Relay</span></span>
* <span data-ttu-id="ac49b-412">markdown 파일을 업데이트하여 예제에서 매개 변수 이름 문제에 대해 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-412">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="ac49b-413">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="ac49b-413">AzureRM.Resources</span></span>
* <span data-ttu-id="ac49b-414">Roledefinition 및 Roleassignment cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-414">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="ac49b-415">페이징의 일부분으로 수행하는 추가 roledefinition 호출을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-415">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="ac49b-416">Get-AzureRmRoleAssignment cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-416">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="ac49b-417">-ExpandPrincipalGroups 명령 매개 변수 기능 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-417">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="ac49b-418">'Get-AzureRmResource'에서 '-ResourceType' 매개 변수가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-418">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="ac49b-419">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ac49b-419">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="ac49b-420">top 및 skip 매개 변수가 cmdlet 목록을 나열하도록 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-420">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="ac49b-421">표준을 프리미엄 네임스페이스 마이그레이션 cmdlet에 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-421">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="ac49b-422">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="ac49b-422">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="ac49b-423">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="ac49b-423">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="ac49b-424">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="ac49b-424">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="ac49b-425">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="ac49b-425">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="ac49b-426">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="ac49b-426">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="ac49b-427">PSServiceBusDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="ac49b-427">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="ac49b-428">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ac49b-428">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="ac49b-429">‘New-AzureRmServiceFabricCluster’에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-429">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="ac49b-430">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="ac49b-430">AzureRM.Sql</span></span>
* <span data-ttu-id="ac49b-431">Management.Sql에 대한 새 cmdlet을 추가하여 고객이 TDE 인증서를 SQL Server 인스턴스 또는 Managed Instance에 추가할 수 있도록 허용</span><span class="sxs-lookup"><span data-stu-id="ac49b-431">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="ac49b-432">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="ac49b-432">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="ac49b-433">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="ac49b-433">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="ac49b-434">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="ac49b-434">AzureRM.Websites</span></span>
* <span data-ttu-id="ac49b-435">`Set-AzureRmWebApp -AssignIdentity` 및 `Set-AzureRmWebAppSlot -AssignIdentity`가 false로 설정되면 사이트 개체에서 Identity 속성이 제거됩니다. 미리보기 태그도 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-435">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="ac49b-436">`Get-AzureRmWebAppMetrics`, `Get-AzureRmAppServicePlanMetrics` 예제가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-436">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="ac49b-437">`Set-AzureRmWebApp -PhpVersion`이 유효한 php 버전으로 해제 지원</span><span class="sxs-lookup"><span data-stu-id="ac49b-437">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="ac49b-438">6.4.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="ac49b-438">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="ac49b-439">일반</span><span class="sxs-lookup"><span data-stu-id="ac49b-439">General</span></span>
* <span data-ttu-id="ac49b-440">대부분의 모듈에 대한 도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-440">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="ac49b-441">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="ac49b-441">AzureRM.Profile</span></span>
* <span data-ttu-id="ac49b-442">기본 출력 형식에 추가된 Ps1Xml 특성</span><span class="sxs-lookup"><span data-stu-id="ac49b-442">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="ac49b-443">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="ac49b-443">AzureRM.Compute</span></span>
* <span data-ttu-id="ac49b-444">VMSS에 대한 IP 태그 기능</span><span class="sxs-lookup"><span data-stu-id="ac49b-444">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="ac49b-445">'New-AzureRmVmssIpTagConfig' cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-445">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="ac49b-446">New-AzureRmVmssIpConfig에 IpTag 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-446">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="ac49b-447">VMSS에 대한 자동 OS 롤백 기능</span><span class="sxs-lookup"><span data-stu-id="ac49b-447">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="ac49b-448">New-AzureRmVmssConfig 및 Update-AzureRmVmss에 DisableAutoRollback 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-448">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="ac49b-449">Vmss에 대한 OS 업그레이드 기록 기능</span><span class="sxs-lookup"><span data-stu-id="ac49b-449">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="ac49b-450">Get-AzureRmVmss에 OSUpgradeHistory 스위치 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-450">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="ac49b-451">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="ac49b-451">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="ac49b-452">다음 명령을 통해 카탈로그 액세스 제어 목록에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-452">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="ac49b-453">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="ac49b-453">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="ac49b-454">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="ac49b-454">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="ac49b-455">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="ac49b-455">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="ac49b-456">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ac49b-456">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="ac49b-457">Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl에 대한 취소 지원 및 진행률 추적 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-457">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="ac49b-458">Export-AzureRmDataLakeStoreChildItemProperties에 대한 취소 지원 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-458">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="ac49b-459">재귀 작업을 수행하는 cmdlet에 대한 디버그 메시지 플러시 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-459">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="ac49b-460">DataLake cmdlet의 테스트 위치 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-460">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="ac49b-461">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="ac49b-461">AzureRM.EventHub</span></span>
* <span data-ttu-id="ac49b-462">목록 작업 cmdlet Get-AzureRmEventHub 및 Get-AzureRmEventHubConsumerGroup에 선택적 MaxCount 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-462">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="ac49b-463">새 EventHub 만드는 동안 하나 이상의 매개 변수가 필요한 New-AzureRmEventHub cmdlet 문제를 해결.</span><span class="sxs-lookup"><span data-stu-id="ac49b-463">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="ac49b-464">기본 매개 변수 집합을 제공.</span><span class="sxs-lookup"><span data-stu-id="ac49b-464">Provided Default Parameter set.</span></span>
* <span data-ttu-id="ac49b-465">선택적 매개 변수 -KeyValue를 New-AzureRmEventHubKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-465">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="ac49b-466">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ac49b-466">AzureRM.KeyVault</span></span>
* <span data-ttu-id="ac49b-467">Get-AzureRmKeyVault -Tag 실행 시 모든 리소스가 리턴되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-467">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="ac49b-468">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="ac49b-468">AzureRM.Network</span></span>
* <span data-ttu-id="ac49b-469">영역 중복 VirtualNetworkGateways에 대한 새 Sku를 노출합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-469">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="ac49b-470">기능에 대한 새 명령이 추가됨: ARM을 통한 ExpressRoute Partner APIs</span><span class="sxs-lookup"><span data-stu-id="ac49b-470">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="ac49b-471">Get- AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-471">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="ac49b-472">Set-AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-472">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="ac49b-473">Add-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-473">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="ac49b-474">Get-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-474">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="ac49b-475">Remove-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-475">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="ac49b-476">Get-AzureRMExpressRouteCrossConnectionArpTable 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-476">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="ac49b-477">Get-AzureRMExpressRouteCrossConnectionRouteTable 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-477">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="ac49b-478">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-478">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="ac49b-479">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="ac49b-479">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="ac49b-480">Get-AzureRmRecoveryServicesBackupStatus cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-480">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="ac49b-481">이 cmdlet은 VM ID를 가져와서 VM이 구독에서 일부 자격 증명 모음으로 보호되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-481">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="ac49b-482">이러한 자격 증명 모음이 존재하는 경우 cmdlet은 자격 증명 모음 세부 정보를 출력 합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-482">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="ac49b-483">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="ac49b-483">AzureRM.Resources</span></span>
* <span data-ttu-id="ac49b-484">Get-AzureRmPolicyAssignment cmdlet을 다음과 같이 업데이트함.</span><span class="sxs-lookup"><span data-stu-id="ac49b-484">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="ac49b-485">관리 그룹 수준에서 -Scope 값 리스팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-485">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="ac49b-486">관리 그룹 수준에서 -Scope 값을 사용하여 개별 할당값을 검색하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-486">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="ac49b-487">제어 매개 변수에 -Effective 및 -All 스위치 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-487">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="ac49b-488">Get/New/Remove/Set-AzureRmPolicyDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-488">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="ac49b-489">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-489">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="ac49b-490">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-490">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="ac49b-491">Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-491">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="ac49b-492">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-492">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="ac49b-493">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-493">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="ac49b-494">'New-AzureRmResourceGroupDeployment'에서 'TemplateParameterObject'를 사용하는 경우 매개 변수에 KeyVault 비밀 참조 지원 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-494">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="ac49b-495">'New-AzureRmADAppCredential'에 대해 '-EndDate' 매개 변수가 무시되는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-495">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="ac49b-496">'Add-AzureRmADGroupMember'가 요청에 잘못된 URL을 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-496">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="ac49b-497">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ac49b-497">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="ac49b-498">선택적 매개 변수 -KeyValue를 New-AzureRmServiceBusKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-498">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="ac49b-499">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="ac49b-499">AzureRM.Sql</span></span>
* <span data-ttu-id="ac49b-500">New-AzureRmSqlDatabaseRestorePoint 도움말에서 SQLDW에 대한 사용자 정의 복원 지점 명시</span><span class="sxs-lookup"><span data-stu-id="ac49b-500">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="ac49b-501">몇 가지 cmdlet에서-ComputeGeneration 매개 변수의 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-501">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="ac49b-502">6.3.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="ac49b-502">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="ac49b-503">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="ac49b-503">AzureRM.Profile</span></span>
* <span data-ttu-id="ac49b-504">Enable-AzureRmContextAutoSave에 대한 오류 메시지 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-504">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="ac49b-505">이전 컨텍스트 없이 'Connect-AzureRmAccount' 실행 시 각 구독에 대한 컨텍스트 생성</span><span class="sxs-lookup"><span data-stu-id="ac49b-505">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="ac49b-506">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="ac49b-506">Azure.Storage</span></span>
* <span data-ttu-id="ac49b-507">도움말 파일 내 -Permissions 매개 변수에 대한 추가 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-507">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="ac49b-508">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="ac49b-508">AzureRM.Compute</span></span>
* <span data-ttu-id="ac49b-509">'Get-AzureRmVmDiskEncryptionStatus'가 데이터 디스크가 없는 VM에 대해 관찰된 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-509">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="ac49b-510">Compute 클라이언트 라이브러리 버전을 업데이트하여 다음 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-510">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="ac49b-511">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="ac49b-511">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="ac49b-512">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="ac49b-512">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="ac49b-513">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="ac49b-513">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="ac49b-514">다음 cmdlet이 '작업 ID' 및 '작업 상태'를 올바르게 표시하도록 수정:</span><span class="sxs-lookup"><span data-stu-id="ac49b-514">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="ac49b-515">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="ac49b-515">Start-AzureRmVM</span></span>
    - <span data-ttu-id="ac49b-516">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="ac49b-516">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="ac49b-517">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="ac49b-517">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="ac49b-518">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="ac49b-518">Set-AzureRmVM</span></span>
    - <span data-ttu-id="ac49b-519">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="ac49b-519">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="ac49b-520">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="ac49b-520">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="ac49b-521">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="ac49b-521">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="ac49b-522">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="ac49b-522">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="ac49b-523">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="ac49b-523">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="ac49b-524">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="ac49b-524">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="ac49b-525">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="ac49b-525">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="ac49b-526">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="ac49b-526">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="ac49b-527">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="ac49b-527">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="ac49b-528">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="ac49b-528">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="ac49b-529">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="ac49b-529">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="ac49b-530">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="ac49b-530">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="ac49b-531">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="ac49b-531">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="ac49b-532">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="ac49b-532">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="ac49b-533">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="ac49b-533">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="ac49b-534">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ac49b-534">AzureRM.EventGrid</span></span>
* <span data-ttu-id="ac49b-535">Update-AzureRmEventGridSubscription cmdlet의 SubjectBeginsWith/SubjectEndsWith에 대한 ValidateNotNullOrEmpty 유효성 검사 조건을 제거하여 필요에 따라 이러한 매개 변수를 빈 문자열로 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-535">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="ac49b-536">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ac49b-536">AzureRM.KeyVault</span></span>
* <span data-ttu-id="ac49b-537">Get-AzureRmKeyVault -Tag 실행 시 태그가 리턴되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-537">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="ac49b-538">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ac49b-538">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="ac49b-539">Policy Insights cmdlet의 공개 릴리스</span><span class="sxs-lookup"><span data-stu-id="ac49b-539">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="ac49b-540">API 버전 2018-04-04 사용</span><span class="sxs-lookup"><span data-stu-id="ac49b-540">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="ac49b-541">PolicyDefinitionReferenceId를 Get-AzureRmPolicyStateSummary의 결과 집합에 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-541">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="ac49b-542">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="ac49b-542">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="ac49b-543">-Vault 매개 변수를 RecoveryServices.Backup cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="ac49b-543">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="ac49b-544">전달되는 경우 이는 Set-AzureRmRecoveryServicesContext cmdlet을 재정의함.</span><span class="sxs-lookup"><span data-stu-id="ac49b-544">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="ac49b-545">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="ac49b-545">AzureRM.Sql</span></span>
* <span data-ttu-id="ac49b-546">Get-AzureRmSqlDatabaseExpanded에 대한 도움말 파일의 예가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-546">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="ac49b-547">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ac49b-547">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="ac49b-548">Add-AzureRmTrafficManagerEndpointConfig에대한 도움말 파일이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-548">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="ac49b-549">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="ac49b-549">AzureRM.Websites</span></span>
* <span data-ttu-id="ac49b-550">-AssignIdentity를 사용할 때 AppSetting을 덮어쓰지 않도록 'Set-AzureRmWebApp'이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-550">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="ac49b-551">'New-AzureRmWebAppSlot'이 AppServicePlan을 옵션 매개변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-551">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="ac49b-552">6.2.1 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="ac49b-552">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="ac49b-553">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ac49b-553">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="ac49b-554">PSWorkspace 모델이 Network 형식을 매개 변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-554">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="ac49b-555">6.2.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="ac49b-555">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="ac49b-556">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="ac49b-556">AzureRM.Profile</span></span>
* <span data-ttu-id="ac49b-557">Newtonsoft.Json의 버전 10.0.3이 모듈 가져오기에 로드되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-557">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="ac49b-558">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="ac49b-558">AzureRM.Compute</span></span>
* <span data-ttu-id="ac49b-559">VMSS VM 업데이트 기능</span><span class="sxs-lookup"><span data-stu-id="ac49b-559">VMSS VM Update feature</span></span>
    - <span data-ttu-id="ac49b-560">'Update-AzureRmVmssVM' 및 'New-AzureRmVMDataDisk' cmdlets 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-560">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="ac49b-561">데이터 디스크를 Vmss VM에 추가할 수 있도록 지원하기 위해 VirtualMachineScaleSetVM 매개변수를 'Add-AzureRmVMDataDisk' cmdlet에 추가하였습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-561">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="ac49b-562">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="ac49b-562">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="ac49b-563">ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.8.0-preview로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-563">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="ac49b-564">팩터리 리포지토리 작업 구성 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-564">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="ac49b-565">QuickBooks LinkedService가 ConsumerKey 및 consumerSecret 속성을 노출하도록 업데이트됨 </span><span class="sxs-lookup"><span data-stu-id="ac49b-565">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="ac49b-566">여러 모델 유형을 SecretBase에서 개체로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="ac49b-566">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="ac49b-567">Blob 이벤트 트리거 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-567">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="ac49b-568">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ac49b-568">AzureRM.KeyVault</span></span>
* <span data-ttu-id="ac49b-569">예제 출력으로 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-569">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="ac49b-570">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="ac49b-570">AzureRM.Network</span></span>
* <span data-ttu-id="ac49b-571">Network Watcher cmdlet에서 트래픽 분석 매개 변수를 사용가능하도록 설정</span><span class="sxs-lookup"><span data-stu-id="ac49b-571">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="ac49b-572">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="ac49b-572">AzureRM.Resources</span></span>
* <span data-ttu-id="ac49b-573">'Get AzureRmResource'에서 반환된 'PSResource' 개체의 'Properties' 속성의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-573">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="ac49b-574">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="ac49b-574">AzureRM.Scheduler</span></span>
* <span data-ttu-id="ac49b-575">ServiceBusQueueJob 업데이트가 새 인증 값을 설정하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ac49b-575">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="ac49b-576">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="ac49b-576">AzureRM.Sql</span></span>
* <span data-ttu-id="ac49b-577">옵션 LicenseType 매개 변수를 사용하여 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="ac49b-577">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="ac49b-578">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="ac49b-578">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="ac49b-579">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="ac49b-579">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="ac49b-580">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="ac49b-580">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="ac49b-581">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="ac49b-581">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="ac49b-582">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="ac49b-582">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="ac49b-583">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="ac49b-583">AzureRM.Websites</span></span>
* <span data-ttu-id="ac49b-584">'New-AzureRMWebApp'이 전략 라이브러리의 공통 알고리즘을 사용하도록 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-584">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="ac49b-585">6.1.0 - 2018년 5월</span><span class="sxs-lookup"><span data-stu-id="ac49b-585">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="ac49b-586">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="ac49b-586">AzureRM.Profile</span></span>
* <span data-ttu-id="ac49b-587">'Clear-AzureRmContext'를 실행하면 이전 기본 컨텍스트의 이름으로 빈 컨텍스트가 유지되어 사용자가 이전 이름으로 새 컨텍스트를 만들지 못하게 되는 문제를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-587">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="ac49b-588">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ac49b-588">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="ac49b-589">AS에서 게이트웨이가 작업을 연결하거나 연결 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-589">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="ac49b-590">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ac49b-590">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="ac49b-591">ApiVersions, ApiReleases 및 ApiRevisions에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-591">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="ac49b-592">ServiceFabric 백 엔드에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-592">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="ac49b-593">Application Insights 로거에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-593">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="ac49b-594">'기본' SKU를 API Management 서비스의 유효한 SKU로 인식하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-594">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="ac49b-595">개인 CA가 발급한 인증서를 루트 또는 CA로 설치하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-595">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="ac49b-596">KeyVault 및 다중 프록시 호스트 이름을 통한 사용자 정의 SSL 인증서를 수락하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-596">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="ac49b-597">MSI ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="ac49b-597">Added support for MSI identity</span></span>
* <span data-ttu-id="ac49b-598">URL을 통한 정책을 수락하는 지원 추가됨 참고: 다음 cmdlet은 이후 릴리스에서 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-598">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="ac49b-599">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="ac49b-599">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="ac49b-600">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac49b-600">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="ac49b-601">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="ac49b-601">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="ac49b-602">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="ac49b-602">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="ac49b-603">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="ac49b-603">AzureRM.Batch</span></span>
* <span data-ttu-id="ac49b-604">새 cmdlet Get AzureBatchPoolNodeCounts 릴리스</span><span class="sxs-lookup"><span data-stu-id="ac49b-604">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="ac49b-605">새 cmdlet Start-AzureBatchComputeNodeServiceLogUpload 릴리스</span><span class="sxs-lookup"><span data-stu-id="ac49b-605">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="ac49b-606">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="ac49b-606">AzureRM.Consumption</span></span>
* <span data-ttu-id="ac49b-607">Expand, ResourceGroup, InstanceName, InstanceId, Tags, Top on Cmdlet Get-AzureRmConsumptionUsageDetail 등 새 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="ac49b-607">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="ac49b-608">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ac49b-608">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="ac49b-609">Export-AzureRmDataLakeStoreChildItemProperties에 대한 예제 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-609">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="ac49b-610">Set-AzureRmDataLakeStoreItemAclEntry에서 재귀 사례에 대한 null 매개 변수 예외 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-610">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="ac49b-611">Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry에 대한 도움말 파일 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-611">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="ac49b-612">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="ac49b-612">AzureRM.Network</span></span>
* <span data-ttu-id="ac49b-613">18.0.0-preview에서 19.0.0-preview로 네트워크 SDK 버전 업그레이드</span><span class="sxs-lookup"><span data-stu-id="ac49b-613">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="ac49b-614">프로토콜 구성을 만들기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="ac49b-614">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="ac49b-615">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac49b-615">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="ac49b-616">기존 Express 경로 회로에 새 회로 연결을 추가하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="ac49b-616">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="ac49b-617">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="ac49b-617">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="ac49b-618">기존 Express 경로 회로에서 회로 연결을 제거하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="ac49b-618">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="ac49b-619">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="ac49b-619">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="ac49b-620">회로 연결을 검색하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="ac49b-620">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="ac49b-621">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="ac49b-621">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="ac49b-622">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ac49b-622">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="ac49b-623">생성된 인증서로 고정 서버 인증 사용(문제 # 5998)</span><span class="sxs-lookup"><span data-stu-id="ac49b-623">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="ac49b-624">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="ac49b-624">AzureRM.Sql</span></span>
* <span data-ttu-id="ac49b-625">AuditActions 또는 AuditActionGroups를 제거할 수 있도록 업데이트된 감사 cmdlet</span><span class="sxs-lookup"><span data-stu-id="ac49b-625">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="ac49b-626">'Azure 복구 서비스 자격 증명 모음을 사용하여 장기 보존 정책을 구성하면 정책이 더 이상 지원되지 않습니다. 새로운 유연 보유 정책으로 요청을 제출하십시오.'라는 메시지와 함께 명령이 실패하는 새로운 유연 보유 정책을 설정할 때</span><span class="sxs-lookup"><span data-stu-id="ac49b-626">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="ac49b-627">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy의 문제 수정</span><span class="sxs-lookup"><span data-stu-id="ac49b-627">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="ac49b-628">Azure SQL Database/ElasticPool Creation/Update 관련 cmdlet을 모두 업데이트하여 규모 및 계층 관련 속성에 대한 SKU 속성을 지원하는 새 데이터베이스 API를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-628">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="ac49b-629">업데이트된 cmdlet는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-629">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="ac49b-630">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="ac49b-630">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="ac49b-631">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="ac49b-631">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="ac49b-632">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="ac49b-632">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="ac49b-633">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="ac49b-633">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="ac49b-634">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="ac49b-634">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="ac49b-635">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ac49b-635">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="ac49b-636">-Name 매개 변수를 사용할 때 -ResourceGroupName 매개 변수가 필요하도록 'Get-AzureRmTrafficManagerProfile'에 대한 매개 변수를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="ac49b-636">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
