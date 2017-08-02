---
title: "Azure PowerShell 변경 로그 | Microsoft Docs"
description: "Azure PowerShell에 대한 최신 릴리스의 변경 내용입니다."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: 
ms.date: 07/26/2017
ms.openlocfilehash: cc2fe75f498f9043e5a4b632c144877af0143173
ms.sourcegitcommit: 20bcef86db4e4869125bb63085fcffd009c19280
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2017
---
# <a name="release-notes"></a>릴리스 정보

Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.

## <a name="20170717---version-421"></a>2017.07.17 - 버전 4.2.1
* Compute
    - VM 디스크 및 VM 디스크 스냅샷 만들기 및 업데이트 cmdlet 관련 문제 수정(링크)[https://github.com/azure/azure-powershell/issues/4309]
      - New-AzureRmDisk
      - New-AzureRmSnapshot
      - Update-AzureRmDisk
      - Update-AzureRmSnapshot
* 프로필
    - RDFE에서 비 대화형 사용자 인증 관련 문제 수정(링크)[https://github.com/Azure/azure-powershell/issues/4299]
* ServiceManagement
    - 비 대화형 사용자 인증 관련 문제 수정(링크)[https://github.com/Azure/azure-powershell/issues/4299]

## <a name="2017711---version-420"></a>2017.7.11 - 버전 4.2.0
* AnalysisServices
    * 새 데이터 평면 API 추가
        - AS 서버 로그 Export-AzureAnalysisServicesInstanceLog를 인출하는 API를 도입했습니다.
* Automation
    * New-AzureRmAutomationSchedule의 주별 및 월별 일정에 표준 시간대 값을 제대로 설정합니다.
        - 이 문제에 대한 자세한 내용은 다음에 있습니다. https://github.com/Azure/azure-powershell/issues/3043
* AzureBatch
    - 새 Get-AzureBatchJobPreparationAndReleaseTaskStatus cmdlet이 추가되었습니다.
    - Get-AzureBatchNodeFileContent 매개 변수에 바이트 범위 시작 및 종료가 추가되었습니다.
* CognitiveServices
    * Cognitive Services Management SDK 버전 1.0.0과 통합합니다.
    * 계정 이름 길이 확인 버그를 수정합니다.
* Compute
    * 이미지 디스크에 대한 저장소 계정 형식 지원:
        - Set-AzureRmImageOsDisk 및 Add-AzureRmImageDataDisk에 'StorageAccountType' 매개 변수가 추가되었습니다.
    * VMSS IP 구성에서 PrivateIP 및 PublicIP 기능:
        - New-AzureRmVmssIpConfig에 'PrivateIPAddressVersion', 'PublicIPAddressConfigurationName', 'PublicIPAddressConfigurationIdleTimeoutInMinutes', 'DnsSetting' 이름이 추가되었습니다.
        - New-AzureRmVmssIpConfig에 IPv4 또는 IPv6을 지정하는 'PrivateIPAddressVersion' 매개 변수가 추가되었습니다.
    * 성능 유지 관리 기능:
        - Restart-AzureRmVM에 'PerformMaintenance' 스위치 매개 변수가 추가되었습니다.
        - Get-AzureRmVM 상태는 지정된 VM의 성능 유지 관리 정보를 보여줍니다.
    * 가상 컴퓨터 ID 기능:
        - New-AzureRmVMConfig 및 UpdateAzureRmVM에 'IdentityType' 매개 변수가 추가되었습니다.
        - Get-AzureRmVM은 지정된 VM의 ID 정보를 보여줍니다.
    * VMSS ID 기능:
        - New-AzureRmVmssConfig에 'IdentityType' 매개 변수가 추가되었습니다.
        - Get-AzureRmVmss는 지정된 VMSS의 ID 정보를 보여줍니다.
    * VMSS 부트 진단 기능:
        - VMSS 개체의 부트 진단을 설정하는 새 cmdlet: Set-AzureRmVmssBootDiagnostics
        - New-AzureRmVmssConfig에 'BootDiagnostic' 매개 변수가 추가되었습니다.
    * VMSS LicenseType 기능:
        - New-AzureRmVmssConfig에 'LicenseType' 매개 변수가 추가되었습니다.
    * RecoveryPolicyMode 지원:
        - New-AzureRmVmssConfig에 'RecoveryPolicyMode' 매개 변수가 추가되었습니다.
    * 계산 리소스 SKU 기능:
        - 새 cmdlet인 'Get-AzureRmComputeResourceSku'는 모든 계산 리소스 SKU를 나열합니다.
* DataFactories
    * New-AzureRmDataFactoryGatewayKey를 사용하지 않습니다.
    * New-AzureRmDataFactoryGatewayAuthKey 및 Get-AzureRmDataFactoryGatewayAuthKey를 추가하여 게이트웨이 인증 주요 기능을 도입합니다.
* DataLakeAnalytics
    * 다음 명령을 통해 계산 정책 CRUD에 대한 지원을 추가합니다.
        - New-AzureRMDataLakeAnalyticsComputePolicy
        - Get-AzureRMDataLakeAnalyticsComputePolicy
        - Remove-AzureRMDataLakeAnalyticsComputePolicy
        - Update-AzureRMDataLakeAnalyticsComputePolicy
    * 되풀이 작업 및 작업 파이프라인의 도움말에 작업 관계 메타데이터에 대한 지원을 추가합니다. 다음 명령은 업데이트하거나 추가했습니다.
        - Submit-AzureRMDataLakeAnalyticsJob
        - Get-AzureRMDataLakeAnalyticsJob
        - Get-AzureRMDataLakeAnalyticsJobRecurrence
        - Get-AzureRMDataLakeAnalyticsJobPipeline
    * 작업과 카탈로그 API에 토큰 대상을 업데이트하여 Azure 리소스 그룹 대신 올바른 Data Lake 특정 대상을 사용합니다.
* DataLakeStore
    * Set-AzureRMDataLakeStoreAccount cmdlet에서 사용자관리 KeyVault 키 회전에 대한 지원을 추가했습니다.
    * 사용자 관리 KeyVault가 추가되거나 키를 회전할 경우 `enableKeyVault` 호출을 자동으로 트리거하도록 수명 품질 업데이트를 추가했습니다.
    * 작업과 카탈로그 API에 토큰 대상을 업데이트하여 Azure 리소스 그룹 대신 올바른 Data Lake 특정 대상을 사용합니다.
    * 다음 cmdlet을 사용하여 만든/추가한 파일의 크기를 제한하는 버그를 수정했습니다.
        - New-AzureRmDataLakeStoreItem
        - Add-AzureRmDataLakeStoreItemContent
* Dns
    * Get-AzureRmDnsZone에 대한 파이프 시나리오에서 버그를 수정합니다.
        - 자세한 내용은 여기에서 찾을 수 있습니다. https://github.com/Azure/azure-powershell/issues/4203
* HDInsight
    * OMS(Operations Management Suite)를 활성화/비활성화하는 지원이 추가되었습니다.
    * 새 cmdlet
        - Enable-AzureRmHDInsightOperationsManagementSuite
        - Disable-AzureRmHDInsightOperationsManagementSuite
        - Get-AzureRmHDInsightOperationsManagementSuite
    * Add-AzureRmHDInsightConfigValues에 Spark 사용자 지정 구성을 설정하는 새 매개 변수를 추가합니다.
        - Spark 1.6의 SparkDefaults 및 SparkThriftConf 매개 변수
        - Spark 2.0의 Spark2Defaults 및 Spark2ThriftConf 매개 변수
* 자세한 정보
    * 문제 #4215(변경 요청)는 Get-AzureRmLog cmdlet의 시간 창에서 15일 제한을 제거합니다. 또한 단위 테스트 이름을 사소하게 변경합니다.
    * 문제 #3957는 Get-AzureRmLog를 수정했습니다.
        - 문제 #1: 백 엔드는 각 200개의 레코드 페이지에서 레코드를 반환하며, 연속 토큰에서 다음 페이지로 연결됩니다. 200개 이상의 레코드가 있더라도 cmdlet에서는 반환되는 200개의 레코드만이 표시되었습니다. 200보다 값이 작지 않으면 MaxEvents에 설정한 값에 관계없이 발생했습니다.
        - 문제 #2: 예를 들어 설명서에 포함된 이 cmdlet에 대한 잘못된 데이터는 기본 timewindow가 1시간이었습니다.
        - 수정 사항 #1: 이제 cmdlet은 MaxEvents 또는 집합의 끝에 도달할 때까지 백 엔드에서 반환한 연속 토큰을 수행합니다.<br>MaxEvents의 기본값은 1000이며 최대 100000입니다. 1보다 작은 MaxEvents 값은 무시되고 대신 기본값이 사용됩니다. 이러한 값과 동작은 변경되지 않았으며 이제 올바르게 문서화됩니다.<br>cmdlet의 이름이 이벤트가 아닌 로그를 가리키기 때문에 MaxEvents의 별칭인 MaxRecords가 추가되었습니다.
        - 수정 #2: 설명서는 새 별칭, 올바른 시간 창, 올바른 기본, 최소 및 최대 값에 대한 정확하고 자세한 정보를 포함합니다.
* KeyVault
    * -UserPrincipalName을 Set-AzureRMKeyVaultAccessPolicy 및 Remove-AzureRMKeyVaultAccessPolicy cmdlet에 지정한 경우 디렉터리 쿼리에서 전자 메일 주소를 제거합니다.
      - 이제 cmdlet 모두에 전자 메일 주소를 적절히 쿼리하는 경우 -UserPrincipalName 매개 변수 대신 사용할 수 있는 -EmailAddress 매개 변수를 만들었습니다.  디렉터리에 있는 둘 이상의 전자 메일 주소가 일치하는 경우 cmdlet이 실패합니다.
* 네트워크
    * New-AzureRmIpsecPolicy: SALifeTimeSeconds 및 SADataSizeKilobytes는 더 이상 필수 매개 변수가 아닙니다.
        - SALifeTimeSeconds의 기본값은 27000초입니다.
        - SADataSizeKilobytes의 기본값은 102400000KB입니다.
    * SSL 정책을 사용하고 Application Gateway에서 모든 SSL 옵션 API를 나열하여 사용자 지정 암호 제품군 구성에 대한 지원을 추가했습니다.
        - 선택적 매개 변수인 -PolicyType, -PolicyName, -MinProtocolVersion, -Ciphersuite를 추가했습니다.
            - Add-AzureRmApplicationGatewaySslPolicy
            - New-AzureRmApplicationGatewaySslPolicy
            - Set-AzureRmApplicationGatewaySslPolicy
        - Get-AzureRmApplicationGatewayAvailableSslOptions(별칭: List-AzureRmApplicationGatewayAvailableSslOptions)를 추가했습니다.
        - Get-AzureRmApplicationGatewaySslPredefinedPolicy(별칭: List-AzureRmApplicationGatewaySslPredefinedPolicy)를 추가했습니다.
    * Application Gateway에서 리디렉션 지원을 추가했습니다.
        - Add-AzureRmApplicationGatewayRedirectConfiguration을 추가했습니다.
        - Get-AzureRmApplicationGatewayRedirectConfiguration을 추가했습니다.
        - New-AzureRmApplicationGatewayRedirectConfiguration을 추가했습니다.
        - Remove-AzureRmApplicationGatewayRedirectConfiguration을 추가했습니다.
        - Set-AzureRmApplicationGatewayRedirectConfiguration을 추가했습니다.
        - 선택적 매개 변수인 -RedirectConfiguration을 추가했습니다.
            - Add-AzureRmApplicationGatewayRequestRoutingRule
            - New-AzureRmApplicationGatewayRequestRoutingRule
            - Set-AzureRmApplicationGatewayRequestRoutingRule
        - 선택적 매개 변수인 -DefaultRedirectConfiguration을 추가했습니다.
            - Add-AzureRmApplicationGatewayUrlPathMapConfig
            - New-AzureRmApplicationGatewayUrlPathMapConfig
            - Set-AzureRmApplicationGatewayUrlPathMapConfig
        - 선택적 매개 변수인 -RedirectConfiguration을 추가했습니다.
            - Add-AzureRmApplicationGatewayPathRuleConfig
            - New-AzureRmApplicationGatewayPathRuleConfig
            - Set-AzureRmApplicationGatewayPathRuleConfig
        - 선택적 매개 변수인 RedirectConfigurations를 추가했습니다.
            - New-AzureRmApplicationGateway
            - Set-AzureRmApplicationGateway
    * Application Gateway에서 Azure 웹 사이트에 대한 지원을 추가했습니다.
        - New-AzureRmApplicationGatewayProbeHealthResponseMatch를 추가했습니다.
        - 선택적 매개 변수인 PickHostNameFromBackendHttpSettings, -MinServers, -Match를 추가했습니다.
            - Add-AzureRmApplicationGatewayProbeConfig
            - New-AzureRmApplicationGatewayProbeConfig
            - Set-AzureRmApplicationGatewayProbeConfig
        - 선택적 매개 변수인 PickHostNameFromBackendAddress, -AffinityCookieName, -ProbeEnabled, -Path를 추가했습니다.
            - Add-AzureRmApplicationGatewayBackendHttpSettings
            - New-AzureRmApplicationGatewayBackendHttpSettings
            - Set-AzureRmApplicationGatewayBackendHttpSettings
    * Get-AzureRmPublicIPaddress를 업데이트하여 VM 확장 집합을 통해 만든 publicipaddress 리소스를 검색합니다.
    * 현재 가상 네트워크 사용량을 가져오는 cmdlet을 추가했습니다.
        - Get-AzureRmVirtualNetworkUsageList
* 프로필
    * Import-AzureRmContext 또는 Save-AzureRmContext를 사용하는 경우에 발생하는 오류를 수정했습니다.
        - 이 문제에 대한 자세한 내용은 다음에 있습니다. https://github.com/Azure/azure-powershell/issues/3954
* RecoveryServices.SiteRecovery
    * Azure Site Recovery 작업에 대한 새 모듈을 도입합니다.
        - 모든 cmdlet은 AzureRmRecoveryServicesAsr*로 시작합니다.
* Sql
    * AzureRM.Sql에 데이터 동기화 PowerShell Cmdlet을 추가합니다.
    * 서버를 만들 때 시간 초과를 방지하는 새 REST API 버전을 사용하도록 AzureRmSqlServer cmdlet을 업데이트했습니다.
    * 이전 서버 버전(2.0)이 더 이상 존재하지 않기 때문에 사용되지 않는 서버가 cmdlet을 업그레이드합니다.
    * 새 선택적 스위치 매개 변수인 "AssignIdentity"를 New-AzureRmSqlServer 및 Set-AzureRmSqlServer cmdlet에 추가하여 SQL Server 리소스에 대한 리소스 ID를 프로비전하도록 지원합니다.
    * 매개 변수 ResourceGroupName은 이제 Get-AzureRmSqlServer에 선택 사항입니다.
        - 다음 문제에 대한 자세한 내용은 다음에 있습니다. https://github.com/Azure/azure-powershell/issues/635
* ServiceManagement ExpressRoute의 경우:
    * 다음과 같은 새 옵션을 추가하는 New-AzureBgpPeering cmdlet을 업데이트했습니다.
        - PeerAddressType: 해당 주소 제품군 형식의 BGP 피어링 만들기 위해 "IPv4" 또는 "IPv6" 값을 지정할 수 있습니다.
    * 다음과 같은 새 옵션을 추가하는 Set-AzureBgpPeering cmdlet을 업데이트했습니다.
        - PeerAddressType: 해당 주소 제품군 형식의 BGP 피어링 업데이트하기 위해 "IPv4" 또는 "IPv6" 값을 지정할 수 있습니다.
    * 다음과 같은 새 옵션을 추가하는 Remove-AzureBgpPeering cmdlet을 업데이트했습니다.
        - PeerAddressType: 해당 주소 제품군 형식의 BGP 피어링 또는 모든 항목을 제거하기 위해 "IPv4", "IPv6" 및 모든 값을 지정할 수 있습니다.

## <a name="20170607---version-410"></a>2017.06.07 - 버전 4.1.0
* AnalysisServices
    * B1, B2, S0라는 새 SKU가 추가되었습니다.
    * 스케일 업/다운 지원이 추가되었습니다.
* CognitiveServices
    * Cognitive Services 리소스를 만들 때 라이선스 규약을 자세히 표시하도록 업데이트합니다.
* Compute
    * 여러 개의 Managed Disks가 있는 가상 컴퓨터에서 Test-AzureRmVMAEMExtension을 수정합니다.
    * Set-AzureRmVMAEMExtension을 업데이트했습니다. Premium Managed Disks에 대한 캐시 정보를 추가합니다.
    * Add-AzureRmVhd: VHD의 크기 제한이 4TB로 확장되었습니다.
    * Stop-AzureRmVM: STayProvisioned 매개 변수에 대한 설명서를 분류합니다.
    * New-AzureRmDiskUpdateConfig
      * CreateOption, StorageAccountId, ImageReference, SourceUri, SourceResourceId 매개 변수는 사용되지 않습니다.
    * Set-AzureRmDiskUpdateImageReference: 사용되지 않는 cmdlet
    * New-AzureRmSnapshotUpdateConfig
      * CreateOption, StorageAccountId, ImageReference, SourceUri, SourceResourceId 매개 변수는 사용되지 않습니다.
    * Set-AzureRmSnapshotUpdateImageReference: 사용되지 않는 cmdlet
* DataLakeStore
    * Enable-AzureRmDataLakeStoreKeyVault(Enable-AdlStoreKeyVault)
      * Data Lake Store에 KeyVault 관리되는 암호화를 사용합니다.
* DevTestLabs
    * cmdlet을 업데이트하여 현재 및 업데이트된 DevTest Labs API 버전에서 작업합니다.
* IotHub
    * IoTHub cmdlet에 라우팅 지원을 추가합니다.
* KeyVault
  * KeyVault 관리되는 저장소 계정 키를 지원하는 새 cmdlet
    * Get-AzureKeyVaultManagedStorageAccount
    * Add-AzureKeyVaultManagedStorageAccount
    * Remove-AzureKeyVaultManagedStorageAccount
    * Update-AzureKeyVaultManagedStorageAccount
    * Update-AzureKeyVaultManagedStorageAccountKey
    * Get-AzureKeyVaultManagedStorageSasDefinition
    * Set-AzureKeyVaultManagedStorageSasDefinition
    * Remove-AzureKeyVaultManagedStorageSasDefinition
* 네트워크
    * Get-AzureRmNetworkUsage: 네트워크 사용량 및 용량 정보를 표시하는 새 cmdlet
    * VirtualNetworkGateways에 새 GatewaySku 옵션을 추가했습니다.
        * VpnGw1, VpnGw2, VpnGw3은 VPN Gateway에 추가된 새 SKU입니다.
    * Set-AzureRmNetworkWatcherConfigFlowLog
      * 도움말 예제를 수정했습니다.
* NotificationHubs
    * 새 API의 NotificationHubs cmdlet에 대한 투명한 업데이트
* 프로필
    * Resolve-AzureRmError
      * 서버 요청/응답 데이터를 비롯한 cmdlet에서 throw한 오류 및 예외 세부 정보를 표시하는 새 cmdlet
    * Send-Feedback
      * 로그인하지 않고 송신 피드백을 사용하도록 설정했습니다.
    * Get-AzureRmSubscription
      * CSP 구독을 검색할 때 발생하는 버그를 수정합니다.
* 리소스
    * roleassignments의 수가 1000보다 큰 경우 Get-AzureRMRoleAssignment가 잘못된 요청을 발생시키는 문제를 수정했습니다.
        * 이제 사용자는 반환되는 roleassignments가 1000보다 큰 경우에도 Get-AzureRMRoleAssignment를 사용할 수 있습니다.
* Sql
    * Restore-AzureRmSqlDatabase: 설명서 예제를 업데이트합니다.
* 저장소
    * AssignIdentity 설정 지원을 리소스 모드 저장소 계정 cmdlet에 추가합니다.
        * New-AzureRmStorageAccount
        * Set-AzureRmStorageAccount
    * 고객 키 지원을 리소스 모드 저장소 계정 cmdlet에 추가합니다.
        * Set-AzureRmStorageAccount
        * New-AzureRmStorageAccountEncryptionKeySource
* TrafficManager

    * 새로운 모니터링 설정 'MonitorIntervalInSeconds', 'MonitorTimeoutInSeconds', 'MonitorToleratedNumberOfFailures'
    * 새로운 모니터링 프로토콜 'TCP'
* ServiceManagement
    * Add-AzureVhd: VHD의 크기 제한이 4TB로 확장되었습니다.
    * New-AzureBGPPeering: LegacyMode를 지원합니다.
* Azure.Storage
    * 와일드 카드 문자를 허용하고 StorageContext 형식을 업데이트하는 매개 변수에 대한 도움말을 업데이트합니다.

## <a name="20170523---version-402"></a>2017.05.23 - 버전 4.0.2
* 프로필
    * Add-AzureRmAccount
      * AzureRM.profile의 2.x 버전을 사용하여 이전 버전과 호환성을 위해 `-EnvironmentName` 매개 변수 별칭을 추가했습니다.

## <a name="20170512---version-401"></a>2017.05.12 - 버전 4.0.1
 * 오프라인 시나리오에서 New-AzureStorageContext에 관련된 문제를 수정합니다. https://github.com/Azure/azure-powershell/issues/3939

## <a name="20170510---version-400"></a>2017.05.10 - 버전 4.0.0


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
