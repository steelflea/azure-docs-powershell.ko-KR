# <a name="azure-stack-module-140"></a><span data-ttu-id="f7c03-101">Azure Stack 모듈 1.4.0</span><span class="sxs-lookup"><span data-stu-id="f7c03-101">Azure Stack Module 1.4.0</span></span>

## <a name="requirements"></a><span data-ttu-id="f7c03-102">Requirements:</span><span class="sxs-lookup"><span data-stu-id="f7c03-102">Requirements:</span></span>
<span data-ttu-id="f7c03-103">최소 지원 Azure Stack 버전은 1804입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-103">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="f7c03-104">참고: 이전 버전을 사용하는 경우 1.2.11 버전을 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="f7c03-104">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="f7c03-105">알려진 문제:</span><span class="sxs-lookup"><span data-stu-id="f7c03-105">Known issues:</span></span>

- <span data-ttu-id="f7c03-106">경고 닫기에는 Azure Stack 버전 1803이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-106">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="f7c03-107">New-AzsOffer는 상태를 공개하여 제안을 만들 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-107">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="f7c03-108">상태를 변경하려면 Set-AzsOffer cmdlet을 나중에 호출해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-108">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="f7c03-109">재배포하지 않고는 IP 풀을 제거할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-109">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="f7c03-110">주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="f7c03-110">Breaking Changes</span></span>
<span data-ttu-id="f7c03-111">버전 1.3.0과 호환성이 손상되는 변경은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-111">There are no breaking changes from the version 1.3.0.</span></span> <span data-ttu-id="f7c03-112">1.2.11에서 마이그레이션하는 호환성이 손상되는 변경은 모두 여기 https://aka.ms/azspowershellmigration에 문서화되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-112">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="f7c03-113">설치</span><span class="sxs-lookup"><span data-stu-id="f7c03-113">Install</span></span>
```
# 1.4.0 can be installed side by side with 1.3.0
# Remove previous version 1.2.11
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Uninstall-Module -Name AzureStack -Force 


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.4.0
```
## <a name="release-notes"></a><span data-ttu-id="f7c03-114">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="f7c03-114">Release Notes</span></span>
    * <span data-ttu-id="f7c03-115">Azurestack 1.4.0 버전에는 이전 버전인 1.3.0과 호환성이 손상되는 변경은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-115">Azurestack 1.4.0 version has no breaking changes from the previous release 1.3.0</span></span>
    * <span data-ttu-id="f7c03-116">Azs.AzureBridge.Admin</span><span class="sxs-lookup"><span data-stu-id="f7c03-116">Azs.AzureBridge.Admin</span></span>
        - <span data-ttu-id="f7c03-117">페이지가 매겨진 결과 내에서 단일 페이지만 반환하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="f7c03-117">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="f7c03-118">Azs.Backup.Admin</span><span class="sxs-lookup"><span data-stu-id="f7c03-118">Azs.Backup.Admin</span></span>
        - <span data-ttu-id="f7c03-119">새 매개 변수 BackupFrequencyInHours, IsBackupSchedulerEnabled, BackupRetentionPeriodInDays를 Set-AzsBackupShare cmdlet에 추가</span><span class="sxs-lookup"><span data-stu-id="f7c03-119">Added new parameters BackupFrequencyInHours, IsBackupSchedulerEnabled, BackupRetentionPeriodInDays in cmdlet Set-AzsBackupShare</span></span>
        - <span data-ttu-id="f7c03-120">암호화 키 만들기를 용이하게 하기 위해 New-EncyptionKeyBase64 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="f7c03-120">Added a cmdlet New-EncyptionKeyBase64 to facilitate creating encryption key</span></span>
        - <span data-ttu-id="f7c03-121">페이지가 매겨진 결과 내에서 단일 페이지만 반환하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="f7c03-121">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="f7c03-122">Azs.Commerce.Admin</span><span class="sxs-lookup"><span data-stu-id="f7c03-122">Azs.Commerce.Admin</span></span>
        - <span data-ttu-id="f7c03-123">페이지가 매겨진 결과 내에서 단일 페이지만 반환하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="f7c03-123">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="f7c03-124">Azs.Fabric.Admin</span><span class="sxs-lookup"><span data-stu-id="f7c03-124">Azs.Fabric.Admin</span></span>
        - <span data-ttu-id="f7c03-125">페이지가 매겨진 결과 내에서 단일 페이지만 반환하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="f7c03-125">Fix for the bug that returned only a single page in paginated results</span></span>
        - <span data-ttu-id="f7c03-126">azurestack 스탬프에 새 배율 단위 노드를 추가하는 관리자를 활성화하는 Add-AzsScaleUnitNode cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="f7c03-126">Added a cmdlet Add-AzsScaleUnitNode to enable admin to add new scale unit nodes to the azurestack stamp</span></span>
        - <span data-ttu-id="f7c03-127">배율 단위 매개 변수 개체 생성을 용이하게 하기 위해 cmdlet 및 New-AzsScaleUnitNodeObject 추가</span><span class="sxs-lookup"><span data-stu-id="f7c03-127">Added cmdlet and New-AzsScaleUnitNodeObject to facilitate the creation scale unit parameter objects</span></span>
    * <span data-ttu-id="f7c03-128">Azs.Gallery.Admin</span><span class="sxs-lookup"><span data-stu-id="f7c03-128">Azs.Gallery.Admin</span></span>
        - <span data-ttu-id="f7c03-129">페이지가 매겨진 결과 내에서 단일 페이지만 반환하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="f7c03-129">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="f7c03-130">Azs.InfrastructureInsights.Admin</span><span class="sxs-lookup"><span data-stu-id="f7c03-130">Azs.InfrastructureInsights.Admin</span></span>
        - <span data-ttu-id="f7c03-131">페이지가 매겨진 결과 내에서 단일 페이지만 반환하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="f7c03-131">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="f7c03-132">Azs.Network.Admin</span><span class="sxs-lookup"><span data-stu-id="f7c03-132">Azs.Network.Admin</span></span>
        - <span data-ttu-id="f7c03-133">페이지가 매겨진 결과 내에서 단일 페이지만 반환하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="f7c03-133">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="f7c03-134">Azs.Update.Admin</span><span class="sxs-lookup"><span data-stu-id="f7c03-134">Azs.Update.Admin</span></span>
        - <span data-ttu-id="f7c03-135">페이지가 매겨진 결과 내에서 단일 페이지만 반환하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="f7c03-135">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="f7c03-136">Azs.Subscriptions</span><span class="sxs-lookup"><span data-stu-id="f7c03-136">Azs.Subscriptions</span></span>
        - <span data-ttu-id="f7c03-137">페이지가 매겨진 결과 내에서 단일 페이지만 반환하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="f7c03-137">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="f7c03-138">Azs.Subscriptions.Admin</span><span class="sxs-lookup"><span data-stu-id="f7c03-138">Azs.Subscriptions.Admin</span></span>
        - <span data-ttu-id="f7c03-139">위임된 공급자 제안 간에 구독을 이동하기 위한 Move-AzsSubscription cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="f7c03-139">Added a cmdlet Move-AzsSubscription to move subscriptions between delegated provider offers</span></span>
        - <span data-ttu-id="f7c03-140">사용자 구독이 위임된 공급자 제품 간에 이동할 수 있는지 유효성 검사를 하기 위해 Test-AzsMoveSubscription cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="f7c03-140">Added a cmdlet Test-AzsMoveSubscription to validate that user subscriptions can be moved between delegated provider offers</span></span>
        - <span data-ttu-id="f7c03-141">페이지가 매겨진 결과 내에서 단일 페이지만 반환하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="f7c03-141">Fix for the bug that returned only a single page in paginated results'</span></span>

## <a name="content"></a><span data-ttu-id="f7c03-142">콘텐츠:</span><span class="sxs-lookup"><span data-stu-id="f7c03-142">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="f7c03-143">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="f7c03-143">Azure Bridge</span></span>
<span data-ttu-id="f7c03-144">Azure의 이미지를 배포할 수 있게 해주는 Azure Stack AzureBridge 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-144">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="f7c03-145">Backup</span><span class="sxs-lookup"><span data-stu-id="f7c03-145">Backup</span></span>
<span data-ttu-id="f7c03-146">관리자가 다음을 수행할 수 있도록 해주는 Backup 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-146">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="f7c03-147">백업이 저장되는 위치 구성</span><span class="sxs-lookup"><span data-stu-id="f7c03-147">Configure where backups are stored</span></span>
- <span data-ttu-id="f7c03-148">백업 수행</span><span class="sxs-lookup"><span data-stu-id="f7c03-148">Perform backups</span></span>
- <span data-ttu-id="f7c03-149">완료된 백업 나열 및 복원</span><span class="sxs-lookup"><span data-stu-id="f7c03-149">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="f7c03-150">상거래</span><span class="sxs-lookup"><span data-stu-id="f7c03-150">Commerce</span></span>
<span data-ttu-id="f7c03-151">Azure Stack 시스템의 집계 데이터 사용량을 볼 수 있는 방법을 제공하는 Azure Stack Commerce 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-151">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="f7c03-152">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="f7c03-152">Compute</span></span>
<span data-ttu-id="f7c03-153">컴퓨팅 할당량, 플랫폼 이미지 및 가상 컴퓨터 확장을 관리하는 기능을 제공하는 Azure Stack Compute 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-153">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="f7c03-154">Fabric</span><span class="sxs-lookup"><span data-stu-id="f7c03-154">Fabric</span></span>
<span data-ttu-id="f7c03-155">관리자가 다음 작업을 위해 인프라 구성 요소를 보고 관리할 수 있게 해주는 Azure Stack Fabric 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-155">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="f7c03-156">배율 단위 노드의 중지, 시작 및 종료</span><span class="sxs-lookup"><span data-stu-id="f7c03-156">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="f7c03-157">FRU 관련 활동에 대한 배율 단위 노드의 배출 및 재개</span><span class="sxs-lookup"><span data-stu-id="f7c03-157">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="f7c03-158">배율 단위 노드의 복구</span><span class="sxs-lookup"><span data-stu-id="f7c03-158">Repair of scale unit nodes</span></span>
- <span data-ttu-id="f7c03-159">인프라 역할의 다시 시작</span><span class="sxs-lookup"><span data-stu-id="f7c03-159">Restart of Infrastructure role</span></span>
- <span data-ttu-id="f7c03-160">인프라 역할 인스턴스의 중지, 시작 및 종료</span><span class="sxs-lookup"><span data-stu-id="f7c03-160">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="f7c03-161">새 IP 풀 만들기</span><span class="sxs-lookup"><span data-stu-id="f7c03-161">Create new IP Pools</span></span>

### <a name="gallery"></a><span data-ttu-id="f7c03-162">갤러리</span><span class="sxs-lookup"><span data-stu-id="f7c03-162">Gallery</span></span>
<span data-ttu-id="f7c03-163">Azure Stack Marketplace에서 갤러리 항목을 관리하는 기능을 제공하는 Azure Stack Gallery 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-163">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="f7c03-164">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="f7c03-164">Infrastructure Insights</span></span>
<span data-ttu-id="f7c03-165">관리자가 다음을 수행할 수 있는 Infrastructure Insight 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-165">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="f7c03-166">Azure Stack 스탬프 리소스의 상태 보기</span><span class="sxs-lookup"><span data-stu-id="f7c03-166">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="f7c03-167">경고 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="f7c03-167">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="f7c03-168">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f7c03-168">KeyVault</span></span>
<span data-ttu-id="f7c03-169">관리자가 KeyVault 할당량을 볼 수 있는 Azure Stack KeyVault 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-169">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="f7c03-170">네트워크</span><span class="sxs-lookup"><span data-stu-id="f7c03-170">Network</span></span>
<span data-ttu-id="f7c03-171">다음을 수행할 수 있는 Network 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-171">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="f7c03-172">네트워크 할당량 관리</span><span class="sxs-lookup"><span data-stu-id="f7c03-172">Management of network quotas</span></span>
- <span data-ttu-id="f7c03-173">공용 IP 주소, 가상 네트워크, 부하 분산 장치와 같은 할당된 네트워크 리소스 보기</span><span class="sxs-lookup"><span data-stu-id="f7c03-173">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="f7c03-174">관리자 개요를 표시하는 cmdlet을 제공</span><span class="sxs-lookup"><span data-stu-id="f7c03-174">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="f7c03-175">Storage</span><span class="sxs-lookup"><span data-stu-id="f7c03-175">Storage</span></span>
<span data-ttu-id="f7c03-176">Azure Stack Storage 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-176">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="f7c03-177">이 릴리스에서는 다음을 수행하기 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-177">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="f7c03-178">저장소 할당량 관리</span><span class="sxs-lookup"><span data-stu-id="f7c03-178">Manage storage quotas</span></span>
- <span data-ttu-id="f7c03-179">삭제된 저장소 리소스 가비지 수집</span><span class="sxs-lookup"><span data-stu-id="f7c03-179">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="f7c03-180">삭제된 저장소 계정 복원</span><span class="sxs-lookup"><span data-stu-id="f7c03-180">Restore deleted storage accounts</span></span>
- <span data-ttu-id="f7c03-181">한 공유에서 다른 공유로 컨테이너 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="f7c03-181">Migrate containers from one share to another</span></span>
- <span data-ttu-id="f7c03-182">개별 저장소 구성 요소에 대한 정보 보기</span><span class="sxs-lookup"><span data-stu-id="f7c03-182">View information about the individual storage components</span></span>
- <span data-ttu-id="f7c03-183">사용량 및 성능 정보 보기</span><span class="sxs-lookup"><span data-stu-id="f7c03-183">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="f7c03-184">구독 관리자</span><span class="sxs-lookup"><span data-stu-id="f7c03-184">Subscription Admin</span></span>
<span data-ttu-id="f7c03-185">Azure Stack Subscription 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-185">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="f7c03-186">이 모듈은 관리자가 다음을 수행하기 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-186">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="f7c03-187">계획 및 제안 관리</span><span class="sxs-lookup"><span data-stu-id="f7c03-187">Manage plans and offers</span></span>
- <span data-ttu-id="f7c03-188">사용량 및 성능 정보 보기</span><span class="sxs-lookup"><span data-stu-id="f7c03-188">View usage and performance information</span></span>
- <span data-ttu-id="f7c03-189">RBAC 관리</span><span class="sxs-lookup"><span data-stu-id="f7c03-189">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="f7c03-190">구독</span><span class="sxs-lookup"><span data-stu-id="f7c03-190">Subscription</span></span>
<span data-ttu-id="f7c03-191">Azure Stack Subscription 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-191">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="f7c03-192">이 모듈은 사용자가 다음을 수행하기 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-192">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="f7c03-193">구독 생성, 삭제 및 업데이트</span><span class="sxs-lookup"><span data-stu-id="f7c03-193">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="f7c03-194">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="f7c03-194">Update</span></span>
<span data-ttu-id="f7c03-195">Azure Stack Update 관리자 모듈의 미리 보기 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-195">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="f7c03-196">이 모듈에서 관리자는 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f7c03-196">In this module administrators can:</span></span>
- <span data-ttu-id="f7c03-197">사용 가능한 업데이트 나열 및 설치</span><span class="sxs-lookup"><span data-stu-id="f7c03-197">List and install available updates</span></span>
- <span data-ttu-id="f7c03-198">중단된 업데이트 다시 시작</span><span class="sxs-lookup"><span data-stu-id="f7c03-198">Resume interrupted updates</span></span>
- <span data-ttu-id="f7c03-199">설치된 업데이트 보기</span><span class="sxs-lookup"><span data-stu-id="f7c03-199">View installed updates</span></span>
