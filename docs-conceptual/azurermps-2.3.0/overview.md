---
title: Azure Stack PowerShell 개요 | Microsoft Docs
description: 설치 및 구성에 대한 설명을 포함한 Azure Stack PowerShell 개요입니다.
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: d514e43d82bcb51f65831dc506e58e8747db0381
ms.sourcegitcommit: ff44dec6418a449757bded3c6ebe0a7d4c05ee6e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/01/2018
ms.locfileid: "50737325"
---
# <a name="azurerm-module-230"></a><span data-ttu-id="cabe8-103">AzureRM 모듈 2.3.0</span><span class="sxs-lookup"><span data-stu-id="cabe8-103">AzureRM Module 2.3.0</span></span>

## <a name="requirements"></a><span data-ttu-id="cabe8-104">Requirements:</span><span class="sxs-lookup"><span data-stu-id="cabe8-104">Requirements:</span></span>
<span data-ttu-id="cabe8-105">최소 지원 Azure Stack 버전은 1808입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-105">Minimum supported Azure Stack version is 1808.</span></span>

<span data-ttu-id="cabe8-106">참고: 이전 버전을 사용하는 경우 1.2.11 버전을 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="cabe8-106">Note: If you are using an earlier version install version 1.2.11</span></span>


## <a name="install"></a><span data-ttu-id="cabe8-107">설치</span><span class="sxs-lookup"><span data-stu-id="cabe8-107">Install</span></span>
```powershell
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module -Name AzureRM -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force -ErrorAction Continue
Uninstall-Module AzureRM.AzureStackStorage -Force -ErrorAction Continue
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force
Get-Module Azure.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

```

##<a name="release-notes"></a><span data-ttu-id="cabe8-108">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="cabe8-108">Release Notes</span></span>
* <span data-ttu-id="cabe8-109">2.3.0 릴리스에는 호환성이 손상되는 변경 목록이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-109">The release 2.3.0 comes with a list of breaking changes.</span></span> <span data-ttu-id="cabe8-110">1.2.11 버전에서 업그레이드하여, https://aka.ms/azspowershellmigration에 마이그레이션 가이드를 만들었습니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-110">To upgrade from the 1.2.11 version, we have created a migration guide at https://aka.ms/azspowershellmigration</span></span>
* <span data-ttu-id="cabe8-111">이 릴리스는 azurestack 특정 api 프로필 2018-03-01-hybrid에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-111">This release corresponds to the azurestack specific api profile 2018-03-01-hybrid</span></span>
* <span data-ttu-id="cabe8-112">모든 모듈은 AzureRm.Profile 모듈에 대한 종속성 이상으로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-112">All the modules are taking greater than or equal to dependency on the AzureRm.Profile module.</span></span>
* <span data-ttu-id="cabe8-113">각 모듈이 지원하는 api 버전이 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-113">Api version suppoerted by  each of the modules are updated.</span></span> 
    * <span data-ttu-id="cabe8-114">컴퓨팅 - 2017-03-30</span><span class="sxs-lookup"><span data-stu-id="cabe8-114">Compute - 2017-03-30</span></span>
    * <span data-ttu-id="cabe8-115">네트워크 - 2017-10-01</span><span class="sxs-lookup"><span data-stu-id="cabe8-115">Network - 2017-10-01</span></span>
    * <span data-ttu-id="cabe8-116">저장소 - 2016-01-01</span><span class="sxs-lookup"><span data-stu-id="cabe8-116">Storage - 2016-01-01</span></span>
    * <span data-ttu-id="cabe8-117">리소스 - 2018-02-01</span><span class="sxs-lookup"><span data-stu-id="cabe8-117">Resources - 2018-02-01</span></span>
    * <span data-ttu-id="cabe8-118">Keyvault - 2016-10-01</span><span class="sxs-lookup"><span data-stu-id="cabe8-118">Keyvault - 2016-10-01</span></span>
    * <span data-ttu-id="cabe8-119">Dns - 2016-04-01</span><span class="sxs-lookup"><span data-stu-id="cabe8-119">Dns - 2016-04-01</span></span>
* <span data-ttu-id="cabe8-120">각 리소스 종류에 대한 전체 API 버전 맵은 https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json에서 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-120">The complete api version map for each of the resource types can be found at https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json</span></span>

## <a name="content"></a><span data-ttu-id="cabe8-121">콘텐츠:</span><span class="sxs-lookup"><span data-stu-id="cabe8-121">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="cabe8-122">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="cabe8-122">Azure Bridge</span></span>
<span data-ttu-id="cabe8-123">Azure의 이미지를 배포할 수 있게 해주는 Azure Stack AzureBridge 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-123">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="cabe8-124">Backup</span><span class="sxs-lookup"><span data-stu-id="cabe8-124">Backup</span></span>
<span data-ttu-id="cabe8-125">관리자가 다음을 수행할 수 있도록 해주는 Backup 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-125">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="cabe8-126">백업이 저장되는 위치 구성</span><span class="sxs-lookup"><span data-stu-id="cabe8-126">Configure where backups are stored</span></span>
- <span data-ttu-id="cabe8-127">백업 수행</span><span class="sxs-lookup"><span data-stu-id="cabe8-127">Perform backups</span></span>
- <span data-ttu-id="cabe8-128">완료된 백업 나열 및 복원</span><span class="sxs-lookup"><span data-stu-id="cabe8-128">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="cabe8-129">상거래</span><span class="sxs-lookup"><span data-stu-id="cabe8-129">Commerce</span></span>
<span data-ttu-id="cabe8-130">Azure Stack 시스템의 집계 데이터 사용량을 볼 수 있는 방법을 제공하는 Azure Stack Commerce 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-130">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="cabe8-131">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="cabe8-131">Compute</span></span>
<span data-ttu-id="cabe8-132">컴퓨팅 할당량, 플랫폼 이미지, 관리 디스크 및 가상 머신 확장을 관리하는 기능을 제공하는 Azure Stack Compute 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-132">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, managed disks and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="cabe8-133">Fabric</span><span class="sxs-lookup"><span data-stu-id="cabe8-133">Fabric</span></span>
<span data-ttu-id="cabe8-134">관리자가 다음 작업을 위해 인프라 구성 요소를 보고 관리할 수 있게 해주는 Azure Stack Fabric 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-134">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="cabe8-135">배율 단위 노드의 중지, 시작 및 종료</span><span class="sxs-lookup"><span data-stu-id="cabe8-135">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="cabe8-136">FRU 관련 활동에 대한 배율 단위 노드의 배출 및 재개</span><span class="sxs-lookup"><span data-stu-id="cabe8-136">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="cabe8-137">배율 단위 노드의 복구</span><span class="sxs-lookup"><span data-stu-id="cabe8-137">Repair of scale unit nodes</span></span>
- <span data-ttu-id="cabe8-138">인프라 역할의 다시 시작</span><span class="sxs-lookup"><span data-stu-id="cabe8-138">Restart of Infrastructure role</span></span>
- <span data-ttu-id="cabe8-139">인프라 역할 인스턴스의 중지, 시작 및 종료</span><span class="sxs-lookup"><span data-stu-id="cabe8-139">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="cabe8-140">새 IP 풀 만들기</span><span class="sxs-lookup"><span data-stu-id="cabe8-140">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="cabe8-141">갤러리</span><span class="sxs-lookup"><span data-stu-id="cabe8-141">Gallery</span></span>
<span data-ttu-id="cabe8-142">Azure Stack Marketplace에서 갤러리 항목을 관리하는 기능을 제공하는 Azure Stack Gallery 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-142">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="cabe8-143">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="cabe8-143">Infrastructure Insights</span></span>
<span data-ttu-id="cabe8-144">관리자가 다음을 수행할 수 있는 Infrastructure Insight 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-144">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="cabe8-145">Azure Stack 스탬프 리소스의 상태 보기</span><span class="sxs-lookup"><span data-stu-id="cabe8-145">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="cabe8-146">경고 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="cabe8-146">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="cabe8-147">KeyVault</span><span class="sxs-lookup"><span data-stu-id="cabe8-147">KeyVault</span></span>
<span data-ttu-id="cabe8-148">관리자가 KeyVault 할당량을 볼 수 있는 Azure Stack KeyVault 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-148">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="cabe8-149">네트워크</span><span class="sxs-lookup"><span data-stu-id="cabe8-149">Network</span></span>
<span data-ttu-id="cabe8-150">다음을 수행할 수 있는 Network 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-150">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="cabe8-151">네트워크 할당량 관리</span><span class="sxs-lookup"><span data-stu-id="cabe8-151">Management of network quotas</span></span>
- <span data-ttu-id="cabe8-152">공용 IP 주소, 가상 네트워크, 부하 분산 장치와 같은 할당된 네트워크 리소스 보기</span><span class="sxs-lookup"><span data-stu-id="cabe8-152">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="cabe8-153">관리자 개요를 표시하는 cmdlet을 제공</span><span class="sxs-lookup"><span data-stu-id="cabe8-153">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="cabe8-154">Storage</span><span class="sxs-lookup"><span data-stu-id="cabe8-154">Storage</span></span>
<span data-ttu-id="cabe8-155">Azure Stack Storage 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-155">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="cabe8-156">이 릴리스에서는 다음을 수행하기 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-156">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="cabe8-157">저장소 할당량 관리</span><span class="sxs-lookup"><span data-stu-id="cabe8-157">Manage storage quotas</span></span>
- <span data-ttu-id="cabe8-158">삭제된 저장소 리소스 가비지 수집</span><span class="sxs-lookup"><span data-stu-id="cabe8-158">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="cabe8-159">삭제된 저장소 계정 복원</span><span class="sxs-lookup"><span data-stu-id="cabe8-159">Restore deleted storage accounts</span></span>
- <span data-ttu-id="cabe8-160">한 공유에서 다른 공유로 컨테이너 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="cabe8-160">Migrate containers from one share to another</span></span>
- <span data-ttu-id="cabe8-161">개별 저장소 구성 요소에 대한 정보 보기</span><span class="sxs-lookup"><span data-stu-id="cabe8-161">View information about the individual storage components</span></span>
- <span data-ttu-id="cabe8-162">사용량 및 성능 정보 보기</span><span class="sxs-lookup"><span data-stu-id="cabe8-162">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="cabe8-163">구독 관리자</span><span class="sxs-lookup"><span data-stu-id="cabe8-163">Subscription Admin</span></span>
<span data-ttu-id="cabe8-164">Azure Stack Subscription 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-164">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="cabe8-165">이 모듈은 관리자가 다음을 수행하기 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-165">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="cabe8-166">계획 및 제안 관리</span><span class="sxs-lookup"><span data-stu-id="cabe8-166">Manage plans and offers</span></span>
- <span data-ttu-id="cabe8-167">사용량 및 성능 정보 보기</span><span class="sxs-lookup"><span data-stu-id="cabe8-167">View usage and performance information</span></span>
- <span data-ttu-id="cabe8-168">RBAC 관리</span><span class="sxs-lookup"><span data-stu-id="cabe8-168">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="cabe8-169">구독</span><span class="sxs-lookup"><span data-stu-id="cabe8-169">Subscription</span></span>
<span data-ttu-id="cabe8-170">Azure Stack Subscription 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-170">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="cabe8-171">이 모듈은 사용자가 다음을 수행하기 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-171">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="cabe8-172">구독 생성, 삭제 및 업데이트</span><span class="sxs-lookup"><span data-stu-id="cabe8-172">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="cabe8-173">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="cabe8-173">Update</span></span>
<span data-ttu-id="cabe8-174">Azure Stack Update 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-174">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="cabe8-175">이 모듈에서 관리자는 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cabe8-175">In this module administrators can:</span></span>
- <span data-ttu-id="cabe8-176">사용 가능한 업데이트 나열 및 설치</span><span class="sxs-lookup"><span data-stu-id="cabe8-176">List and install available updates</span></span>
- <span data-ttu-id="cabe8-177">중단된 업데이트 다시 시작</span><span class="sxs-lookup"><span data-stu-id="cabe8-177">Resume interrupted updates</span></span>
- <span data-ttu-id="cabe8-178">설치된 업데이트 보기</span><span class="sxs-lookup"><span data-stu-id="cabe8-178">View installed updates</span></span>
