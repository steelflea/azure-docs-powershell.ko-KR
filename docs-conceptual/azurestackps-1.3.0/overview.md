---
title: Azure Stack Admin PowerShell 개요 | Microsoft Docs
description: 설치 및 구성에 대한 설명을 포함한 Azure Stack Admin PowerShell 개요입니다.
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: fb892daeafb1365ea62324392ac806cf9f3d39cf
ms.sourcegitcommit: 19dffee617477001f98d43e39a50ce1fad087b74
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/27/2018
ms.locfileid: "47179142"
---
# <a name="azure-stack-module-130"></a><span data-ttu-id="9d66e-103">Azure Stack 모듈 1.3.0</span><span class="sxs-lookup"><span data-stu-id="9d66e-103">Azure Stack Module 1.3.0</span></span>

## <a name="requirements"></a><span data-ttu-id="9d66e-104">Requirements:</span><span class="sxs-lookup"><span data-stu-id="9d66e-104">Requirements:</span></span>
<span data-ttu-id="9d66e-105">최소 지원 Azure Stack 버전은 1804입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-105">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="9d66e-106">참고: 이전 버전을 사용하는 경우 1.2.11 버전을 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="9d66e-106">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="9d66e-107">알려진 문제:</span><span class="sxs-lookup"><span data-stu-id="9d66e-107">Known issues:</span></span>

- <span data-ttu-id="9d66e-108">경고 닫기에는 Azure Stack 버전 1803이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-108">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="9d66e-109">일부 저장소 cmdlet는 Azure Stack 버전 1804가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-109">Some Storage cmdlets do require Azure Stack version 1804</span></span>
- <span data-ttu-id="9d66e-110">New-AzsOffer는 상태를 공개하여 제안을 만들 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-110">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="9d66e-111">상태를 변경하려면 Set-AzsOffer cmdlet을 나중에 호출해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-111">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="9d66e-112">재배포하지 않고는 IP 풀을 제거할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-112">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="9d66e-113">주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="9d66e-113">Breaking Changes</span></span>
<span data-ttu-id="9d66e-114">1.2.11에서 마이그레이션하는 호환성이 손상되는 변경은 모두 여기 https://aka.ms/azspowershellmigration에 문서화되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-114">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="9d66e-115">설치</span><span class="sxs-lookup"><span data-stu-id="9d66e-115">Install</span></span>
```
# Remove previous Versions
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Uninstall-Module -Name AzureStack -Force 


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.3.0
```
## <a name="content"></a><span data-ttu-id="9d66e-116">콘텐츠:</span><span class="sxs-lookup"><span data-stu-id="9d66e-116">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="9d66e-117">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="9d66e-117">Azure Bridge</span></span>
<span data-ttu-id="9d66e-118">Azure의 이미지를 배포할 수 있게 해주는 Azure Stack AzureBridge 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-118">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="9d66e-119">Backup</span><span class="sxs-lookup"><span data-stu-id="9d66e-119">Backup</span></span>
<span data-ttu-id="9d66e-120">관리자가 다음을 수행할 수 있도록 해주는 Backup 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-120">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="9d66e-121">백업이 저장되는 위치 구성</span><span class="sxs-lookup"><span data-stu-id="9d66e-121">Configure where backups are stored</span></span>
- <span data-ttu-id="9d66e-122">백업 수행</span><span class="sxs-lookup"><span data-stu-id="9d66e-122">Perform backups</span></span>
- <span data-ttu-id="9d66e-123">완료된 백업 나열 및 복원</span><span class="sxs-lookup"><span data-stu-id="9d66e-123">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="9d66e-124">상거래</span><span class="sxs-lookup"><span data-stu-id="9d66e-124">Commerce</span></span>
<span data-ttu-id="9d66e-125">Azure Stack 시스템의 집계 데이터 사용량을 볼 수 있는 방법을 제공하는 Azure Stack Commerce 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-125">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="9d66e-126">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="9d66e-126">Compute</span></span>
<span data-ttu-id="9d66e-127">컴퓨팅 할당량, 플랫폼 이미지 및 가상 컴퓨터 확장을 관리하는 기능을 제공하는 Azure Stack Compute 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-127">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="9d66e-128">Fabric</span><span class="sxs-lookup"><span data-stu-id="9d66e-128">Fabric</span></span>
<span data-ttu-id="9d66e-129">관리자가 다음 작업을 위해 인프라 구성 요소를 보고 관리할 수 있게 해주는 Azure Stack Fabric 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-129">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="9d66e-130">배율 단위 노드의 중지, 시작 및 종료</span><span class="sxs-lookup"><span data-stu-id="9d66e-130">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="9d66e-131">FRU 관련 활동에 대한 배율 단위 노드의 배출 및 재개</span><span class="sxs-lookup"><span data-stu-id="9d66e-131">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="9d66e-132">배율 단위 노드의 복구</span><span class="sxs-lookup"><span data-stu-id="9d66e-132">Repair of scale unit nodes</span></span>
- <span data-ttu-id="9d66e-133">인프라 역할의 다시 시작</span><span class="sxs-lookup"><span data-stu-id="9d66e-133">Restart of Infrastructure role</span></span>
- <span data-ttu-id="9d66e-134">인프라 역할 인스턴스의 중지, 시작 및 종료</span><span class="sxs-lookup"><span data-stu-id="9d66e-134">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="9d66e-135">새 IP 풀 만들기</span><span class="sxs-lookup"><span data-stu-id="9d66e-135">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="9d66e-136">갤러리</span><span class="sxs-lookup"><span data-stu-id="9d66e-136">Gallery</span></span>
<span data-ttu-id="9d66e-137">Azure Stack Marketplace에서 갤러리 항목을 관리하는 기능을 제공하는 Azure Stack Gallery 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-137">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="9d66e-138">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="9d66e-138">Infrastructure Insights</span></span>
<span data-ttu-id="9d66e-139">관리자가 다음을 수행할 수 있는 Infrastructure Insight 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-139">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="9d66e-140">Azure Stack 스탬프 리소스의 상태 보기</span><span class="sxs-lookup"><span data-stu-id="9d66e-140">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="9d66e-141">경고 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="9d66e-141">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="9d66e-142">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9d66e-142">KeyVault</span></span>
<span data-ttu-id="9d66e-143">관리자가 KeyVault 할당량을 볼 수 있는 Azure Stack KeyVault 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-143">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="9d66e-144">네트워크</span><span class="sxs-lookup"><span data-stu-id="9d66e-144">Network</span></span>
<span data-ttu-id="9d66e-145">다음을 수행할 수 있는 Network 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-145">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="9d66e-146">네트워크 할당량 관리</span><span class="sxs-lookup"><span data-stu-id="9d66e-146">Management of network quotas</span></span>
- <span data-ttu-id="9d66e-147">공용 IP 주소, 가상 네트워크, 부하 분산 장치와 같은 할당된 네트워크 리소스 보기</span><span class="sxs-lookup"><span data-stu-id="9d66e-147">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="9d66e-148">관리자 개요를 표시하는 cmdlet을 제공</span><span class="sxs-lookup"><span data-stu-id="9d66e-148">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="9d66e-149">Storage</span><span class="sxs-lookup"><span data-stu-id="9d66e-149">Storage</span></span>
<span data-ttu-id="9d66e-150">Azure Stack Storage 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-150">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="9d66e-151">이 릴리스에서는 다음을 수행하기 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-151">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="9d66e-152">저장소 할당량 관리</span><span class="sxs-lookup"><span data-stu-id="9d66e-152">Manage storage quotas</span></span>
- <span data-ttu-id="9d66e-153">삭제된 저장소 리소스 가비지 수집</span><span class="sxs-lookup"><span data-stu-id="9d66e-153">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="9d66e-154">삭제된 저장소 계정 복원</span><span class="sxs-lookup"><span data-stu-id="9d66e-154">Restore deleted storage accounts</span></span>
- <span data-ttu-id="9d66e-155">한 공유에서 다른 공유로 컨테이너 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="9d66e-155">Migrate containers from one share to another</span></span>
- <span data-ttu-id="9d66e-156">개별 저장소 구성 요소에 대한 정보 보기</span><span class="sxs-lookup"><span data-stu-id="9d66e-156">View information about the individual storage components</span></span>
- <span data-ttu-id="9d66e-157">사용량 및 성능 정보 보기</span><span class="sxs-lookup"><span data-stu-id="9d66e-157">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="9d66e-158">구독 관리자</span><span class="sxs-lookup"><span data-stu-id="9d66e-158">Subscription Admin</span></span>
<span data-ttu-id="9d66e-159">Azure Stack Subscription 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-159">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="9d66e-160">이 모듈은 관리자가 다음을 수행하기 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-160">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="9d66e-161">계획 및 제안 관리</span><span class="sxs-lookup"><span data-stu-id="9d66e-161">Manage plans and offers</span></span>
- <span data-ttu-id="9d66e-162">사용량 및 성능 정보 보기</span><span class="sxs-lookup"><span data-stu-id="9d66e-162">View usage and performance information</span></span>
- <span data-ttu-id="9d66e-163">RBAC 관리</span><span class="sxs-lookup"><span data-stu-id="9d66e-163">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="9d66e-164">구독</span><span class="sxs-lookup"><span data-stu-id="9d66e-164">Subscription</span></span>
<span data-ttu-id="9d66e-165">Azure Stack Subscription 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-165">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="9d66e-166">이 모듈은 사용자가 다음을 수행하기 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-166">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="9d66e-167">구독 생성, 삭제 및 업데이트</span><span class="sxs-lookup"><span data-stu-id="9d66e-167">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="9d66e-168">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="9d66e-168">Update</span></span>
<span data-ttu-id="9d66e-169">Azure Stack Update 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-169">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="9d66e-170">이 모듈에서 관리자는 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d66e-170">In this module administrators can:</span></span>
- <span data-ttu-id="9d66e-171">사용 가능한 업데이트 나열 및 설치</span><span class="sxs-lookup"><span data-stu-id="9d66e-171">List and install available updates</span></span>
- <span data-ttu-id="9d66e-172">중단된 업데이트 다시 시작</span><span class="sxs-lookup"><span data-stu-id="9d66e-172">Resume interrupted updates</span></span>
- <span data-ttu-id="9d66e-173">설치된 업데이트 보기</span><span class="sxs-lookup"><span data-stu-id="9d66e-173">View installed updates</span></span>
