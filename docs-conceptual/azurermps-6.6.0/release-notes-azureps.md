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
ms.openlocfilehash: 340c1d2d28e1b97cdd2ec98033361eb00b4302da
ms.sourcegitcommit: 72086f8d368ec84bd403e802305acfc336c08978
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/14/2018
ms.locfileid: "43018528"
---
# <a name="release-notes"></a>릴리스 정보

Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.

---
## <a name="660---july-2018"></a>6.6.0 - 2018년 7월
#### <a name="general"></a>일반
* 전체 매개 변수 형식 및 올바른 입/출력 형식을 포함하도록 모든 도움말 파일을 업데이트했습니다.

#### <a name="azurermprofile"></a>AzureRM.Profile
* Common.Strategy 라이브러리가 리소스에 대한 현재 구성이 대상 리소스와 호환되는지 유효성을 검사할 수 있도록 업데이트했습니다.
* Common.Storage에 ps1xml 형식 추가

#### <a name="azurestorage"></a>Azure.Storage
* DefaultProfile에서 저장소 컨텍스트를 가져오기 위한 지원 추가
* Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* 문제 https://github.com/Azure/azure-powershell/issues/6370 해결
    - PsApiManagementApi를 ApiContract로 좌표 이동하도록 Automapper 버그가 수정됨
* 문제 https://github.com/Azure/azure-powershell/issues/6515 해결
    - 인코딩 형식을 사용하여 오버로드하지 않도록 File.Save 버그가 수정됨
* 문제 https://github.com/Azure/azure-powershell/issues/6560 해결
    - apiId에서 패턴 예외를 수정하는 4.0.3 Nuget 버전으로 업그레이드됨

#### <a name="azurermcompute"></a>AzureRM.Compute
* PremiumLRS 저장소 계정 형식 이름 바꾸기로 인해 New-AzureRmVm에서 DiskFileParameterSet를 사용하여 vm 생성 시 실패하는 문제를 해결합니다.
* Invoke-AzureRmVMRunCommand cmdlet 수정
* Get-AzureRmAvailabilitySet를 업데이트하여 구독에서 모든 가용성 집합 리스트를 사용하도록 합니다.  (ResouceGroupName 매개 변수는 이제 선택적 요소입니다.)
* vm 선별에 가속화된 네트워크를 사용하도록 'New-AzureRmVm'의 SimpleParameterSet를 업데이트합니다.
* New-AzureRmVmss 간단 매개 변수가 사용자 지정 LB가 이미 존재할 때 vms 생성에 실패하도록 설정하여 업데이트합니다.
* New-AzureRmDisk에 대한 예제 업데이트
* 'New-AzureRmVM'에 대한 예제 추가
* Set-AzureRmVMOSDisk에 대한 설명 업데이트
* Set-AzureRmVMBginfoExtension 맞춤법 및 접두사를 수정하도록 예제 1을 업데이트합니다. 

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* ADF.Net SDK 버전을 1.1.0으로 업데이트했습니다.
* 데이터 팩터리를 공유하는 자체 호스팅된 통합 런타임을 지원합니다.
     - 새 매개 변수 -SharedIntegrationRuntimeResourceId를 Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.
     - 새로운 선택적 매개 변수 -LinkedDataFactoryName을 Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* DataPlane SDK(Microsoft.Azure.DataLake.Store) 버전을 1.1.9로 업데이트

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨

#### <a name="azurerminsights"></a>AzureRM.Insights
* 도움말 파일에서 OutputType 서식 지정 수정
* Microsoft.Azure.Management.Monitor SDK 0.19.1-preview를 사용

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Set-AzureRmKeyVaultAccessPolicy 내 파이핑 문제 해결

#### <a name="azurermnetwork"></a>AzureRM.Network
* LoadBalancerInboundNatPoolConfig cmdlet에 대한 예제가 추가되었습니다.

#### <a name="azurermresources"></a>AzureRM.Resources
* 'Get-AzureRmResource'에 대한 태그 이름 및 값을 제공할 때의 문제 해결
    - https://github.com/Azure/azure-powershell/issues/6765
* 'Set-AzureRmResource'를 사용하여 파이핑 시나리오 해결

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨
* 몇 가지 문제 해결
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a>AzureRM.Sql
* 다음 cmdlet 사용하여 서버 Advanced Threat Protection 지원을 추가합니다.
    - Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy
* 다음 cmdlet을 사용하여 취약성 평가 지원을 추가합니다.
    - Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings
    - Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline
    - Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan
* Remove-AzureRmSqlServerFirewallRule의 예제 수정
* Get-AzureSqlSyncGroupLog에서 미국이 아닌 문화권에서 날짜/시간을 올바르지 않게 다루는 문제 해결

#### <a name="azurermstorage"></a>AzureRM.Storage
* Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가
* StorageAccount cmdlet 출력을 테이블 뷰로 표시
    - Get-AzureRmStorageAccount
    - New-AzureRmStorageAccount
    - Set-AzureRmStorageAccount

#### <a name="azurermtags"></a>AzureRM.Tags
* 태그 cmdlet 도움말에서 잘못된 문을 제거합니다
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a>6.5.0 - 2018년 7월
#### <a name="azurermprofile"></a>AzureRM.Profile
* 'Get-AzureRmContextAutosaveSetting'에 대한 도움말이 업데이트됨

#### <a name="azurestorage"></a>Azure.Storage
* 쓰기 전용 SaS 토큰을 사용하는 Blob 또는 파일 업로드 지원
- Set-AzureStorageBlobContent
- Set-AzureStorageFileContent

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* 필수 속성 ResourceGroupName을 AS에 추가

#### <a name="azurermautomation"></a>AzureRM.Automation
* 도움말을 업데이트하고 'New-AzureRMAutomationSchedule'에 대한 예제 추가

#### <a name="azurermcompute"></a>AzureRM.Compute
* -Tag 매개 변수를 Update/New-AzureRmAvailabilitySet에 추가
* ‘Add-AzureRmVmssExtension’에 대한 예제 추가
* ‘Remove-AzureRmVmssExtension’에 대한 예제 추가
* ‘Set-AzureRmVMAccessExtension’에 대한 도움말 업데이트
* 기본으로 SinglePlacementGroup을 false로 설정하고 단일 배치 그룹에 VMSS를 만들 수 있는 스위치 매개 변수 'SinglePlacementGroup'을 추가하도록 New-AzureRmVmss에 대한 SimpleParameterSet을 업데이트합니다.

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* PSEventHubDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Set-AzureRmKeyVaultAccessPolicy에 대한 오류 메시지 업데이트

#### <a name="azurermlogicapp"></a>AzureRM.LogicApp
* New-AzureRmLogicApp에서 "매개 변수 집합을 확인할 수 없습니다" 오류 해결

#### <a name="azurermnetwork"></a>AzureRM.Network
* Set/Add-AzureRmVirtualNetworkPeering에 대한 여러 테넌트의 가상 네트워크에서 피어링을 사용하도록 설정
* Application Gateway에 대한 아래 cmdlet 업데이트
    - New-AzureRmApplicationGateway: EnableFIPS 플래그 및 영역 지원 추가
    - New-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가
    - Set-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가
* 최신 생성기를 사용하여 RouteTable cmdlet을 재생성

#### <a name="azurermrelay"></a>AzureRM.Relay
* markdown 파일을 업데이트하여 예제에서 매개 변수 이름 문제에 대해 해결

#### <a name="azurermresources"></a>AzureRM.Resources
* Roledefinition 및 Roleassignment cmdlet을 업데이트
    - 페이징의 일부분으로 수행하는 추가 roledefinition 호출을 제거합니다.
* Get-AzureRmRoleAssignment cmdlet 수정
    - -ExpandPrincipalGroups 명령 매개 변수 기능 수정
* 'Get-AzureRmResource'에서 '-ResourceType' 매개 변수가 대/소문자를 구분하는 문제 해결

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* top 및 skip 매개 변수가 cmdlet 목록을 나열하도록 추가
* 표준을 프리미엄 네임스페이스 마이그레이션 cmdlet에 추가
    - Start-AzureRmServiceBusMigration
    - Get-AzureRmServiceBusMigration
    - Complete-AzureRmServiceBusMigration
    - Stop-AzureRmServiceBusMigration
    - Remove-AzureRmServiceBusMigration
* PSServiceBusDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* ‘New-AzureRmServiceFabricCluster’에 대한 예제 업데이트

#### <a name="azurermsql"></a>AzureRM.Sql
* Management.Sql에 대한 새 cmdlet을 추가하여 고객이 TDE 인증서를 SQL Server 인스턴스 또는 Managed Instance에 추가할 수 있도록 허용
    - Add-AzureRmSqlServerTransparentDataEncryptionCertificate
    - Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate

#### <a name="azurermwebsites"></a>AzureRM.Websites
* `Set-AzureRmWebApp -AssignIdentity` 및 `Set-AzureRmWebAppSlot -AssignIdentity`가 false로 설정되면 사이트 개체에서 Identity 속성이 제거됩니다. 미리보기 태그도 제거됩니다.
* `Get-AzureRmWebAppMetrics`, `Get-AzureRmAppServicePlanMetrics` 예제가 업데이트됨
* `Set-AzureRmWebApp -PhpVersion`이 유효한 php 버전으로 해제 지원

## <a name="640---july-2018"></a>6.4.0 - 2018년 7월
#### <a name="general"></a>일반
* 대부분의 모듈에 대한 도움말 파일에서 OutputType 서식 지정 수정

#### <a name="azurermprofile"></a>AzureRM.Profile
* 기본 출력 형식에 추가된 Ps1Xml 특성

#### <a name="azurermcompute"></a>AzureRM.Compute
* VMSS에 대한 IP 태그 기능
    - 'New-AzureRmVmssIpTagConfig' cmdlet 추가
    - New-AzureRmVmssIpConfig에 IpTag 매개 변수가 추가됨
* VMSS에 대한 자동 OS 롤백 기능
    - New-AzureRmVmssConfig 및 Update-AzureRmVmss에 DisableAutoRollback 매개 변수가 추가됨
* Vmss에 대한 OS 업그레이드 기록 기능
    - Get-AzureRmVmss에 OSUpgradeHistory 스위치 매개 변수 추가

#### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* 다음 명령을 통해 카탈로그 액세스 제어 목록에 대한 지원을 추가합니다.
    - Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry
    - Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry
    - Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl에 대한 취소 지원 및 진행률 추적 추가
* Export-AzureRmDataLakeStoreChildItemProperties에 대한 취소 지원 추가
* 재귀 작업을 수행하는 cmdlet에 대한 디버그 메시지 플러시 수정
* DataLake cmdlet의 테스트 위치 수정

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* 목록 작업 cmdlet Get-AzureRmEventHub 및 Get-AzureRmEventHubConsumerGroup에 선택적 MaxCount 매개 변수 추가
* 새 EventHub 만드는 동안 하나 이상의 매개 변수가 필요한 New-AzureRmEventHub cmdlet 문제를 해결. 기본 매개 변수 집합을 제공.
* 선택적 매개 변수 -KeyValue를 New-AzureRmEventHubKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Get-AzureRmKeyVault -Tag 실행 시 모든 리소스가 리턴되는 문제 해결

#### <a name="azurermnetwork"></a>AzureRM.Network
* 영역 중복 VirtualNetworkGateways에 대한 새 Sku를 노출합니다.
* 기능에 대한 새 명령이 추가됨: ARM을 통한 ExpressRoute Partner APIs
    - Get- AzureRmExpressRouteCrossConnection 추가
    - Set-AzureRmExpressRouteCrossConnection 추가
    - Add-AzureRmExpressRouteCrossConnectionPeering 추가
    - Get-AzureRmExpressRouteCrossConnectionPeering 추가
    - Remove-AzureRmExpressRouteCrossConnectionPeering 추가
    - Get-AzureRMExpressRouteCrossConnectionArpTable 추가
    - Get-AzureRMExpressRouteCrossConnectionRouteTable 추가
    - Get-AzureRMExpressRouteCrossConnectionRouteTableSummary 추가

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* Get-AzureRmRecoveryServicesBackupStatus cmdlet 추가 이 cmdlet은 VM ID를 가져와서 VM이 구독에서 일부 자격 증명 모음으로 보호되는지 확인합니다. 이러한 자격 증명 모음이 존재하는 경우 cmdlet은 자격 증명 모음 세부 정보를 출력 합니다.

#### <a name="azurermresources"></a>AzureRM.Resources
* Get-AzureRmPolicyAssignment cmdlet을 다음과 같이 업데이트함.
    - 관리 그룹 수준에서 -Scope 값 리스팅에 대한 지원 추가
    - 관리 그룹 수준에서 -Scope 값을 사용하여 개별 할당값을 검색하는 것에 대한 지원 추가
    - 제어 매개 변수에 -Effective 및 -All 스위치 추가
* Get/New/Remove/Set-AzureRmPolicyDefinition cmdlet 업데이트
    - 지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가
    - 지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가
* Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlet 업데이트
    - 지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가
    - 지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가
* 'New-AzureRmResourceGroupDeployment'에서 'TemplateParameterObject'를 사용하는 경우 매개 변수에 KeyVault 비밀 참조 지원 추가
* 'New-AzureRmADAppCredential'에 대해 '-EndDate' 매개 변수가 무시되는 문제를 해결
    - https://github.com/Azure/azure-powershell/issues/6505
* 'Add-AzureRmADGroupMember'가 요청에 잘못된 URL을 사용하는 문제 해결
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* 선택적 매개 변수 -KeyValue를 New-AzureRmServiceBusKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.

#### <a name="azurermsql"></a>AzureRM.Sql
* New-AzureRmSqlDatabaseRestorePoint 도움말에서 SQLDW에 대한 사용자 정의 복원 지점 명시
* 몇 가지 cmdlet에서-ComputeGeneration 매개 변수의 설명서 업데이트

## <a name="630---june-2018"></a>6.3.0 - 2018년 6월
#### <a name="azurermprofile"></a>AzureRM.Profile
* Enable-AzureRmContextAutoSave에 대한 오류 메시지 업데이트됨
* 이전 컨텍스트 없이 'Connect-AzureRmAccount' 실행 시 각 구독에 대한 컨텍스트 생성

#### <a name="azurestorage"></a>Azure.Storage
* 도움말 파일 내 -Permissions 매개 변수에 대한 추가 정보가 추가됨

#### <a name="azurermcompute"></a>AzureRM.Compute
* 'Get-AzureRmVmDiskEncryptionStatus'가 데이터 디스크가 없는 VM에 대해 관찰된 문제를 해결 
* Compute 클라이언트 라이브러리 버전을 업데이트하여 다음 cmdlet 수정
    - Grant-AzureRmDiskAccess
    - Grant-AzureRmSnapshotAccess
    - Save-AzureRmVMImage
* 다음 cmdlet이 '작업 ID' 및 '작업 상태'를 올바르게 표시하도록 수정:
    - Start-AzureRmVM
    - Stop-AzureRmVM
    - Restart-AzureRmVM
    - Set-AzureRmVM
    - Remove-AzuerRmVM
    - Set-AzureRmVmss
    - Start-AzureRmVmssRollingOSUpgrade
    - Stop-AzureRmVmssRollingUpgrade
    - Start-AzureRmVmss
    - Restart-AzureRmVmss
    - Stop-AzureRmVmss
    - Remove-AzureRmVmss
    - ConvertTo-AzureRmVMManagedDisk
    - Revoke-AzureRmSnapshotAccess
    - Remove-AzureRmSnapshot
    - Revoke-AzureRmDiskAccess
    - Remove-AzureRmDisk
    - Remove-AzureRmContainerService
    - Remove-AzureRmAvailabilitySet

#### <a name="azurermeventgrid"></a>AzureRM.EventGrid
* Update-AzureRmEventGridSubscription cmdlet의 SubjectBeginsWith/SubjectEndsWith에 대한 ValidateNotNullOrEmpty 유효성 검사 조건을 제거하여 필요에 따라 이러한 매개 변수를 빈 문자열로 변경할 수 있습니다.

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Get-AzureRmKeyVault -Tag 실행 시 태그가 리턴되지 않는 문제 해결

#### <a name="azurermpolicyinsights"></a>AzureRM.PolicyInsights
* Policy Insights cmdlet의 공개 릴리스
    - API 버전 2018-04-04 사용
    - PolicyDefinitionReferenceId를 Get-AzureRmPolicyStateSummary의 결과 집합에 추가

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* -Vault 매개 변수를 RecoveryServices.Backup cmdlet에 추가. 전달되는 경우 이는 Set-AzureRmRecoveryServicesContext cmdlet을 재정의함.

#### <a name="azurermsql"></a>AzureRM.Sql
* Get-AzureRmSqlDatabaseExpanded에 대한 도움말 파일의 예가 업데이트됨

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* Add-AzureRmTrafficManagerEndpointConfig에대한 도움말 파일이 업데이트됨

#### <a name="azurermwebsites"></a>AzureRM.Websites
* -AssignIdentity를 사용할 때 AppSetting을 덮어쓰지 않도록 'Set-AzureRmWebApp'이 업데이트됨
* 'New-AzureRmWebAppSlot'이 AppServicePlan을 옵션 매개변수로 사용하도록 업데이트됨

## <a name="621---june-2018"></a>6.2.1 - 2018년 6월
### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* PSWorkspace 모델이 Network 형식을 매개 변수로 사용하도록 업데이트됨

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
