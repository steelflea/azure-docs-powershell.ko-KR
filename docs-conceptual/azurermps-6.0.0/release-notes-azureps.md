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
ms.date: 5/1/2018
ms.openlocfilehash: 8515a267e80e5d1f7bb97557efa72b9e86b7b45d
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/08/2018
---
# <a name="release-notes"></a>릴리스 정보

Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.

---

## <a name="600---may-2018"></a>6.0.0 - 2018년 5월

### <a name="general"></a>일반
* 모듈의 최소 종속성이 PowerShell 5.0으로 설정되었습니다.

### <a name="azurestorage"></a>Azure.Storage
* Storage Blob 컨테이너 이름으로 지원됩니다.
    - New-AzureStorageBlobContainer
    - Remove-AzureStorageBlobContainer
    - Set-AzureStorageBlobContent
    - Get-AzureStorageBlobContent
* 일부 Storage cmdlet 실패 출력에 오류 세부 정보가 포함되지 않는 문제가 수정되었습니다.

### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* 여러 가지 주요 변경이 도입되었습니다.
    - 자세한 내용은 마이그레이션 가이드를 참조하세요.

### <a name="azurermautomation"></a>AzureRM.Automation
* 다음 cmdlet에서 사용되지 않는 'Tags' 별칭이 제거되었습니다.
    - 'Set-AzureRmAutomationRunbook'

### <a name="azurermbatch"></a>AzureRM.Backup
* 사용되지 않는 예제를 제거하도록 New-AzureBatchPool 설명서가 업데이트되었습니다.

### <a name="azurermcdn"></a>AzureRM.Cdn
* 여러 가지 주요 변경이 도입되었습니다.
    - 자세한 내용은 마이그레이션 가이드를 참조하세요.

### <a name="azurermcompute"></a>AzureRM.Compute
* 'New-AzureRmVm'과 'New-AzureRmVmss'에서 매개 변수의 자세한 정보 출력을 지원합니다.
* 'New-AzureRmVm' 및 'New-AzureRmVmss'(단순 매개 변수 집합)에서 사용자 정의 및(또는) 시스템 정의 ID를 VM에 할당하도록 지원합니다.
* VMSS 재배포 및 PerformMaintenance 기능
    -  새 스위치 매개 변수(-Redeploy 및 -PerformMaintenance)가 'Set-AzureRmVmss' 및 'Set-AzureRmVmssVM'에 추가되었습니다.
* DisableVMAgent 스위치 매개 변수가 'Set-AzureRmVMOperatingSystem' cmdlet에 추가되었습니다.
* 'New-AzureRmVm'과 'New-AzureRmVmss'(단순 매개 변수 집합)에서 'Win10' 이미지를 지원합니다.
* 'Repair-AzureRmVmssServiceFabricUpdateDomain' cmdlet이 추가되었습니다.
* 여러 가지 주요 변경이 도입되었습니다.
    - 자세한 내용은 마이그레이션 가이드를 참조하세요.
* 'Set-AzureRmVmDiskEncryptionExtension'에서 AAD 매개 변수를 선택적으로 만듭니다.

### <a name="azurermdatafactories"></a>AzureRM.DataFactories
* 다음 cmdlet에서 사용되지 않는 'Tags' 별칭이 제거되었습니다.
    - New-AzureRmDataFactory

### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.7.0-preview로 업데이트되었습니다.
    - ExecuteSSISPackage 활동에 실행 매개 변수 및 연결 관리자 속성이 추가되었습니다.
    - PostgreSql, MySql 연결된 서비스에서 서버, 데이터베이스, 스키마, 사용자 이름 및 암호 대신 전체 연결 문자열을 사용하도록 업데이트되었습니다.
    - DB2 연결된 서비스에서 스키마가 제거되었습니다.
    - Teradata 연결된 서비스에서 스키마 속성이 제거되었습니다.
    - Responsys에 대한 LinkedService, Dataset, CopySource가 추가되었습니다.

### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* 다음 cmdlet에서 사용되지 않는 'Tags' 별칭이 제거되었습니다.
    - 'New-AzureRmDataLakeAnalyticsAccount'
    - 'Set-AzureRmDataLakeAnalyticsAccount'

### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* 재귀적 Acl 변경에 대한 새 기능이 Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl에 추가되었습니다.
* 디렉터리 아래에서 콘텐츠 요약을 검색하는 새 cmdlet이 추가되었습니다.
* 디스크 사용 및 Acl 덤프를 검색하는 새 cmdlet이 추가되었습니다.
* Set-AzureRmDataLakeStoreItemAcl 부울의 반환 형식이 IEnumerable<DataLakeStoreItemAce>로 수정되었습니다.
* Set-AzureRmDataLakeStoreItemAclEntry 부울의 반환 형식이 IEnumerable<DataLakeStoreItemAce>로 수정되었습니다.
* Export-AzureRmDataLakeStoreItem, Import-AzureRmDataLakeStoreItem, Remove-AzureRmDataLakeStoreItem이 크게 변경되었습니다.

### <a name="azurermdns"></a>AzureRM.Dns
* 여러 가지 주요 변경이 도입되었습니다.
    - 자세한 내용은 마이그레이션 가이드를 참조하세요.

### <a name="azurermeventhub"></a>AzureRM.EventHub
* 누락된 예제가 있는 cmdlet에 대한 도움말이 업데이트되었습니다.

### <a name="azurerminsights"></a>AzureRM.Insights
* 여러 가지 주요 변경이 도입되었습니다.
    - 자세한 내용은 마이그레이션 가이드를 참조하세요.

### <a name="azurermiothub"></a>AzureRM.IotHub
* IotHub에서 태그 및 기본 SKU를 사용하도록 설정됩니다.

### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* 파이핑 시나리오를 지원하도록 크게 변경되었습니다.
* 추가된 새 cmdlet: Backup/Restore-AzureKeyVaultManagedStorageAccount, Backup/Restore-AzureKeyVaultCertificate, Undo-AzureKeyVaultManagedStorageSasDefinitionRemoval 및 Undo-AzureKeyVaultManagedStorageAccountRemoval

### <a name="azurermmachinelearning"></a>AzureRM.MachineLearning
* 다음 cmdlet에서 사용되지 않는 'Tags' 별칭이 제거되었습니다.
    - Update-AzureRmMlCommitmentPlan

### <a name="azurermmedia"></a>AzureRM.Media
* 다음 cmdlet에서 사용되지 않는 'Tags' 별칭이 제거되었습니다.
    - 'Set-AzureRmMediaService'

### <a name="azurermnetwork"></a>AzureRM.Network
* DDoS 보호 계획 리소스에 대한 지원이 추가되었습니다.
* 여러 가지 주요 변경이 도입되었습니다.
    - 자세한 내용은 마이그레이션 가이드를 참조하세요.

### <a name="azurermnotificationhubs"></a>AzureRM.NotificationHubs
* 여러 가지 주요 변경이 도입되었습니다.
    - 자세한 내용은 마이그레이션 가이드를 참조하세요.

### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* 여러 가지 주요 변경이 도입되었습니다.
    - 자세한 내용은 마이그레이션 가이드를 참조하세요.

### <a name="azurermprofile"></a>AzureRM.Profile
* 기본적으로 컨텍스트 자동 저장을 사용하도록 설정됩니다.
* 미국 정부를 위한 Azure 환경에 USGovernmentOperationalInsightsEndpoint 및 USGovernmentOperationalInsightsEndpointResourceId 속성이 추가되었습니다.

### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* SiteRecovery 시나리오의 인증 헤더가 수정되었습니다.

### <a name="azurermrediscache"></a>AzureRM.RedisCache
* 여러 가지 주요 변경이 도입되었습니다.
    - 자세한 내용은 마이그레이션 가이드를 참조하세요.

### <a name="azurermresources"></a>AzureRM.Resources
* Get-AzureRmRoledefinition 호출에서 사용되지 않는 -AtScopeAndBelow 매개 변수가 제거되었습니다.
* 삭제된 USers/Groups/ServicePrincipals에 대한 할당이 Get-AzureRmRoleAssignment 결과에 포함되었습니다.
* Scope 및 ResourceType에 대한 Tab 완성자가 추가되었습니다.
* ServicePrincipals를 만드는 편리한 cmdlet이 추가되었습니다.
* Get-AzureRmResource에서 Get- 및 Find- 기능이 병합되었습니다.
* 추가된 AD cmdlet:
  - Remove-AzureRmADGroupMember
  - Get-AzureRmADGroup
  - New-AzureRmADGroup
  - Remove-AzureRmADGroup
  - Remove-AzureRmADUser
  - Update-AzureRmADApplication
  - Update-AzureRmADServicePrincipal
  - Update-AzureRmADUser

### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* 기본 Linux 이미지 버전 SKU가 업데이트되었습니다.
  - NewAzureServiceFabricCluster.cs 기본 UbuntuServer1604 SKU가 업데이트되었습니다.

### <a name="azurermstorage"></a>AzureRM.Storage
* 여러 가지 주요 변경이 도입되었습니다.
    - 자세한 내용은 마이그레이션 가이드를 참조하세요.

### <a name="azurermwebsites"></a>AzureRM.Websites
* 최신 버전의 Websites SDK로 업그레이드되었습니다.
* Set-AzureRmWebApp 및 Set-AzureRmWebAppSlot에 대한 -AssignIdentity 및 -Httpsonly 속성이 추가되었습니다.
* 추가된 새 cmdlet: Get-AzureRmWebAppSnapshots 및 Restore-AzureRmWebAppSnapshot
