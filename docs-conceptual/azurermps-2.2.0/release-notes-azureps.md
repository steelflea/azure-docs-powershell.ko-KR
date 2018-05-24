---
title: Azure PowerShell 변경 로그 | Microsoft Docs
description: Azure PowerShell에 대한 최신 릴리스의 변경 내용입니다.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: 6fe226a2525142f82b894318b0588681bff0e2ef
ms.sourcegitcommit: 5971c92cb023bdd1d71fa2ad0a3b378abfbd092a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/23/2018
---
# <a name="release-notes"></a><span data-ttu-id="b64ce-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="b64ce-103">Release notes</span></span>

<span data-ttu-id="b64ce-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="b64ce-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-220"></a><span data-ttu-id="b64ce-105">2.2.0 버전</span><span class="sxs-lookup"><span data-stu-id="b64ce-105">Version 2.2.0</span></span>
* <span data-ttu-id="b64ce-106">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="b64ce-106">Compute</span></span>
  - <span data-ttu-id="b64ce-107">AzureDiskEncryptionForLinux 확장에서 암호화 상태 쿼리 에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b64ce-107">Add support for querying encryption status from the AzureDiskEncryptionForLinux extension</span></span>
* <span data-ttu-id="b64ce-108">DataFactory</span><span class="sxs-lookup"><span data-stu-id="b64ce-108">DataFactory</span></span>
  - <span data-ttu-id="b64ce-109">활동 창을 나열하는 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="b64ce-109">Added new cmdlet for listing activity windows</span></span>
    + <span data-ttu-id="b64ce-110">Get-AzureRmDataFactoryActivityWindow</span><span class="sxs-lookup"><span data-stu-id="b64ce-110">Get-AzureRmDataFactoryActivityWindow</span></span>
* <span data-ttu-id="b64ce-111">DataLake</span><span class="sxs-lookup"><span data-stu-id="b64ce-111">DataLake</span></span>
  - <span data-ttu-id="b64ce-112">`Host` 매개 변수를 `DatabaseHost`로 변경하고, 별칭을 `Host`에 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="b64ce-112">Changed parameter `Host` to `DatabaseHost` and added alias to `Host`</span></span>
    + <span data-ttu-id="b64ce-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="b64ce-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
    + <span data-ttu-id="b64ce-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="b64ce-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
  - <span data-ttu-id="b64ce-115">ACL 및 기본 ACL 제거 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b64ce-115">Add support for ACL and Default ACL removal</span></span>
  - <span data-ttu-id="b64ce-116">파일 및 폴더에 대한 이름이 없는 권한 가져오기 및 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b64ce-116">Add support for getting and setting unnamed permissions on files and folders</span></span>
* <span data-ttu-id="b64ce-117">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b64ce-117">KeyVault</span></span>
  - <span data-ttu-id="b64ce-118">인증서 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b64ce-118">Add support for certificates</span></span>
    + <span data-ttu-id="b64ce-119">Add-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="b64ce-119">Add-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="b64ce-120">Add-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="b64ce-120">Add-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="b64ce-121">Get-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="b64ce-121">Get-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="b64ce-122">Get-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="b64ce-122">Get-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="b64ce-123">Get-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="b64ce-123">Get-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="b64ce-124">Get-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="b64ce-124">Get-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="b64ce-125">Get-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="b64ce-125">Get-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="b64ce-126">Import-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="b64ce-126">Import-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="b64ce-127">New-AzureKeyVaultCertificateAdministratorDetails</span><span class="sxs-lookup"><span data-stu-id="b64ce-127">New-AzureKeyVaultCertificateAdministratorDetails</span></span>
    + <span data-ttu-id="b64ce-128">New-AzureKeyVaultCertificateOrganizationDetails</span><span class="sxs-lookup"><span data-stu-id="b64ce-128">New-AzureKeyVaultCertificateOrganizationDetails</span></span>
    + <span data-ttu-id="b64ce-129">New-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="b64ce-129">New-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="b64ce-130">Remove-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="b64ce-130">Remove-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="b64ce-131">Remove-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="b64ce-131">Remove-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="b64ce-132">Remove-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="b64ce-132">Remove-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="b64ce-133">Remove-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="b64ce-133">Remove-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="b64ce-134">Set-AzureKeyVaultCertificateAttribute</span><span class="sxs-lookup"><span data-stu-id="b64ce-134">Set-AzureKeyVaultCertificateAttribute</span></span>
    + <span data-ttu-id="b64ce-135">Set-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="b64ce-135">Set-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="b64ce-136">Set-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="b64ce-136">Set-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="b64ce-137">Stop-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="b64ce-137">Stop-AzureKeyVaultCertificateOperation</span></span>
* <span data-ttu-id="b64ce-138">네트워크</span><span class="sxs-lookup"><span data-stu-id="b64ce-138">Network</span></span>

  - <span data-ttu-id="b64ce-139">가속화된 네트워킹을 설정/해제하기 위해 네트워크 인터페이스에 새 스위치 매개 변수(+New-AzureRmNetworkInterface -EnableAcceleratedNetworking) 추가</span><span class="sxs-lookup"><span data-stu-id="b64ce-139">New switch parameter added for network interface to enable/disable accelerated networking +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span></span>
  - <span data-ttu-id="b64ce-140">활성-활성 게이트웨이 기능 PowerShell cmdlet 사용 설정</span><span class="sxs-lookup"><span data-stu-id="b64ce-140">Enable Active-Active gateway feature PowerShell cmdlets</span></span>
    + <span data-ttu-id="b64ce-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="b64ce-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
    + <span data-ttu-id="b64ce-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="b64ce-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="b64ce-143">새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="b64ce-143">Added new cmdlet</span></span>
    + <span data-ttu-id="b64ce-144">Test-AzureRmPrivateIpAddressAvailability</span><span class="sxs-lookup"><span data-stu-id="b64ce-144">Test-AzureRmPrivateIpAddressAvailability</span></span>
* <span data-ttu-id="b64ce-145">리소스</span><span class="sxs-lookup"><span data-stu-id="b64ce-145">Resources</span></span>
  - <span data-ttu-id="b64ce-146">공급자 및 리소스 cmdlet에서 영역 지원</span><span class="sxs-lookup"><span data-stu-id="b64ce-146">Support zones in provider and resource cmdlets</span></span>
    + <span data-ttu-id="b64ce-147">Get-AzureRmProvider</span><span class="sxs-lookup"><span data-stu-id="b64ce-147">Get-AzureRmProvider</span></span>
    + <span data-ttu-id="b64ce-148">New-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="b64ce-148">New-AzureRmResource</span></span>
    + <span data-ttu-id="b64ce-149">Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="b64ce-149">Set-AzureRmResource</span></span>
* <span data-ttu-id="b64ce-150">Sql</span><span class="sxs-lookup"><span data-stu-id="b64ce-150">Sql</span></span>
  - <span data-ttu-id="b64ce-151">서버 수준의 Azure SQL 위협 검색 정책 관리에 대한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="b64ce-151">Added new cmdlets for Azure SQL threat detection policy management at server level</span></span>
    + <span data-ttu-id="b64ce-152">Get-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b64ce-152">Get-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="b64ce-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b64ce-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="b64ce-154">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b64ce-154">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
  - <span data-ttu-id="b64ce-155">Sql Azure DataWarehouse에 대한 GeoBackupPolicy 설정/해제를 지원하는 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="b64ce-155">Added new cmdlets to support enabling/disabling GeoBackupPolicy for Sql Azure DataWarehouses</span></span>
    + <span data-ttu-id="b64ce-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="b64ce-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
    + <span data-ttu-id="b64ce-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="b64ce-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
  - <span data-ttu-id="b64ce-158">Azure Sql Advisor 및 권장 작업 API에 대한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="b64ce-158">Added new cmdlets for Azure Sql Advisors and Recommended Actions APIs</span></span>
    + <span data-ttu-id="b64ce-159">Get-AzureRmSqlDatabaseAdvisor</span><span class="sxs-lookup"><span data-stu-id="b64ce-159">Get-AzureRmSqlDatabaseAdvisor</span></span>
    + <span data-ttu-id="b64ce-160">Get-AzureRmSqlElasticPoolAdvisor</span><span class="sxs-lookup"><span data-stu-id="b64ce-160">Get-AzureRmSqlElasticPoolAdvisor</span></span>
    + <span data-ttu-id="b64ce-161">Get-AzureRmSqlServerAdvisor</span><span class="sxs-lookup"><span data-stu-id="b64ce-161">Get-AzureRmSqlServerAdvisor</span></span>
    + <span data-ttu-id="b64ce-162">Get-AzureRmSqlDatabaseRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="b64ce-162">Get-AzureRmSqlDatabaseRecommendedActions</span></span>
    + <span data-ttu-id="b64ce-163">Get-AzureRmSqlElasticPoolRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="b64ce-163">Get-AzureRmSqlElasticPoolRecommendedActions</span></span>
    + <span data-ttu-id="b64ce-164">Get-AzureRmSqlServerRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="b64ce-164">Get-AzureRmSqlServerRecommendedActions</span></span>
    + <span data-ttu-id="b64ce-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="b64ce-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="b64ce-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="b64ce-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="b64ce-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="b64ce-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="b64ce-168">Set-AzureRmSqlDatabaseRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="b64ce-168">Set-AzureRmSqlDatabaseRecommendedActionState</span></span>
    + <span data-ttu-id="b64ce-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="b64ce-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span></span>
    + <span data-ttu-id="b64ce-170">Set-AzureRmSqlServerRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="b64ce-170">Set-AzureRmSqlServerRecommendedActionState</span></span>
