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
ms.date: 11/14/2017
ms.openlocfilehash: ab35cbc4ec1a0bd4e7ee40e1864bd7941f5bca87
ms.sourcegitcommit: 79dd3700b5cb4cb90b268778b482082052160093
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/14/2017
---
# <a name="release-notes"></a>릴리스 정보

Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.

## <a name="20171110-version-501"></a>2017.11.10 버전 5.0.1
* 다음과 같은 모듈에서 실행할 때 몇 가지 cmdlet이 실패하는 어셈블리 로딩 문제 해결:
    - AzureRM.ApiManagement
    - AzureRM.Backup
    - AzureRM.Backup
    - AzureRM.Compute
    - AzureRM.DataFactories
    - AzureRM.HDInsight
    - AzureRM.KeyVault
    - AzureRM.RecoveryServices
    - AzureRM.RecoveryServices.Backup
    - AzureRM.RecoveryServices.SiteRecovery
    - AzureRM.RedisCache
    - AzureRM.SiteRecovery
    - AzureRM.Sql
    - AzureRM.Storage
    - AzureRM.StreamAnalytics

## <a name="2017118---version-500"></a>2017.11.8 - 버전 5.0.0
* 참고: 이는 중요 변경 릴리스입니다. 소개된 중요 변경 사항의 전체 목록은 마이그레이션 가이드(https://aka.ms/azps-migration-guide)를 참조하세요.
* AzureRM의 모든 cmdlet는 이제 온라인 도움말을 지원합니다.
    - -Online 매개 변수와 함께 Get-Help를 실행하여 기본 인터넷 브라우저에서 온라인 도움말을 엽니다.
* AnalysisServices
    * 동기화를 위해 새로운 AsAzure REST API로 작동하도록 Synchronize-AzureAsInstance 명령 수정
* ApiManagement
    * 이 릴리스의 ApiManagement에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.
    * 문제를 해결하기 위해 cmdlet Get-AzureRmApiManagementUser 업데이트됨 https://github.com/Azure/azure-powershell/issues/4510
    * 빈 경로가 있는 Api를 만들기 위해 cmdlet New-AzureRmApiManagementApi 업데이트됨 https://github.com/Azure/azure-powershell/issues/4069
* ApplicationInsights
    * applicaiton insights 리소스를 가져오기/만들기/제거하기 위해 명령 추가
        - Get AzureRmApplicationInsights
        - Get AzureRmApplicationInsights
        - Get AzureRmApplicationInsights
    * application insights 리소스의 가격 책정/일일 상한선을 가져오기/업데이트하기 위해 명령 추가
        - Get-AzureRmApplicationInsights -IncludeDailyCap
        - Set-AzureRmApplicationInsightsPricingPlan
        - Set-AzureRmApplicationInsightsDailyCap
    * applicaiton insights 리소스의 연속 내보내기를 가져오기/만들기/업데이트하기/제거하기 위해 명령 추가
        - Get-AzureRmApplicationInsightsContinuousExport
        - Set-AzureRmApplicationInsightsContinuousExport
        - New-AzureRmApplicationInsightsContinuousExport
        - Remove-AzureRmApplicationInsightsContinuousExport
    * applicaiton insights 리소스의 api 키를 가져오기/만들기/제거하기 위해 명령 추가
        - Get-AzureRmApplicationInsightsApiKey
        - New-AzureRmApplicationInsightsApiKey
        - Remove-AzureRmApplicationInsightsApiKey
* AzureBatch
    * `New-AzureRmBatchAccount`에 새 매개 변수를 추가했습니다.
        - `PoolAllocationMode`: 배치 계정에서 풀을 만드는 데 사용하는 할당 모드입니다. 사용자의 구독에서 풀 노드를 할당하는 배치 계정을 만들려면 이를 `UserSubscription`으로 설정합니다.
        - `KeyVaultId`: 배치 계정과 연결된 Azure Key Vault의 리소스 ID입니다.
        - `KeyVaultUrl`: 배치 계정과 연결된 Azure Key Vault의 URL입니다.
    * 매개 변수를 `New-AzureBatchTask`로 업데이트했습니다.
        - `RunElevated` 스위치를 제거했습니다. `UserIdentity` 매개 변수가 `RunElevated`를 대체하기 위해 추가되었으며, 아래와 같이 `PSUserIdentity`를 구성하여 동등한 동작을 얻을 수 있습니다.
            - $autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")
            - $userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser
        - `AuthenticationTokenSettings` 매개 변수를 추가했습니다. 이 매개 변수를 사용하면 실행할 때 일괄 처리 서비스가 인증 토큰을 작업에 제공하도록 요청할 수 있어, 일괄 처리 서비스에 요청을 발행하기 위해 배치 계정 키를 작업에 전달할 필요가 없게 됩니다.
        - `ContainerSettings` 매개 변수를 추가했습니다.
            - 이 매개 변수를 사용하면 일괄 처리 서비스가 컨테이너 내의 작업을 실행하도록 요청할 수 있습니다.
        - `OutputFiles` 매개 변수를 추가했습니다.
            - 이 매개 변수를 사용하면 완료된 후 Azure Storage에 파일을 업로드하는 작업을 구성할 수 있습니다.
    * 매개 변수를 `New-AzureBatchPool`로 업데이트했습니다.
        - `UserAccounts` 매개 변수를 추가했습니다.
            - 이 매개 변수는 풀의 각 노드에서 만든 사용자 계정을 정의합니다.
        - `TargetLowPriorityComputeNodes`를 추가하고 `TargetDedicated`의 이름을 `TargetDedicatedComputeNodes`으로 변경했습니다.
            - `TargetDedicatedComputeNodes` 매개 변수에 대해 `TargetDedicated` 별칭이 만들어졌습니다.
        - `NetworkConfiguration` 매개 변수를 추가했습니다.
            - 이 매개 변수를 사용하면 풀 네트워크 설정을 구성할 수 있습니다.
    * 매개 변수를 `New-AzureBatchCertificate`로 업데이트했습니다.
        - `Password` 매개 변수가 이제 `SecureString`이 되었습니다.
    * 매개 변수를 `New-AzureBatchComputeNodeUser`로 업데이트했습니다.
        - `Password` 매개 변수가 이제 `SecureString`이 되었습니다.
    * 매개 변수를 `Set-AzureBatchComputeNodeUser`로 업데이트했습니다.
        - `Password` 매개 변수가 이제 `SecureString`이 되었습니다.
    * `Get-AzureBatchNodeFile`, `Get-AzureBatchNodeFileContent`, 및 `Remove-AzureBatchNodeFile`에서 `Name` 매개 변수의 이름이 `Path`로 변경되었습니다.
        - `Path` 매개 변수에 대해 `Name` 별칭이 만들어졌습니다.
    * 개체에 대한 변경 사항
        - 전체 목록은 일괄 처리 변경 로그를 참조하세요.
    * Azure Active Directory 기반 인증에 대한 지원이 추가되었습니다.
        - Azure Active Directory 인증을 사용하려면 `Get-AzureRmBatchAccount` cmdlet를 사용하여 `BatchAccountContext` 개체를 검색하고 이 `BatchAccountContext`를 일괄 처리 서비스 cmdlet의 `-BatchContext` 매개 변수에 제공합니다. Azure Active Directory 인증은 `PoolAllocationMode = UserSubscription`이 있는 계정에 필수입니다.
        - 기존 계정 또는 `PoolAllocationMode = BatchService`로 만든 새 계정의 경우, `Get-AzureRmBatchAccoutKeys` cmdlet를 사용하는 `BatchAccountContext` 개체를 검색하여 공유 키 인증을 계속 사용할 수 있습니다.
* Compute
    * Azure Disk Encryption 확장 명령
        - 'Set-AzureRmVmDiskEncryptionExtension'에 대한 새 매개 변수': '-EncryptFormatAll' 암호화 형식 데이터 디스크
        - 'Set-AzureRmVmDiskEncryptionExtension'에 대한 새로운 매개 변수: '-ExtensionPublisherName' 및 '-ExtensionType'이 다른 확장 버전으로 전환 허용
        - 'Disable-AzureRmVmDiskEncryption'에 대한 새로운 매개 변수: '-ExtensionPublisherName' 및 '-ExtensionType'이 다른 확장 버전으로 전환 허용
        - 'Get-AzureRmVmDiskEncryptionStatus'에 대한 새로운 매개 변수: '-ExtensionPublisherName' 및 '-ExtensionType'이 다른 확장 버전으로 전환 허용
* DataLakeAnalytics
    * 이 릴리스의 DataLakeAnalytics에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.
    * Get-AzureRmDataLakeAnalyticsAccount의 두 가지 OutputTypes 중 하나를 변경
        - 목록\<DataLakeAnalyticsAccount> 목록\<PSDataLakeAnalyticsAccountBasic>으로
        - PSDataLakeAnalyticsAccountBasic의 속성은 DataLakeAnalyticsAccount 속성의 엄격한 하위 집합입니다.
        - DataLakeAnalyticsAccount에 있는 추가 속성은 서비스에 의해 반환되지 않습니다.  따라서 이 변경 사항은 이를 정확하게 반영합니다. 이러한 추가 속성은 PSDataLakeAnalyticsAccountBasic에 여전히 있지만, Obsolete로 태그가 지정됩니다.
    * Get-AzureRmDataLakeAnalyticsJob의 두 가지 OutputTypes 중 하나를 변경
        - 목록\<JobInformation> 목록\<PSJobInformationBasic>으로
        - PSJobInformationBasic 속성은 JobInformation 속성의 엄격한 하위 집합입니다.
        - JobInformation에 있는 추가 속성은 서비스에 의해 반환되지 않습니다.  따라서 이 변경 사항은 이를 정확하게 반영합니다. 이러한 추가 속성은 PSJobInformationBasic에 여전히 있지만, Obsolete로 태그가 지정됩니다.
* DataLakeStore
    * 이 릴리스의 DataLakeStore에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.
    * Get-AzureRmDataLakeStoreAccount의 두 가지 OutputTypes 중 하나를 변경
        - 목록\<PSDataLakeStoreAccount> 목록\<PSDataLakeStoreAccountBasic>으로
        - PSDataLakeStoreAccountBasic의 속성은 PSDataLakeStoreAccount 속성의 엄격한 하위 집합입니다.
        - PSDataLakeStoreAccount에 있는 추가 속성은 서비스에 의해 반환되지 않습니다.  따라서 이 변경 사항은 이를 정확하게 반영합니다. 이러한 추가 속성은 PSDataLakeStoreAccountBasic에 여전히 있지만, Obsolete로 태그가 지정됩니다.
* Dns
    * Azure DNS의 CAA 레코드 종류에 대한 지원
       - CAA 레코드 종류에서 모든 작업 지원
* EventHub
    * 이 릴리스의 EventHub에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.
* 자세한 정보
    * 이 릴리스의 Insights에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.
* 네트워크
    * 이 릴리스의 Network에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.
    * 지정된 Azure 지역에 대해 사용 가능한 인터넷 서비스 공급자를 나열하는 cmdlet이 추가됨
        - Get-AzureRmNetworkWatcherReachabilityProvidersList
    * 지정된 위치에서 Azure 지역까지 인터넷 서비스 공급자에 대한 상대적 대기 시간 점수를 얻기 위한 cmdlet이 추가됨
        - Get-AzureRmNetworkWatcherReachabilityReport
* 프로필
    - Set-AzureRmDefault
        - 이 cmdlet을 사용하여 기본 리소스 그룹을 설정합니다.  이렇게 하면 일부 cmdlet에 대해 -ResourceGroup 매개 변수가 선택 사항이 되고 리소스 그룹이 지정되지 않은 경우 기본값이 사용됩니다.
        - ```Set-AzureRmDefault -ResourceGroupName "ExampleResourceGroup"```
        - 구독에 지정된 리소스 그룹이 있으면 이 리소스 그룹은 기본값으로 설정됩니다.  그렇지 않은 경우 리소스 그룹이 만들어진 다음 기본값으로 설정됩니다.
    - Get-AzureRmDefault
        - 이 cmdlet을 사용하여 현재 기본 리소스 그룹(및 나중의 다른 기본값)을 가져옵니다.
        - ```Get-AzureRmDefault -ResourceGroup```
    - Clear-AzureRmDefault
        - 이 cmdlet을 사용하여 현재 기본 리소스 그룹을 제거합니다.
        - ```Clear-AzureRmDefault -ResourceGroup```
    - Add-AzureRmEnvironment 및 Set-AzureRmEnvironment
        - 일괄 처리 서비스에 대한 인증 토큰을 얻을 때 사용할 Azure Batch Active Directory 대상을 지정할 수 있는 BatchAudience 매개 변수를 추가합니다.
* RecoveryServices.Backup
    * 즉시 파일 복구를 수행하기 위해 cmdlet을 추가했습니다.
        - Get-AzureRmRecoveryServicesBackupRPMountScript
        - Disable-AzureRmRecoveryServicesBackupRPMountScript
    * RecoveryServices.Backup SDK 버전을 최신 버전으로 업데이트됨
    * 테스트 실행에 필요한 모든 설정이 테스트 자체에서 지정되도록 Azure VM 워크로드에 대한 테스트를 업데이트했습니다.
    * https://github.com/Azure/azure-powershell/issues/3164 수정
* RecoveryServices.SiteRecovery
    * ASR VMware의 Azure Site Recovery에 대한 변경 사항(cmdlet은 현재 Enterprise-Enterprise, Enterprise-Azure, HyperV-Azure에 대한 작업을 지원)
        - New-AzureRmRecoveryServicesAsrPolicy
        - New-AzureRmRecoveryServicesAsrProtectedItem
        - Update-AzureRmRecoveryServicesAsrPolicy
        - Update-AzureRmRecoveryServicesAsrProtectionDirection
    * AAD 기반 자격 증명 모음에 대한 지원이 추가됨
    * VCenter 리소스를 관리하기 위해 cmdlet이 추가됨
        - Get-AzureRmRecoveryServicesAsrVCenter
        - New-AzureRmRecoveryServicesAsrVCenter
        - Remove-AzureRmRecoveryServicesAsrVCenter
        - Update-AzureRmRecoveryServicesAsrVCenter
    * 다른 cmdlet 추가
        - Get-AzureRmRecoveryServicesAsrAlertSetting
        - Get-AzureRmRecoveryServicesAsrEvent
        - New-AzureRmRecoveryServicesAsrProtectableItem
        - Set-AzureRmRecoveryServicesAsrAlertSetting
        - Start-AzureRmRecoveryServicesAsrResynchronizeReplicationJob
        - Start-AzureRmRecoveryServicesAsrSwitchProcessServerJob
        - Start-AzureRmRecoveryServicesAsrTestFailoverCleanupJob
        - Update-AzureRmRecoveryServicesAsrMobilityService
* ServiceBus
    - 이 릴리스의 ServiceBus에 대한 중요 변경 사항은 마이그레이션 가이드를 참조하세요.
* Sql
    * 목록에 대한 지원 추가 및 데이터베이스에서 비동기 updatelo 작업 취소
        - 기존 cmdlet Get-AzureRmSqlDatabaseActivity를 업데이트하여 DB updateslo를 작업 상태로 반환합니다.
        - 새 cmdlet Stop-AzureRmSqlDatabaseActivity를 추가하여 데이터베이스에서 비동기 updateslo 작업을 취소합니다.
    * 데이터베이스 및 탄성 풀에 대한 영역 중복 지원 추가
        - New-AzureRmSqlDatabase에 ZoneRedundant 스위치 매개 변수 추가
        - Set-AzureRmSqlDatabase에 ZoneRedundant 스위치 매개 변수 추가
        - New-AzureRmSqlElasticPool에 ZoneRedundant 스위치 매개 변수 추가
        - Set-AzureRmSqlElasticPool에 ZoneRedundant 스위치 매개 변수 추가
    * 서버 DNS 별칭에 대한 지원 추가
        - 서버 및 별칭 이름별 서버 DNS 별칭 또는 Azure SQL Server에 대한 서버 DNS 별칭의 목록을 가져오는 Get-AzureRmSqlServerDnsAlias cmdlet 추가
        - 지정된 Azure SQL Server에 대한 새 서버 DNS 별칭을 만드는 New-AzureRmSqlServerDnsAlias cmdlet 추가
        - 서버 DNS 별칭이 가리키는 Azure SQL Server의 업데이트를 허용하는 Set-AzurermSqlServerDnsAlias cmlet 추가
        - Azure SQL Server에 대한 새 서버 DNS 별칭을 제거하는 Remove-AzureRmSqlServerDnsAlias cmdlet 추가
* Azure.Storage
    * Azure Storage 클라이언트 라이브러리 8.5.0 및 Azure Storage DataMovement 라이브러리 0.6.3으로 업그레이드
    * 파일 공유 스냅숏 지원 기능 추가
        - Get-AzureStorageShare에 'SnapshotTime' 매개 변수 추가
        - Remove-AzureStorageShare에 'IncludeAllSnapshot' 매개 변수 추가