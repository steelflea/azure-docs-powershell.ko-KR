Azure PowerShell 4.3.1 설치 관리자: [링크](https://github.com/Azure/azure-powershell/releases/download/v4.3.1-August2017/azure-powershell.4.3.1.msi)

ARM Cmdlet용 갤러리 모듈: [링크](https://www.powershellgallery.com/packages/AzureRM/4.3.1)

서비스 관리를 위한 Legacy Cmdlet용 갤러리 모듈(RDFE): [링크](https://www.powershellgallery.com/packages/Azure/4.3.1)

## <a name="changes-in-431"></a>4.3.1의 변경 내용

- 특정 어셈블리가 서명되지 않아 모듈을 가져올 때 `could not load file or assembly` 오류가 발생하는 문제가 수정되었습니다.

## <a name="changes-in-430"></a>4.3.0의 변경 내용

* AnalysisServices
    * Set-AzureRmAnalysisServciesServer에서 버그 수정됨
        - 관리자가 제공되지 않으면 관리자가 제거됩니다.
    * New-AzureRmAnalysisServicesServer 및 Set-AzureRmAnalysisServicesServer에서 BackupBlobContainerUri가 추가됨
        - Azure Analysis Services Server 백업/복원을 위해 백업 Blob 컨테이너 설정/비활성화 사용
    * New-AzureRmAnalysisServicesServer 및 Set-AzureRmAnalysisServicesServer에서 Sku 조회가 업데이트됨
        - 하드 코딩된 Sku가 동적 조회로 변경되었습니다.
    * 서비스 주체로 로그인을 지원하는 Add-AzureAnalysisServicesAccount
* Automation
    * AutomationDSC* cmdlet이 100개가 넘는 레코드를 풀하도록 변경되었음
    * 일부 Automation cmdlet(예: Get-AzureRmAutomationVariable, Get-AzureRmAutomationJob)을 호출한 후 자세한 정보 표시 스트림 작동이 중지되는 문제가 해결되었습니다.
    * NodeConfiguration 빌드 버전 관리에 대한 지원이 StartAzureAutomationDscCompilationJob 및 ImportAzureAutomationDscNodeConfiguration에서 추가되었습니다.
    * 기존 문제에 대한 버그 수정 - 별칭 문제 해결은 #3775이며 runOn 별칭 및 HybridWorkers에 대한 지원
* Compute
    * Set-AzureRmVMAEMExtension: 새로운 프리미엄 디스크 크기에 대한 지원 추가
    * Set-AzureRmVMAEMExtension: M 시리즈에 대한 지원 추가
    * ForceUpdateTag 매개 변수를 Add-AzureRmVmssExtension에 추가
    * 기본 매개 변수를 New-AzureRmVmssIpConfig에 추가
    * EnableAcceleratedNetworking 매개 변수를 Add-AzureRmVmssNetworkInterfaceConfig에 추가
    * Set-AzureRmVmss에 인스턴스 ID 추가
    * Get-AzureRmVM -Status 출력에 MaintenanceRedeployStatus 공개
    * Get-AzureRmComputeResourceSku의 테이블 형식에 제한 및 기능 공개
* DataLakeStore
    * 문제 수정: https://github.com/Azure/azure-powershell/issues/4323
* EventHub
    * ResourceGroup 속성이 NamespaceAttributes에 추가됨
        - 'ResourceGroup'은 네임스페이스가 있는 리소스 그룹 이름을 가져옵니다.
    * 새 매개 변수 및 매개 변수 별칭으로 commandlet 업데이트됨
        - 아래 cmdlet이 AuthorizationRule 작업을 위한 네임스페이스 및 EventHub에 대한 Parametersets로 업데이트됨
        - New-AzureRmEventHubAuthorizationRule
            + 기존 NameSpace 또는 EventHub에 새 AuthorizationRule을 추가합니다.
        - Get-AzureRmEventHubAuthorizationRule
            + 기존 NameSpace 또는 EventHub에 대한 AuthorizationRule / AuthorizationRules 목록을 가져옵니다.
        - Set-AzureRmEventHubAuthorizationRule
            + EventHub NameSpace의 기존 AuthorizationRule 속성을 업데이트합니다.
        - Remove-AzureRmEventHubAuthorizationRule
            + 기존 NameSpace 또는 EventHub의 기존 AuthorizationRule을 삭제합니다.
        - New-AzureRmEventHubKey
            + 기존 NameSpace 또는 EventHub의 AuthorizationRule에 대한 새로운 주/보조 키를 생성합니다.
        - Get-AzureRmEventHubKey
            + 기존 NameSpace 또는 EventHub의 AuthorizationRule에 대한 새로운 주/보조 키를 가져옵니다.
* 네트워크
    * New-AzureRmExpressRouteCircuitPeeringConfig: IPv6 지원이 추가되었습니다. 새로운 선택적 매개 변수 추가됨
        - PeerAddressType
    * Set-AzureRmExpressRouteCircuitPeeringConfig: IPv6 지원이 추가되었습니다. 새로운 선택적 매개 변수 추가됨
        - PeerAddressType
    * Remove-AzureRmExpressRouteCircuitPeeringConfig: IPv6 지원이 추가되었습니다. 새로운 선택적 매개 변수 추가됨
        - PeerAddressType
    * 매개 변수 -ProbeEnabled가 사용되지 않는 것으로 표시됨
        - Add-AzureRmApplicationGatewayBackendHttpSettings
        - New-AzureRmApplicationGatewayBackendHttpSettings
        - Set-AzureRmApplicationGatewayBackendHttpSettings
* 프로필
    * 기본적으로 데이터 컬렉션은 사용하도록 설정되었습니다. 사용자 환경을 개선하기 위해 Microsoft에서 사용 현황 데이터를 수집합니다. 데이터는 익명이며 명령줄 인수 값을 포함하지 않습니다.
        - Disable-AzureRmDataCollection cmdlet을 사용하여 기능 해제
        - Enable-AzureRmDataCollection cmdlet을 사용하여 이 기능 설정
* 리소스
    * ARM에 요청을 보내기 전에 다음 roledefinition 및 roleassignment commandlet에 대한 범위의 유효성 검사를 위한 지원 추가
        - Get-AzureRMRoleAssignment
        - New-AzureRMRoleAssignment
        - Remove-AzureRMRoleAssignment
        - Get-AzureRMRoleDefinition
        - New-AzureRMRoleDefinition
        - Remove-AzureRMRoleDefinition
        - Set-AzureRMRoleDefinition
* ServiceBus
    * NameSpace, 큐 및 토픽의 AuthorizationRules에 대한 새로운 commandlet이 아래에 추가되었습니다. 매개 변수 집합에 따라 권한 부여 규칙 작업이 수행됩니다.
     - New-AzureRmServiceBusAuthorizationRule
       - 기존 ServiceBus NameSpace/큐/토픽에 새 AuthorizationRule을 추가합니다.
     - Get-AzureRmServiceBusAuthorizationRule
       - 기존 ServiceBus NameSpace/큐/토픽에 대한 AuthorizationRule / AuthorizationRules 목록을 가져옵니다.
     - Set-AzureRmServiceBusAuthorizationRule
       - Servicebus NameSpace/큐/토픽의 기존 AuthorizationRule 속성을 업데이트합니다.
     - New-AzureRmServiceBusKey
       - 기존 ServiceBus NameSpace/큐/토픽의 AuthorizationRule에 대한 새로운 주/보조 키를 생성합니다.
     - Get-AzureRmServiceBusKey
       - 기존 ServiceBus NameSpace/큐/토픽의 AuthorizationRule에 대한 주/보조 키를 가져옵니다.
     - Remove-AzureRmServiceBusNamespaceAuthorizationRule
       - ServiceBus NameSpace/큐/토픽의 기존 AuthorizationRule을 삭제합니다.
    * 리소스 그룹 속성이 NamespceAttributes에 추가됨
* Sql
    * 암호화 보호기 유형이 AzureKeyVault로 설정되어 있는 경우 경고를 표시하고 확인을 요구하도록 Set-AzureRmSqlServerTransparentDataEncryptionProtector 업데이트 중
    * 감사 설정을 위해 업데이트된 새 cmdlet 추가 중
        - Azure SQL 데이터베이스의 감사 설정을 가져오는 Get-AzureRmSqlDatabaseAuditing cmdlet 추가 중
        - Azure SQL 서버의 감사 설정을 가져오는 Get-AzureRmSqlServerAuditing cmdlet 추가 중
        - Azure SQL 데이터베이스의 감사 설정을 변경하는 Set-AzureRmSqlDatabaseAuditing cmdlet 추가 중
        - Azure SQL 서버의 감사 설정을 변경하는 Set-AzureRmSqlServerAuditing cmdlet 추가 중
    * 기존 감사 정책 cmdlet을 사용 중단하는 중
        - Get-AzureRmSqlDatabaseAuditingPolicy를 사용 중단하는 중
        - Get-AzureRmSqlServerAuditingPolicy를 사용 중단하는 중
        - Set-AzureRmSqlDatabaseAuditingPolicy를 사용 중단하는 중
        - Set-AzureRmSqlServerAuditingPolicy를 사용 중단하는 중
        - Use-AzureRmSqlServerAuditingPolicy를 사용 중단하는 중
        - Remove-AzureRmSqlDatabaseAuditing을 사용 중단하는 중
        - Remove-AzureRmSqlServerAuditing을 사용 중단하는 중
    * Update-AzureRmSqlSyncGroup을 위한 스키마 파일 구문 분석은 대/소문자를 구분하지 않습니다.
* 저장소
    * 리소스 모드 저장소 계정 cmdlet에 NeworkRule 지원 추가
        - New-AzureRmStorageAccount
        - Set-AzureRmStorageAccount
        - Get-AzureRmStorageAccountNetworkRuleSet
        - Update-AzureRmStorageAccountNetworkRuleSet
        - Add-AzureRmStorageAccountNetworkRule
        - Remove-AzureRmStorageAccountNetworkRule

[마지막 릴리스 이후 변경 내용](https://github.com/Azure/azure-powershell/compare/v4.2.1-July2017...v4.3.1-August2017) 보기
