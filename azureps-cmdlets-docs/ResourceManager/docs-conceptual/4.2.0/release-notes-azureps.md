---
title: "Azure PowerShell 변경 로그 | Microsoft Docs"
description: "Azure PowerShell에 대한 최신 릴리스의 변경 내용입니다."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-resource-manager
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: 
ms.date: 05/18/2017
ms.openlocfilehash: 5c8fa2a5a8f94cd24b66f42c237749a7b89af3b3
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/29/2017
---
# <a name="release-notes"></a>릴리스 정보

Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.

## <a name="version-400"></a>버전 4.0.0

* 이 릴리스에는 주요 변경 내용인 포함됩니다. 변경 세부 정보 및 기존 스크립트에 미치는 영향에 대해서는 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.
* ApiManagement
  - New-AzureRmApiManagementGroup에서 기존 그룹을 구성하기 위한 지원이 추가되었습니다.
* 결제
  - 새 Cmdlet Get-AzureRmBillingPeriod
    + 구독의 Azure 청구 기간을 검색하기 위한 cmdlet입니다.
  - Cmdlet Get-AzureRmBillingInvoice 업데이트
  - 새 속성 BillingPeriodNames
  - 목록 보기에서 출력
* 계산
  - 프리미엄 Managed Disks를 지원하도록 Set-AzureRmVMAEMExtension 및 Test-AzureRmVMAEMExtension cmdlet이 업데이트되었습니다.
  - IaaS VM에 대한 암호화 설정 백업 및 실패 시 복원
  - ChefServiceInterval 옵션 이름이 ChefDaemonInterval로 바뀌었습니다. 그렇지만 이전 이름도 계속 사용할 수 있습니다.
  - PS VM 개체에서 중복된 DataDiskNames 및 NetworkInterfaceIDs 속성을 제거합니다.
  - DataDiskNames 및 NetworkInterfaceIDs 매개 변수를 Remove-AzureRmVMDataDisk 및 Remove-AzureRmVMNetworkInterface에서 각각 옵션으로 지정되었습니다.
  - Get cmdlet이 목록 개체를 반환하는 경우 Get cmdlet의 파이핑 문제가 해결되었습니다.
  - RDFE cmdlet과 충돌하는 Cmdlet 이름이 바뀌었습니다. 자세한 내용은 문제 https://github.com/Azure/azure-powershell/issues/2917을 참조하세요.
    + `New-AzureVMSqlServerAutoBackupConfig`는 `New-AzureRmVMSqlServerAutoBackupConfig`로 이름이 변경되었습니다.
    + `New-AzureVMSqlServerAutoPatchingConfig`는 `New-AzureRmVMSqlServerAutoPatchingConfig`로 이름이 변경되었습니다.
    + `New-AzureVMSqlServerKeyVaultCredentialConfig`는 `New-AzureRmVMSqlServerKeyVaultCredentialConfig`로 이름이 변경되었습니다.
* Consumption
  - 새 Cmdlet Get-AzureRmConsumptionUsageDetail
    + 구독의 사용량 세부 정보를 검색하기 위한 cmdlet입니다.
* ContainerRegistry
  - Azure Container Registry에 대한 PowerShell cmdlet이 추가되었습니다.
    + New-AzureRmContainerRegistry
    + Get-AzureRmContainerRegistry
    + Update-AzureRmContainerRegistry
    + Remove-AzureRmContainerRegistry
    + Get-AzureRmContainerRegistryCredential
    + Update-AzureRmContainerRegistryCredential
    + Test-AzureRmContainerRegistryNameAvailability
* DataLakeAnalytics
  - 카탈로그 패키지 가져오기 및 나열에 대한 지원 추가
  - 좀 더 높은 수준의 상위 항목에서 다음 카탈로그 항목을 나열하기 위한 지원 추가
    + 테이블
    + TVF
    + 보기
    + 통계
* DataLakeStore
  - `Import-AzureRMDataLakeStoreItem` 및 `Export-AzureRMDataLakeStoreItem`의 경우 성능 향상을 위해 추적 로깅이 기본적으로 사용되지 않도록 설정되어 있습니다. 추적 로깅이 필요한 경우 `-DiagnosticLogLevel` 및 `-DiagnosticLogPath` 매개 변수를 사용하세요.
  - ADLS에 많은 수의 작은 파일을 업로드하는 경우 때때로 PowerShell이 충돌하도록 하는 버그를 수정했습니다.
* EventHub
  - 버그 수정:
    + Set-AzureRmEventHubNamespace cmdlet 오류에 대한 수정 - 'Tier'가 'SkuName'이어야 하는 경우 null로 지정할 수 없습니다.
    + Set-AzureRmEventHub - EventHub를 업데이트하는 동안 '개체 참조가 개체의 인스턴스로 설정되지 않았습니다.' 오류 수정
* 자세한 정보
  - Add-AzureRm*AlertRule
    + 단일 개체 newResource, statusCode, requestId를 반환합니다.
  - Get-AzureRmAlertRule
    + 이제 출력은 단일 개체로 간주되지 않고 열거됩니다. 해당 형식은 변경되지 않았으므로 여전히 목록입니다.
  - Remove-AzureRmAlertRule
    + statusCode는 요청에 의해 반환된 상태 코드(항상 정상임)를 따릅니다.
  - Add-AzureRmAutoscaleSetting
    + 이제 statusCode, requestId 및 새로 생성/업데이트된 리소스를 포함하는 단일 개체(이전처럼 목록이 아님)를 반환합니다.
    + 상태 코드는 요청에 의해 반환된 상태(항상 정상임)를 따릅니다.
  - New-AzureRmAutoscaleRule
    + 매개 변수 ScaleActionType이 확장되었으며 이제 값 ChangeCount, PercentChangeCount, ExactCount를 수신합니다.
  - Remove-AzureRmAutoscaleSetting
    + 출력의 statusCode는 요청에 의해 반환된 statusCode를 따릅니다. 이 코드가 이전에는 항상 정상이었습니다.
  - Get-AzureRMLogProfile
    + 이제 출력이 열거됩니다. 이전에는 단일 개체로 간주되었습니다. 출력의 형식은 이전처럼 목록으로 유지됩니다.
  - Remove-AzureRmLogProfile
    + PassThru 매개 변수가 구현되었습니다.
  - Metrics API
    + 이 SDK는 이제 MDM에서 메트릭을 검색합니다.
  - Get-AzureRmMetricDefinition
    + 출력은 여전히 목록이지만 목록 구조가 변경되었습니다.
  - Get-AzureRmMetric
    + 호출이 변경되었습니다. 새 구문: Get-AzureRmMetric ResourceId [MetricNames [TimeGrain] [AggregationType] [StartTime] [EndTime]] [DetailedOutput]
    + 출력은 목록이며 해당 요소의 구조가 변경되었습니다.
* KeyVault
  - KeyVault 비밀에 대한 백업/복원 지원 추가
    + 비밀을 백업 및 복원할 수 있으며 키에 대해 현재 지원되는 기능과 일치합니다.

  - 키 및 비밀에 대한 백업 cmdlet은 이제 해당 개체를 입력 매개 변수로 수락합니다.
    + 호출자는 검색 및 백업 작업을 연쇄적으로 진행할 수 있음: Get-AzureKeyVaultKey -VaultName myVault -Name myKey | Backup-AzureKeyVaultKey

  - 이제 백업 cmdlet은 기존 파일을 덮어쓰기 위한 -Force 스위치를 지원합니다.
    + 기존 파일을 덮어쓰려고 해도 더 이상 오류가 throw되지 않으며 대신, 사용자에게 진행 방법을 선택하라는 메시지가 표시됩니다.
* LogicApp
  - 교환 컨트롤 번호 재해 복구 cmdlet에 대한 새 매개 변수:
    + 옵션 - 관련 컨트롤 번호를 지정하기 위한 AgreementType 매개 변수("X12" 또는 "Edifact")
* MachineLearning
  - 새 버전의 Azure Machine Learning .Net SDK를 사용하고 새로운 cmdlet을 추가합니다.
    + Add-AzureRmMlWebServiceRegionalProperty
  - 도움말 텍스트의 일부 표현이 수정되었습니다.
* 네트워크
  - Test-AzureRmNetworkWatcherConnectivity cmdlet이 추가되었습니다.
    + 지정된 원본 VM 및 대상에 대한 연결 정보를 반환합니다.
    + 원본 및 대상 간에 연결을 설정할 수 없는 경우 이 cmdlet은 문제에 대한 세부 정보를 반환합니다.
* 프로필
  - `Send-Feedback' cmdlet 추가: 사용자는 Azure PowerShell 팀에 피드백을 전송하는 일련의 메시지를 시작할 수 있습니다.
  - 다음 별칭은 Azure 모듈의 기존 cmdlet 이름과 충돌하므로 제거되었습니다.
    + `Enable-AzureDataCollection`(`Enable-AzureRmDataCollection`에서 지원)
    + `Disable-AzureDataCollection`(`Disable-AzureRmDataCollection`에서 지원)
* 릴레이
  - 사용자가 모든 Azure Relay 리소스를 만들고 관리할 수 있도록 하는 Azure Relay에 대한 cmdlet을 추가합니다.
    + `New-AzureRmRelayNamespace`
    + `Get-AzureRmRelayNamespace`
    + `Set-AzureRmRelayNamespace`
    + `Remove-AzureRmRelayNamespace`
    + `New-AzureRmWcfRelay`
    + `Get-AzureRmWcfRelay`
    + `Set-AzureRmWcfRelay`
    + `Remove-AzureRmWcfRelay`
    + `New-AzureRmRelayHybridConnection`
    + `Get-AzureRmRelayHybridConnection`
    + `Set-AzureRmRelayHybridConnection`
    + `Remove-AzureRmRelayHybridConnection`
    + `Test-AzureRmRelayName`
    + `Get-AzureRmRelayOperation`
    + `New-AzureRmRelayKey`
    + `Get-AzureRmRelayKey`
    + `New-AzureRmRelayAuthorizationRule`
    + `Get-AzureRmRelayAuthorizationRule`
    + `Set-AzureRmRelayAuthorizationRule`
    + `Remove-AzureRmRelayAuthorizationRule`
* 리소스
  - New-AzureRmResourceGroupDeployment에 대한 리소스 그룹 간 배포를 지원합니다.
    + 이제 사용자는 중첩 배포를 사용하여 다른 리소스 그룹에 배포할 수 있습니다.
* ServiceBus

  - 버그 수정: ServiceBus 큐 개체 속성 값이 null로 설정되었으며 해당 개체는 큐 업데이트를 위해 Set-AzureRmServiceBusQueue cmdlet에서 입력 매개 변수로 사용됩니다.
   - 영향 받는 속성은 LockDuration, EntityAvailabilityStatus, DuplicateDetectionHistoryTimeWindow, MaxDeliveryCount 및 MessageCount입니다.
* ServiceFabric

  - Service Fabric에 대한 cmdlet이 추가되었습니다.
    + Add-AzureRmServiceFabricApplicationCertificate       응용 프로그램 인증서로 사용할 인증서 추가
    + Add-AzureRmServiceFabricClientCertificate       클라이언트 인증을 위해 일반 이름 또는 지문을 클러스터 설정에 추가
    + Add-AzureRmServiceFabricClusterCertificate       기존 인증서를 롤오버하기 위해 클러스터에 보조 클러스터 인증서 추가
    + Add-AzureRmServiceFabricNodes       클러스터에 특정 노드 형식의 노드/VM 추가
    + Add-AzureRmServiceFabricNodeType       기존 클러스터에 노드 형식/VM 추가
    + Get-AzureRmServiceFabricCluster       클러스터 리소스의 세부 정보 가져오기
    + New-AzureRmServiceFabricCluster 새 ServiceFabric 클러스터를 만들기 이 명령은 다양한 시나리오에 적용되는 여러 오버로드를 제공합니다.
    + Remove-AzureRmServiceFabricClientCertificate       클러스터에 액세스하는 데 사용되는 클라이언트 인증서 제거
    + Remove-AzureRmServiceFabricClusterCertificate       클러스터 보안에 사용되지 않도록 클라이언트 인증서 제거
    + Remove-AzureRmServiceFabricNodes       클러스터에서 특정 노드 형식의 노드 제거
    + Remove-AzureRmServiceFabricNodeType       클러스터에서 노드 형식 제거
    + Remove-AzureRmServiceFabricSettings       클러스터에서 하나 이상의 ServiceFabric 설정 제거
    + Set-AzureRmServiceFabricSettings       클러스터의 하나 이상 ServiceFabric 설정 추가 또는 업데이트
    + Set-AzureRmServiceFabricUpgradeType       클러스터의 ServiceFabric 업그레이드 집합 변경
    + Update-AzureRmServiceFabricDurability       클러스터의 지속성 계층 변경
    + Update-AzureRmServiceFabricReliability       클러스터의 안정성 계층 변경
* Sql
  - New-AzureRmSqlDatabase에 -SampleName 매개 변수 추가
  - 장애 조치 그룹 cmdlet에 대한 업데이트
  - 'Tag' 매개 변수 제거
  - Remove-AzureRmSqlDatabaseFailoverGroup cmdlet에서 'PartnerResourceGroupName' 및 'PartnerServerName' 매개 변수 제거
  - New- 및 Set- cmdlet에 'GracePeriodWithDataLossHours' 매개 변수가 추가되고 결과적으로 'GracePeriodWithDataLossHour' 대신 사용됨
  - 설명서가 보완되고 업데이트되었습니다.
  - 반환된 개체의 서식 변경, 필드가 항상 채워지지는 않던 일부 버그 수정
  - 장애 조치(Failover) 그룹 개체에 'DatabaseNames' 및 'PartnerLocation' 속성 추가
  - Switch- cmdlet에서 작업이 완료되기를 기다리지 않고 즉시 반환되도록 하는 버그 수정
  - 높은 유예 기간 값이 사용되는 정수 오버플로 버그 수정
  - 더 낮은 값이 제공될 경우 유예 기간을 최소값인 1시간으로 조정
  - Set-AzureRmSqlDatabaseThreatDetectionPolicy cmdlet 및 Set-AzureRmSqlServerThreatDetectionPolicy cmdlet의 "ExcludedDetectionType" 매개 변수에 대해 허용되는 값 중에서 "Usage_Anomaly" 제거
* 저장소
  - SRP SDK를 6.3.0으로 업그레이드
  - New/Set-AzureRmStorageAccount: EnableHttpsTrafficOnly를 지원하기 위한 새 매개 변수 추가
  - New/Set/Get-AzureRmStorageAccount: 반환된 저장소 계정에 새 특성인 EnableHttpsTrafficOnly가 포함되어 있음
* Azure.Storage
  - Azure Storage 클라이언트 라이브러리 8.1.1 및 Azure Storage DataMovement 라이브러리 0.5.1로 업그레이드
  - Blob 증분 복사 기능을 지원하기 위한 새 cmdlet 추가
