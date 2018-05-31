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
ms.date: 5/1/2018
ms.openlocfilehash: 0b7902155c47f2e6355e9147c203867288caab81
ms.sourcegitcommit: 5971c92cb023bdd1d71fa2ad0a3b378abfbd092a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/23/2018
ms.locfileid: "34461898"
---
# <a name="release-notes"></a>릴리스 정보

Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.

---
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