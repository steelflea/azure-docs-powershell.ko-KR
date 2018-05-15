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
ms.date: 05/18/2017
ms.openlocfilehash: 143d92384fd270711378f6741ba59e88c12833d1
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/08/2018
---
# <a name="release-notes"></a><span data-ttu-id="a893b-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="a893b-103">Release notes</span></span>

<span data-ttu-id="a893b-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="a893b-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-220"></a><span data-ttu-id="a893b-105">2.2.0 버전</span><span class="sxs-lookup"><span data-stu-id="a893b-105">Version 2.2.0</span></span>
* <span data-ttu-id="a893b-106">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="a893b-106">Compute</span></span>
  - <span data-ttu-id="a893b-107">AzureDiskEncryptionForLinux 확장에서 암호화 상태 쿼리 에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a893b-107">Add support for querying encryption status from the AzureDiskEncryptionForLinux extension</span></span>
* <span data-ttu-id="a893b-108">DataFactory</span><span class="sxs-lookup"><span data-stu-id="a893b-108">DataFactory</span></span>
  - <span data-ttu-id="a893b-109">활동 창을 나열하는 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="a893b-109">Added new cmdlet for listing activity windows</span></span>
    + <span data-ttu-id="a893b-110">Get-AzureRmDataFactoryActivityWindow</span><span class="sxs-lookup"><span data-stu-id="a893b-110">Get-AzureRmDataFactoryActivityWindow</span></span>
* <span data-ttu-id="a893b-111">DataLake</span><span class="sxs-lookup"><span data-stu-id="a893b-111">DataLake</span></span>
  - <span data-ttu-id="a893b-112">`Host` 매개 변수를 `DatabaseHost`로 변경하고, 별칭을 `Host`에 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="a893b-112">Changed parameter `Host` to `DatabaseHost` and added alias to `Host`</span></span>
    + <span data-ttu-id="a893b-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="a893b-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
    + <span data-ttu-id="a893b-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="a893b-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
  - <span data-ttu-id="a893b-115">ACL 및 기본 ACL 제거 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a893b-115">Add support for ACL and Default ACL removal</span></span>
  - <span data-ttu-id="a893b-116">파일 및 폴더에 대한 이름이 없는 권한 가져오기 및 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a893b-116">Add support for getting and setting unnamed permissions on files and folders</span></span>
* <span data-ttu-id="a893b-117">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a893b-117">KeyVault</span></span>
  - <span data-ttu-id="a893b-118">인증서 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a893b-118">Add support for certificates</span></span>
    + <span data-ttu-id="a893b-119">Add-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="a893b-119">Add-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="a893b-120">Add-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="a893b-120">Add-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="a893b-121">Get-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="a893b-121">Get-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="a893b-122">Get-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="a893b-122">Get-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="a893b-123">Get-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="a893b-123">Get-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="a893b-124">Get-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="a893b-124">Get-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="a893b-125">Get-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="a893b-125">Get-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="a893b-126">Import-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="a893b-126">Import-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="a893b-127">New-AzureKeyVaultCertificateAdministratorDetails</span><span class="sxs-lookup"><span data-stu-id="a893b-127">New-AzureKeyVaultCertificateAdministratorDetails</span></span>
    + <span data-ttu-id="a893b-128">New-AzureKeyVaultCertificateOrganizationDetails</span><span class="sxs-lookup"><span data-stu-id="a893b-128">New-AzureKeyVaultCertificateOrganizationDetails</span></span>
    + <span data-ttu-id="a893b-129">New-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="a893b-129">New-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="a893b-130">Remove-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="a893b-130">Remove-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="a893b-131">Remove-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="a893b-131">Remove-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="a893b-132">Remove-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="a893b-132">Remove-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="a893b-133">Remove-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="a893b-133">Remove-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="a893b-134">Set-AzureKeyVaultCertificateAttribute</span><span class="sxs-lookup"><span data-stu-id="a893b-134">Set-AzureKeyVaultCertificateAttribute</span></span>
    + <span data-ttu-id="a893b-135">Set-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="a893b-135">Set-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="a893b-136">Set-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="a893b-136">Set-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="a893b-137">Stop-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="a893b-137">Stop-AzureKeyVaultCertificateOperation</span></span>
* <span data-ttu-id="a893b-138">네트워크</span><span class="sxs-lookup"><span data-stu-id="a893b-138">Network</span></span>

  - <span data-ttu-id="a893b-139">가속화된 네트워킹을 설정/해제하기 위해 네트워크 인터페이스에 새 스위치 매개 변수(+New-AzureRmNetworkInterface -EnableAcceleratedNetworking) 추가</span><span class="sxs-lookup"><span data-stu-id="a893b-139">New switch parameter added for network interface to enable/disable accelerated networking +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span></span>
  - <span data-ttu-id="a893b-140">활성-활성 게이트웨이 기능 PowerShell cmdlet 사용 설정</span><span class="sxs-lookup"><span data-stu-id="a893b-140">Enable Active-Active gateway feature PowerShell cmdlets</span></span>
    + <span data-ttu-id="a893b-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="a893b-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
    + <span data-ttu-id="a893b-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="a893b-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="a893b-143">새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="a893b-143">Added new cmdlet</span></span>
    + <span data-ttu-id="a893b-144">Test-AzureRmPrivateIpAddressAvailability</span><span class="sxs-lookup"><span data-stu-id="a893b-144">Test-AzureRmPrivateIpAddressAvailability</span></span>
* <span data-ttu-id="a893b-145">리소스</span><span class="sxs-lookup"><span data-stu-id="a893b-145">Resources</span></span>
  - <span data-ttu-id="a893b-146">공급자 및 리소스 cmdlet에서 영역 지원</span><span class="sxs-lookup"><span data-stu-id="a893b-146">Support zones in provider and resource cmdlets</span></span>
    + <span data-ttu-id="a893b-147">Get-AzureRmProvider</span><span class="sxs-lookup"><span data-stu-id="a893b-147">Get-AzureRmProvider</span></span>
    + <span data-ttu-id="a893b-148">New-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="a893b-148">New-AzureRmResource</span></span>
    + <span data-ttu-id="a893b-149">Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="a893b-149">Set-AzureRmResource</span></span>
* <span data-ttu-id="a893b-150">Sql</span><span class="sxs-lookup"><span data-stu-id="a893b-150">Sql</span></span>
  - <span data-ttu-id="a893b-151">서버 수준의 Azure SQL 위협 검색 정책 관리에 대한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="a893b-151">Added new cmdlets for Azure SQL threat detection policy management at server level</span></span>
    + <span data-ttu-id="a893b-152">Get-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a893b-152">Get-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="a893b-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a893b-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="a893b-154">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a893b-154">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
  - <span data-ttu-id="a893b-155">Sql Azure DataWarehouse에 대한 GeoBackupPolicy 설정/해제를 지원하는 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="a893b-155">Added new cmdlets to support enabling/disabling GeoBackupPolicy for Sql Azure DataWarehouses</span></span>
    + <span data-ttu-id="a893b-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="a893b-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
    + <span data-ttu-id="a893b-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="a893b-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
  - <span data-ttu-id="a893b-158">Azure Sql Advisor 및 권장 작업 API에 대한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="a893b-158">Added new cmdlets for Azure Sql Advisors and Recommended Actions APIs</span></span>
    + <span data-ttu-id="a893b-159">Get-AzureRmSqlDatabaseAdvisor</span><span class="sxs-lookup"><span data-stu-id="a893b-159">Get-AzureRmSqlDatabaseAdvisor</span></span>
    + <span data-ttu-id="a893b-160">Get-AzureRmSqlElasticPoolAdvisor</span><span class="sxs-lookup"><span data-stu-id="a893b-160">Get-AzureRmSqlElasticPoolAdvisor</span></span>
    + <span data-ttu-id="a893b-161">Get-AzureRmSqlServerAdvisor</span><span class="sxs-lookup"><span data-stu-id="a893b-161">Get-AzureRmSqlServerAdvisor</span></span>
    + <span data-ttu-id="a893b-162">Get-AzureRmSqlDatabaseRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="a893b-162">Get-AzureRmSqlDatabaseRecommendedActions</span></span>
    + <span data-ttu-id="a893b-163">Get-AzureRmSqlElasticPoolRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="a893b-163">Get-AzureRmSqlElasticPoolRecommendedActions</span></span>
    + <span data-ttu-id="a893b-164">Get-AzureRmSqlServerRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="a893b-164">Get-AzureRmSqlServerRecommendedActions</span></span>
    + <span data-ttu-id="a893b-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="a893b-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="a893b-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="a893b-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="a893b-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="a893b-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="a893b-168">Set-AzureRmSqlDatabaseRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="a893b-168">Set-AzureRmSqlDatabaseRecommendedActionState</span></span>
    + <span data-ttu-id="a893b-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="a893b-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span></span>
    + <span data-ttu-id="a893b-170">Set-AzureRmSqlServerRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="a893b-170">Set-AzureRmSqlServerRecommendedActionState</span></span>
