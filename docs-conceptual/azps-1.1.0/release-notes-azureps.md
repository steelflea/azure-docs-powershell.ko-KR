---
ms.openlocfilehash: 179d22fa065944695e4769f2698e3cabc7666b04
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342022"
---
## <a name="110---january-2019"></a>1.1.0 - 2019년 1월
#### <a name="azaccounts"></a>Az.Accounts
* Enable-AzureRmAlias에 'Local' 범위 추가

#### <a name="azcompute"></a>Az.Compute
* 이름이 Restart/Start/Stop/Remove/Set-AzVM과 Save-AzVMImage에 설정된 ID 매개 변수에서 선택 사항이 되었습니다.
* 도움말 파일의 ID에 대한 설명이 업데이트 되었습니다.
* Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* SDK 수정을 위해 데이터 평면의 SDK 버전을 1.1.14로 업데이트하세요.
    - getfilestatus 및 liststatus에 대한 음수 acesstime 및 modificationtime 수정, 비동기 취소 토큰 수정

#### <a name="azeventgrid"></a>Az.EventGrid
* 2019-01-01 API 버전을 사용하도록 업데이트되었습니다.
* 2019-01-01 API 버전에서 새 시나리오를 지원하도록 다음 cmdlet을 업데이트
    - New-AzureRmEventGridSubscription: 지정을 위한 새로운 선택적 매개 변수를 추가
        - 이벤트 Time-to-Live
        - 이벤트에 대한 최대 배달 시도
        - 배달 못한 편지의 엔드포인트입니다.
    - Update-AzureRmEventGridSubscription: 지정을 위한 새로운 선택적 매개 변수를 추가
        - 이벤트 Time-to-Live
        - 이벤트에 대한 최대 배달 시도
        - 배달 못한 편지의 엔드포인트입니다.
* New-AzureRmEventGridSubscription 및 Update-AzureRmEventGridSubscription cmdlet의 EndpointType 옵션에 새 열거형 값(즉, storageQueue 및 hybridConnection)을 추가합니다.
* 이벤트 구독을 생성 또는 업데이트할 때 사용자가 직접 조치를 취해야 할 경우 경고 메시지를 표시합니다.

#### <a name="aziothub"></a>Az.IotHub
* 최신 버전의 Azure IotHub SDK로 업데이트됨

#### <a name="azlogicapp"></a>Az.LogicApp
* 지정된 이름이 없는 모든 Get-AzLogicApp 목록

#### <a name="azresources"></a>Az.Resources
* 'Get-AzResource'에 '-ODataQuery'및 '-ResourceId' 매개 변수를 제공할 때 매개 변수 집합 문제 수정
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7875를 참조하세요.
* New/Set-AzPolicyDefinition에서 -Custom 매개 변수 처리 문제 수정
* New-AzDeployment 설명서에서 오타 수정
* 'New-AzADUser'에 '-MailNickname'매개 변수가 필수 항목으로 지정됨
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8220를 참조하세요.

#### <a name="azsignalr"></a>Az.SignalR
* Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.

#### <a name="azsql"></a>Az.Sql
* Storage 관리 클라이언트 종속성을 일반적인 SDK 구현으로 변환했습니다.

#### <a name="azstorage"></a>Az.Storage
* Sas Token, OAuth 또는 Anonymous를 사용하여 스토리지 컨텍스트의 StorageAccountName을 실제 스토리지 계정 이름으로 설정합니다.
    - New-AzStorageContext
* '-FullUri' 매개 변수를 사용하여 BLOB 스냅숏 개체의 Sas Token을 생성하고 반환된 Uri를 스냅숏 Uri로 수정합니다.
    - New-AzStorageBlobSASToken

#### <a name="azwebsites"></a>Az.Websites
* 'Get-AzDeletedWebApp'의 날짜 구문 분석 버그를 수정했습니다.
* Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.

## <a name="100---december-2018"></a>1.0.0 - 2018년 12월
### <a name="general"></a>일반

- Az 모듈 일반 공급
- 각 모듈에 대 한 온라인 도움말
- 자세한 내용과 로드맵은 [Az 알림 페이지](https://aka.ms/azps-announce)를 참조하세요.
- AzureRM에서 마이그레이션하는 것에 대한 정보는 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azaccounts"></a>Az.Accounts
- Az.Profile에서 변경
- 프로필 및 컨텍스트 형식에 대한 표 형식 수정

### <a name="azapimanagement"></a>Az.ApiManagement
- #7002에 대한 수정
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azbatch"></a>Az.Batch
- `PSComputeNode`의 새로운 `NodeAgentInformation` 속성을 통해 풀의 각 VM에서 실행 중인 Azure Batch 노드 에이전트의 버전을 확인하는 기능이 추가되었습니다.
- `PSDataDisk`에 대한 `Caching` 기본 값은 이제 `None` 대신 `ReadWrite`입니다.
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azbilling"></a>Az.Billing
- 청구, 소비 및 UsageAggregates cmdlet 결합 cmdlet에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azcognitivservices"></a>Az.CognitivServices
- New-AzureRmCognitiveServicesAccount 작업에서 사용 가능한 SkuName 및 Typem에 대한 완성자 추가
- Get-AzCognitiveServicesAccountSkus에서 GetSkusWithAccountParamSetName 매개 변수 집합을 제거

### <a name="azcontainerinstance"></a>Az.ContainerInstance
- ManagedIdentity 지원이 추가됨

### <a name="azdatalakeanalytics"></a>Az.DataLakeAnalytics
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azdatalakestore"></a>Az.DataLakeStore
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azmonitor"></a>Az.Monitor
- Az.Monitor 이름 변경 및 기타 사소한 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azkeyvault"></a>Az.KeyVault
- 출력 형식에서 사용되지 않는 'PurgeDisabled' 속성 제거

### <a name="azmachinelearning"></a>Az.MachineLearning
- Az.MachineLearningCompute 모듈의 cmdlet 포함

### <a name="azmedia"></a>Az.Media
- New-AzMediaService에서 사용되지 않는 -Tags 별칭이 제거됨

### <a name="aznetwork"></a>Az.Network
Application Gateway에서 RewriteRuleSets를 구성하는 것에 대한 지원이 추가됨
    - 추가된 새 cmdlet은 다음과 같습니다.
        - Add-AzureRmApplicationGatewayRewriteRuleSet
        - Get-AzureRmApplicationGatewayRewriteRuleSet
        - New-AzureRmApplicationGatewayRewriteRuleSet
        - Remove-AzureRmApplicationGatewayRewriteRuleSet
        - Set-AzureRmApplicationGatewayRewriteRuleSet
        - New-AzureRmApplicationGatewayRewriteRule
        - New-AzureRmApplicationGatewayRewriteRuleActionSet
        - New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration
    - 선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -RewriteRuleSet
        - New-AzureRmApplicationGateway
        - New-AzureRmApplicationGatewayRequestRoutingRule
        - Add-AzureRmApplicationGatewayRequestRoutingRule
        - New-AzureRmApplicationGatewayPathRuleConfig
        - Add-AzureRmApplicationGatewayUrlPathMapConfig
        - New-AzureRmApplicationGatewayUrlPathMapConfig로 ID를 사용하여 Application Gateway에 KeyVault 지원을 추가했습니다.
    - 선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -KeyVaultSecretId, -KeyVaultSecret
        - Add-AzApplicationGatewaySslCertificate
        - New-AzApplicationGatewaySslCertificate
        - Set-AzApplicationGatewaySslCertificate
    - New-AzApplicationGateway cmdlet이 선택적 매개 변수를 사용하도록 업데이트됨 -UserAssignedIdentity
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azoperationalinsights"></a>Az.OperationalInsights
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azprofile"></a>Az.Profile
- Az.Accounts에 모듈 이름이 변경됨

### <a name="azrecoveryservices"></a>Az.RecoveryServices
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azresources"></a>Az.Resources
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azservicefabric"></a>Az.ServiceFabric
- 일반 이름과 지문으로 지정 인증서 지원
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azsignalr"></a>Az.SIgnalR
- SIgnalR에 대한 PowerShell cmdlet에 대한 일반 공급

### <a name="azsql"></a>Az.Sql
- 위협 탐지의 cmdlet에 새로운 Data_Exfiltration 및 Unsafe_Action 검색 유형 추가
- Sql 감사 cmdlet에 대한 설명서 예제 업데이트
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azstorage"></a>Az.Storage
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azwebsites"></a>Az.Websites
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

## <a name="070---december-2018"></a>0.7.0 - 2018년 12월

### <a name="general"></a>일반

* AzureRM에서 Az 전환 예정에 대한 사소한 변경

### <a name="azcompute"></a>Az.Compute

* `New-AzVm(ss)` cmdlet에 대한 간단한 매개 변수 집합에 UltraSSD 및 갤러리 이미지에 대한 지원을 추가합니다.

### <a name="azdatalakestore"></a>Az.DataLakeStore

* ADLS 계정의 도메인의 후행 슬래시를 수정합니다.

### <a name="azfrontdoor"></a>Az.FrontDoor

* 일부 끊어진 링크 수정
    - New-AzureRmFrontDoor 및 Set-AzureRmFrontDoor 아티클에서 New-AzureRmFrontDoorHealthProbeSettingObject cmdlet 아티클에 대한 링크가 수정되었습니다.
    - New-AzureRmFrontDoorManagedRuleObject 아티클에서 New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet 아티클에 대한 링크가 수정되었습니다.

### <a name="azrecoveryservices"></a>Az.RecoveryServices

* Azure File Share 복원 작업에 클라이언트 측 유효성 검사가 추가되었습니다.
* afs 복원의 경우 storageAccountName 및 storageAccountResourceGroupName을 선택적으로 만들었습니다.

### <a name="azresources"></a>Az.Resources

* https://github.com/Azure/azure-powershell/issues/7679 에 대한 수정
    - 기본 관리자를 요청할 때 구독 범위가 제공되는 경우 Get-AzureRmRoleAssignment를 업데이트하여 구독 범위를 사용합니다.

### <a name="azsql"></a>Az.Sql

* AzureRM에서 Az 전환 예정에 대한 사소한 변경
* DotNet 코어에서 Get-AzureRmSqlDatabaseVulnerabilityAssessment를 사용하는 문제 해결
* SQL 감사 cmdlet과 관련된 도움말 메시지의 설명서가 수정되었습니다.

### <a name="azstorage"></a>Az.Storage

* New-AzureRmStorageAccount에 -EnableHierarchicalNamespace 추가
* 파일 복사 cmdlet이 -DestContext 입력이 없을 때 대상의 원본 컨텍스트를 다시 사용할 수 없는 문제 수정
    - Start-AzureStorageFileCopy
* 고정적인 웹 사이트 구성 지원
    - Enable-AzureStorageStaticWebsite
    - Disable-AzureStorageStaticWebsite

### <a name="azwebsites"></a>Az.Websites

* Set-AzureRmWebApp 및 Set-AzureRmWebAppSlot 
    - Windows 및 Linux 컨테이너 응용 프로그램에 탑재할 Azure Storage 경로를 지정하기 위해 새 매개 변수(-AzureStoragePath)가 추가되었습니다. 새 cmdlet New-AzureRmWebAppAzureStoragePath의 출력을 매개 변수로 사용하여 Azure Storage 경로를 설정합니다.

## <a name="061---november-2018"></a>0.6.1 - 2018년 11월

### <a name="azapimanagement"></a>Az.ApiManagement
* 형식 매핑 문제에 대한 종속성 업데이트

### <a name="azautomation"></a>Az.Automation
* Azure Automation cmdlet 기반 Swagger
* 업데이트 관리 cmdlet 추가
* 소스 제어 cmdlet 추가
* Remove-AzureRmAutomationHybridWorkerGroup cmdlet 추가
* DSC 노드 등록 명령 수정

### <a name="azcompute"></a>Az.Compute
* SystemAssigned ID에 대한 ID 문제 수정
* 형식 매핑 문제에 대한 종속성 업데이트

### <a name="azcontainerinstance"></a>Az.ContainerInstance
* 형식 매핑 문제에 대한 종속성 업데이트

### <a name="azmarketplaceordering"></a>Az.MarketplaceOrdering
* 마켓플레이스 cmdlet에 대한 예제 설명 업데이트

### <a name="aznetwork"></a>Az.Network
* New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError cmdlet 추가
* 지원되는 AzureFirewall 네트워크 프로토콜에 ICMP 다시 추가
* Test-AzureRmNetworkWatcherConnectivity cmdlet을 업데이트하여 대상 ID, 주소 및 포트 유효성 검사를 추가합니다. 
* VirtualNetwork 맵의 메모리 사용 문제 해결

### <a name="azrecoveryservicesbackup"></a>Az.RecoveryServices.Backup
* 보호된 파일 공유에 대한 정책을 수정하는 것에 대해 수정합니다.
* 정책 표준 시간대를 대문자로 변환했습니다.

### <a name="azrecoveryservicessiterecovery"></a>Az.RecoveryServices.SiteRecovery
* New-AzureRmRecoveryServicesAsrProtectableItem의 예제 정정
* 형식 매핑 문제에 대한 종속성 업데이트

### <a name="azrelay"></a>Az.Relay
* 선택적 매개 변수 -KeyValue를 New-AzureRmRelayKey cmdlet에 추가하여 사용자가 KeyValue를 제공할 수 있습니다.

### <a name="azresources"></a>Az.Resources
* `New-AzureRmPolicyAssignment` 및 `Set-AzureRmPolicyAssignment`의 자원 ID 관련 매개 변수에 대한 도움말 문서를 업데이트함
* -Metadata를 사용하는 New-AzureRmPolicyDefinition에 대한 예제 추가
* NetStandard의 태그 키에서 대소문자 보존을 허용하도록 수정: #7678 #7703

### <a name="azservicefabric"></a>Az.ServiceFabric
* 향후 호환성이 손상되는 변경에 대한 사용 중단 메시지 추가

### <a name="azsql"></a>Az.Sql
* Azure Sql Database Managed Instance 및 Azure Sql 관리 데이터베이스에 CRUD 작업을 위한 새 cmdlet 추가
    - Get-AzureRmSqlInstance
    - New-AzureRmSqlInstance
    - Set-AzureRmSqlInstance
    - Remove-AzureRmSqlInstance
    - Get-AzureRmSqlInstanceDatabase
    - New-AzureRmSqlInstanceDatabase
    - Restore-AzureRmSqlInstanceDatabase
    - Remove-AzureRmSqlInstanceDatabase
* 서버 또는 데이터베이스에서 확장 감사 정책 관리를 활성화했습니다.
    - 새 매개 변수(PredicateExpression)가 감사 로그 필터링을 사용하도록 추가되었습니다.
    - Cmdlet이 레거시 클라이언트 대신 SQL 클라이언트를 사용하도록 수정되었습니다.
    - Set-AzureRmSqlServerAuditing.
    - Get-AzureRmSqlServerAuditing.
    - Set-AzureRmSqlDatabaseAuditing.
    - Get-AzureRmSqlDatabaseAuditing.
* 스토리지 계정 이름 매개 변수가 설정된 Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings를 사용할 때의 문제 해결

## <a name="050---november-2018"></a>0.5.0 - 2018년 11월
#### <a name="general"></a>일반
* 많은 핵심 cmdlet에 Resource Completers를 추가하여 대화형으로 cmdlet을 호출할 때 기존 리소스 이름을 탭으로 이동할 수 있습니다.

#### <a name="azprofile"></a>Az.Profile
* ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.
* Connect-AzAccount cmdlet의 매개 변수 TenantId 이름을 Tenant로 바꾸고 TenantId의 별칭을 추가합니다
* Connect-AzAccount의 업데이트된 TenantId 설명
* 테넌트 도메인을 제공할 때 실패한 로그인에 대한 오류 메시지 수정
    - https://github.com/Azure/azure-powershell/issues/6936
* 테넌트에 구독이 없는 계정의 컨텍스트 이름 충돌 문제 수정
    - https://github.com/Azure/azure-powershell/issues/7453
* MSI를 사용할 때 DataLake 엔드포인트 문제 수정
    - https://github.com/Azure/azure-powershell/issues/7462
* 연결되지 않은 경우 'Disconnect-AzAccount'가 throw하는 문제 수정
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Get-AzCognitiveServicesAccountSkus 작업을 추가합니다.

#### <a name="azcompute"></a>Az.Compute
* Add-AzVmssVMDataDisk 및 Remove-AzVmssVMDataDisk cmdlet를 추가합니다
* Get-AzVMImage는 AutomaticOSUpgradeProperties를 표시합니다
* 수정된 SetAzVMChefExtension -BootstrapOptions 및 -JsonAttribute option 값이 json 형식으로 설정하지 않습니다.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* DataLake 패키지를 1.1.10으로 업데이트합니다.
* 기본 동시성을 다중 스레드 작업에 추가합니다.

#### <a name="azinsights"></a>Az.Insights
* 해결된 문제 #7267(자동 크기 조정 영역)
    - 열거된 매개 변수를 제대로 설정하지 않은 새 자동 크기 조정 규칙을 만드는 데 문제가 있습니다(이를 항상 기본값으로 설정함).
* 해결된 문제 # 7513[자세한 정보] Set-AzDiagnosticSetting은 설정을 생성하는 동안 범주를 명시적으로 지정해야 합니다
    - 이제 cmdlet은 생성 중에 사용할 범주를 명시적으로 표시할 필요가 없습니다. 즉, 문서화된대로 작동합니다

#### <a name="aznetwork"></a>Az.Network
* 다음 cmdlet에 대해 PeeringType을 필수 매개 변수로 변경했습니다.
    - Get-AzExpressRouteCircuitRouteTable
    - Get-AzExpressRouteCircuitARPTable
    - Get-AzExpressRouteCircuitRouteTableSummary
    - Get-AzExpressRouteCrossConnectionArpTable
    - Get-AzExpressRouteCrossConnectionRouteTable
    - Get-AzExpressRouteCrossConnectionRouteTableSummary

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* 추가된 정책 재구성 cmdlet

#### <a name="azresources"></a>Az.Resources
* https://github.com/Azure/azure-powershell/issues/7402 에 대한 수정
    - 'Get-AzResource'에 대해 '-ResourceId' 매개 변수를 사용하여 리소스 나열 허용

#### <a name="azservicebus"></a>Az.ServiceBus
* 마이그레이션 상태를 알 수 있도록 PSServiceBusMigrationConfigurationAttributes에 MigrationState 읽기 전용 속성 추가.

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Linux Vmss에 인증서 추가 수정.
* Add-AzServiceFabricClusterCertificate 수정
    - 새 인증서(Azure/service-fabric-issues#932)에서 올바른 지문을 사용.
    - 올바르게 예외 표시(Azure/service-fabric-issues#1054).
* Vmss CreateOrUpdate 작업을 시작하기 전에 'Update-AzServiceFabricDurability'를 수정하여 클러스터 구성 업데이트.

## <a name="040---october-2018"></a>0.4.0 - 2018년 10월
#### <a name="azprofile"></a>Az.Profile
* CloudShell에서 Get-AzSubscription을 사용하여 문제를 해결합니다.
* ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.

#### <a name="azcompute"></a>Az.Compute
* 'New-AzVm'에 대해 간단한 매개 변수를 사용하는 경우 가속화된 네트워킹을 설정하기 위해 새 크기가 VM 크기의 허용 목록에 추가되었습니다.
* 모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Virtual Network 규칙에 대한 지원 추가
    - Get-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 가져오거나 나열합니다.
    - Add-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 가상 네트워크 규칙을 추가합니다.
    - Set-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 지정된 가상 네트워크 규칙을 수정합니다.
    - Remove-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 삭제합니다.

#### <a name="aznetwork"></a>Az.Network
* Test-AzNetworkWatcherConnectivity cmdlet을 업데이트하고, 백 엔드에 프로토콜 값을 전달합니다.
* 모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.

#### <a name="azresources"></a>Az.Resources
* (기본 프로필에 구독이 없고 범위가 지정되지 않은 경우) 시나리오에서 의미 있는 예외를 추가하여 Get-AzRoleDefinition이 인식할 수 없는 예외를 throw하는 문제를 수정합니다. 또한 기본 매개 변수 집합을 'RoleDefinitionNameParameterSet'으로 설정합니다.

## <a name="030---october-2018"></a>0.3.0 - 2018년 10월
#### <a name="azurestorage"></a>Azure.Storage
* 대상에 메타데이터가 있을 때 Blob/파일이 메타 데이터를 복사하지 않는 문제 수정
    - Start-AzureStorageBlobCopy
    - Start-AzureStorageFileCopy
* 특정 위치의 저장소 리소스 사용을 지원하고 글로벌 저장소 리소스 사용 가져오기는 더 이상 사용되지 않는다는 경고 메시지를 추가합니다.
    - Get-AzStorageUsage
    
#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* 기존 계정이 없는 Get-AzCognitiveServicesAccountSkus를 지원합니다.

#### <a name="azcompute"></a>Az.Compute
* Get-AzVM -ResourceGroupName <rg>가 필요한 경우 50개가 넘는 결과를 반환하도록 수정
* 'SimpleParameterSet' 예제가 New-AzVmss cmdlet 도움말에 추가됨
* Azure Disk Encryption 진행률 메시지의 오타를 수정

#### <a name="azdatafactoryv2"></a>Az.DataFactoryV2
* ADF.Net SDK 버전을 2.3.0으로 업데이트

#### <a name="aznetwork"></a>Az.Network
* NetworkProfile 기능 추가 추가된 새 cmdlet은 다음과 같습니다.
    - Get-AzNetworkProfile
    - New-AzNetworkProfile
    - Remove-AzNetworkProfile
    - Set-AzNetworkProfile
    - New-AzContainerNicConfig
    - New-AzContainerNicConfigIpConfig
* 서브넷 모델에 서비스 연결 링크 추가
* New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap cmdlet 추가
* Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig cmdlet 추가

#### <a name="azrediscache"></a>Az.RedisCache
* 모든 문자열을 Size 매개 변수로 진행되도록 허용 PSArgumentCompleter 팝업에 P5 추가

#### <a name="azresources"></a>Az.Resources
* -Mode 매개 변수를 Set-AzPolicyDefinition에 추가
* 사용자가 포함된 Origin 작업에서 Get-AzProviderOperation commandlet 버그 수정

#### <a name="azsql"></a>Az.Sql
* 일부 백업 cmdlet이 현재 azure 구독을 인식하지 않는 문제 해결

#### <a name="azwebsites"></a>Az.Websites
* 새 cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - 컨테이너 지속적인 배포 Webhook URL을 가져옵니다.
* 새 cmdlet New-AzWebAppContainerPSSession 및 Enter-WebAppContainerPSSession -  windows 컨테이너 앱에 PowerShell 원격 세션을 시작합니다.

## <a name="020---september-2018"></a>0.2.0 - 2018년 9월
 최초 릴리스