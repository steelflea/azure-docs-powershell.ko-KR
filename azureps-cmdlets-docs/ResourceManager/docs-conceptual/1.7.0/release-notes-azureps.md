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
ms.date: 05/18/2017
ms.openlocfilehash: 0a3f152751fee569d3ac5fba6bcff8c1737f7b8c
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/29/2017
---
# <a name="release-notes"></a>릴리스 정보

Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.

## <a name="version-170"></a>1.7.0 버전

* **모든 cmdlet에 대해 -Force, -Confirm 및 $ConfirmPreference 매개 변수의 동작을 변경합니다. PowerShell 지침에 따라 이 구현을 변경하고 있습니다. 대부분의 cmdlet에 대해 Force 매개 변수를 제거하고 ShouldProcess 프롬프트를 건너뛰므로 사용자가 PowerShell 스크립트에 '-Confirm: $ false' 매개 변수를 포함해야 합니다.** 이 변경 내용은 다음 문제를 해결합니다.
  - –WhatIf 기능의 올바른 구현 - 사용자가 실제로 변경하지 않고 cmdlet 또는 스크립트의 영향을 결정할 수 있게 합니다.
  - 세션 전체 $ConfirmPreference를 사용하여 메시지 표시에 대한 컨트롤 - 사용자에게 잠재적 변경의 영향을 기반으로 한 메시지가 표시됩니다(cmdlet의 ConfirmImpact 설정에서 보고됨).
  - -Confirm 매개 변수를 사용하여 확인 메시지 표시에 대한 cmdlet 관련 컨트롤
  - cmdlet 간에 일관된 ShouldContinue 및 -Force 매개 변수 사용 - 변경의 특수한 특성(예: 숨김 파일 삭제)으로 인해 사용자에게 묻는 메시지를 표시해야 하는 작업에만 사용
  - 다른 PowerShell cmdlet과의 일관성 - 다른 cmdlet의 PowerShell 스크립팅 지식을 Azure PowerShell cmdlet에 즉시 적용할 수 있습니다.

***모든 상황에서 모든 프롬프트를 자동으로 건너뜁니다.* Azure PowerShell cmdlet에서 사용자가 다음 두 매개 변수를 제공해야 합니다.**
```powershell
My-CmdletWithConfirmation –Confirm:$false -Force
```
* Azure Compute
  - Set-AzureRmVMADDomainExtension
  - Get-AzureRmVMADDomainExtension
  - Restart-AzureVM에 대한 -Redeploy 매개 변수
  - Move-AzureService, Move-AzureStorageAccount 및 Move-AzureVirtualNetwork에 대한 -Validate 매개 변수
  - 확장 cmdlet의 name 및 version 매개 변수는 이전과 마찬가지로 선택 사항입니다.
  - New-AzureVM은 VM 개체에서 라이선스 유형을 가져올 수 있습니다.
* Azure 저장소
  - Tags 매개 변수를 Tag로 변경 및 매개 변수 별칭 Tags 추가
    + New-AzureRmStorageAccount
    + Set-AzureRmStorageAccount
* Azure 네트워크
  - 가상 네트워크 피어링에 대한 새 cmdlet 추가
* Azure Redis Cache
  - Reset-AzureRmRedisCache에 대한 새 cmdlet 추가
  - Export-AzureRmRedisCache에 대한 새 cmdlet 추가
  - Import-AzureRmRedisCache에 대한 새 cmdlet 추가
  - vNet에 대한 매개 변수 변경을 포함하도록 New-AzureRmRedisCache cmdlet 수정
* Azure SQL DB 백업/복원
  - LTR(장기 보존) 백업 기능에 대한 cmdlet
  - Get-AzureRmSqlServerBackupLongTermRetentionVault
  - Get-AzureRmSqlDatabaseBackupLongTermRetentionPolicy
  - Set-AzureRmSqlServerBackupLongTermRetentionVault
  - Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy
  - Restore-AzureRmSqlDatabase에서 이제는 삭제된 데이터베이스의 특정 시점 복원 지원
  - Restore-AzureRmSqlDatabase에서 이제는 장기 보존 백업의 복원 지원
* Azure LogicApp
  - LogicApp 통합 계정 cmdlet 추가.
  - Get-AzureRmIntegrationAccountAgreement
  - Get-AzureRmIntegrationAccountCallbackUrl
  - Get-AzureRmIntegrationAccountCertificate
  - Get-AzureRmIntegrationAccount
  - Get-AzureRmIntegrationAccountMap
  - Get-AzureRmIntegrationAccountPartner
  - Get-AzureRmIntegrationAccountSchema
  - New-AzureRmIntegrationAccountAgreement
  - New-AzureRmIntegrationAccountCertificate
  - New-AzureRmIntegrationAccount
  - New-AzureRmIntegrationAccountMap
  - New-AzureRmIntegrationAccountPartner
  - New-AzureRmIntegrationAccountSchema
  - Remove-AzureRmIntegrationAccountAgreement
  - Remove-AzureRmIntegrationAccountCertificate
  - Remove-AzureRmIntegrationAccount
  - Remove-AzureRmIntegrationAccountMap
  - Remove-AzureRmIntegrationAccountPartner
  - Remove-AzureRmIntegrationAccountSchema
  - Set-AzureRmIntegrationAccountAgreement
  - Set-AzureRmIntegrationAccountCertificate
  - Set-AzureRmIntegrationAccount
  - Set-AzureRmIntegrationAccountMap
  - Set-AzureRmIntegrationAccountPartner
  - Set-AzureRmIntegrationAccountSchema
* Azure Data Lake Store
  - 파일과 폴더의 업로드 및 다운로드 성능을 크게 향상.
  - 다운로드에 대한 매개 변수 이름을 약간 변경했고, 업로드에 대한 새로운 두 매개 변수를 포함했습니다.
    + NumThreads -> PerFileThreadCount - 단일 파일에서 사용할 스레드 수를 나타내는 데 사용됩니다.
    + ConcurrentFileCount - 폴더 업로드/다운로드를 위해 병렬로 업로드/다운로드할 파일 수를 나타내는 데 사용됩니다.
  - 기본 스레딩 값이 이제 대부분의 파일 크기에 대한 처리량을 향상시키도록 설계되었습니다. 성능이 원하는 대로 수행되지 않으면 위의 값을 수정하여 요구 사항을 충족할 수 있습니다.
* Azure 데이터 레이크 분석
  - Get-AzureRMDataLakeAnalyticsDataSource가 이제 인수 없이 호출될 때 모든 데이터 원본 반환.
  - 이 변경은 cmdlet에서 데이터 원본 형식 매개 변수도 제거합니다.
  - 이 변경으로 인해 다음 속성을 사용하여 목록 작업에 대해 새 개체를 반환합니다.
    + Type - 데이터 원본 형식입니다.
    + Name - 데이터 원본 이름입니다.
    + IsDefault - 계정에 대한 기본 데이터 원본인 경우 true로 설정합니다.
  - submittedBefore 및 submittedAfter에서 필터링할 때 Get-AzureRMDataLakeAnalyticsJob이 특정 날짜 시간 오프셋 값 목록으로 고정.
* Web Apps
  - 일반 교환 및 미리 보기 포함 교환에 대한 Swap-AzureRmWebAppSlot cmdlet 추가
  - 자동 교환을 지원하도록 Set-AzureRmWebAppSlot cmdlet 확장
* Azure API 관리
  - AzureChinaCloud에 대한 Azure API Management 배포 cmdlet 수정.
  - 기본적으로 Git 액세스를 사용하도록 설정되므로 Set-AzureRmApiManagementTenantGitAccess cmdlet 제거.
* Azure Recovery Services 백업
  - Azure SQL 워크로드 지원 추가
  - 암호화된 Azure VM 백업 및 복원 지원 추가
  - Backup-AzureRmRecoveryServicesBackupItem - 복구 지점에 대한 선택적 보존 시간 기능 추가
  - Get-AzureRmRecoveryServicesBackupContainer 및 Get-AzureRmRecoveryServicesBackupItem cmdlet의 보조 필터 관련 버그 수정
* Azure 자동화
  - Get-AzureRmAutomationHybridWorkerGroup 추가
