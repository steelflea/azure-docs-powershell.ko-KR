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
ms.openlocfilehash: 5bc3c9079cb4019bdb2255ab1f947e8ad35ae4cc
ms.sourcegitcommit: c98e3a21037ebd82936828bcb544eed902b24212
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/08/2018
ms.locfileid: "34853460"
---
# <a name="release-notes"></a>릴리스 정보

Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.

---
## <a name="620---june-2018"></a>6.2.0 - 2018년 6월
#### <a name="azurermprofile"></a>AzureRM.Profile
* Newtonsoft.Json의 버전 10.0.3이 모듈 가져오기에 로드되지 않는 문제 해결

#### <a name="azurermcompute"></a>AzureRM.Compute
* VMSS VM 업데이트 기능
    - 'Update-AzureRmVmssVM' 및 'New-AzureRmVMDataDisk' cmdlets 추가
    - 데이터 디스크를 Vmss VM에 추가할 수 있도록 지원하기 위해 VirtualMachineScaleSetVM 매개변수를 'Add-AzureRmVMDataDisk' cmdlet에 추가하였습니다.

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.8.0-preview로 업데이트되었습니다.
    - 팩터리 리포지토리 작업 구성 추가
    - QuickBooks LinkedService가 ConsumerKey 및 consumerSecret 속성을 노출하도록 업데이트됨 
    - 여러 모델 유형을 SecretBase에서 개체로 업데이트함
    - Blob 이벤트 트리거 추가

### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* 예제 출력으로 설명서 업데이트

### <a name="azurermnetwork"></a>AzureRM.Network
* Network Watcher cmdlet에서 트래픽 분석 매개 변수를 사용가능하도록 설정

#### <a name="azurermresources"></a>AzureRM.Resources
* 'Get AzureRmResource'에서 반환된 'PSResource' 개체의 'Properties' 속성의 문제 해결

#### <a name="azurermscheduler"></a>AzureRM.Scheduler
* ServiceBusQueueJob 업데이트가 새 인증 값을 설정하지 않는 문제 해결

### <a name="azurermsql"></a>AzureRM.Sql
* 옵션 LicenseType 매개 변수를 사용하여 다음 cmdlet을 업데이트
    - New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase
    - New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool
    - New-AzureRmSqlDatabaseCopy
    - New-AzureRmSqlDatabaseSecondary
    - Restore-AzureRmSqlDatabase

#### <a name="azurermwebsites"></a>AzureRM.Websites
* 'New-AzureRMWebApp'이 전략 라이브러리의 공통 알고리즘을 사용하도록 업데이트 되었습니다.

## <a name="610---may-2018"></a>6.1.0 - 2018년 5월
#### <a name="azurermprofile"></a>AzureRM.Profile
* 'Clear-AzureRmContext'를 실행하면 이전 기본 컨텍스트의 이름으로 빈 컨텍스트가 유지되어 사용자가 이전 이름으로 새 컨텍스트를 만들지 못하게 되는 문제를 수정했습니다.

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* AS에서 게이트웨이가 작업을 연결하거나 연결 해제할 수 있습니다.

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* ApiVersions, ApiReleases 및 ApiRevisions에 대한 지원이 추가됨
* ServiceFabric 백 엔드에 대한 지원 추가됨
* Application Insights 로거에 대한 지원 추가됨
* '기본' SKU를 API Management 서비스의 유효한 SKU로 인식하는 지원 추가됨
* 개인 CA가 발급한 인증서를 루트 또는 CA로 설치하는 지원 추가됨
* KeyVault 및 다중 프록시 호스트 이름을 통한 사용자 정의 SSL 인증서를 수락하는 지원 추가됨
* MSI ID에 대한 지원 추가됨
* URL을 통한 정책을 수락하는 지원 추가됨 참고: 다음 cmdlet은 이후 릴리스에서 더 이상 사용되지 않습니다.
   - Import-AzureRmApiManagementHostnameCertificate
   - New-AzureRmApiManagementHostnameConfiguration
   - Set-AzureRmApiManagementHostnames
   - Update-AzureRmApiManagementDeployment

#### <a name="azurermbatch"></a>AzureRM.Backup
* 새 cmdlet Get AzureBatchPoolNodeCounts 릴리스
* 새 cmdlet Start-AzureBatchComputeNodeServiceLogUpload 릴리스

#### <a name="azurermconsumption"></a>AzureRM.Consumption
* Expand, ResourceGroup, InstanceName, InstanceId, Tags, Top on Cmdlet Get-AzureRmConsumptionUsageDetail 등 새 매개 변수 추가

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Export-AzureRmDataLakeStoreChildItemProperties에 대한 예제 수정
* Set-AzureRmDataLakeStoreItemAclEntry에서 재귀 사례에 대한 null 매개 변수 예외 수정 
* Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry에 대한 도움말 파일 수정 

#### <a name="azurermnetwork"></a>AzureRM.Network
* 18.0.0-preview에서 19.0.0-preview로 네트워크 SDK 버전 업그레이드
* 프로토콜 구성을 만들기 위해 추가된 cmdlet
    - New-AzureRmNetworkWatcherProtocolConfiguration
* 기존 Express 경로 회로에 새 회로 연결을 추가하기 위해 추가된 cmdlet
    - Add-AzureRmExpressRouteCircuitConnectionConfig
* 기존 Express 경로 회로에서 회로 연결을 제거하기 위해 추가된 cmdlet
    - Remove-AzureRmExpressRouteCircuitConnectionConfig
* 회로 연결을 검색하기 위해 추가된 cmdlet
    - Get-AzureRmExpressRouteCircuitConnectionConfig

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* 생성된 인증서로 고정 서버 인증 사용(문제 # 5998)

#### <a name="azurermsql"></a>AzureRM.Sql
* AuditActions 또는 AuditActionGroups를 제거할 수 있도록 업데이트된 감사 cmdlet
* 'Azure 복구 서비스 자격 증명 모음을 사용하여 장기 보존 정책을 구성하면 정책이 더 이상 지원되지 않습니다. 새로운 유연 보유 정책으로 요청을 제출하십시오.'라는 메시지와 함께 명령이 실패하는 새로운 유연 보유 정책을 설정할 때 Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy의 문제 수정
* Azure SQL Database/ElasticPool Creation/Update 관련 cmdlet을 모두 업데이트하여 규모 및 계층 관련 속성에 대한 SKU 속성을 지원하는 새 데이터베이스 API를 사용합니다.
* 업데이트된 cmdlet는 다음과 같습니다. 
    - New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase
    - New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool
    - New-AzureRmSqlDatabaseCopy
    - New-AzureRmSqlDatabaseSecondary
    - Restore-AzureRmSqlDatabase

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* -Name 매개 변수를 사용할 때 -ResourceGroupName 매개 변수가 필요하도록 'Get-AzureRmTrafficManagerProfile'에 대한 매개 변수를 업데이트합니다.