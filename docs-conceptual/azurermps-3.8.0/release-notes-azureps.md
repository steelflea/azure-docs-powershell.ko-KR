---
title: Azure PowerShell 변경 로그 | Microsoft Docs
description: Azure PowerShell에 대한 최신 릴리스의 변경 내용입니다.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: 2e17b6f7f62f25d8d91c4d32a4a1ae5c45b8665d
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/06/2018
ms.locfileid: "34821805"
---
# <a name="release-notes"></a>릴리스 정보

Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.

## <a name="version-380"></a>3.8.0 버전
* 컴퓨팅
  - Get-* cmdlet의 버그를 수정하여 여러 페이지의 데이터(120개 이상 항목)를 검색할 수 있습니다.
* DataLakeAnalytics
  - 일부 명령어에 대한 도움말을 수정하여 적절한 verbage와 예제를 제공합니다.
* DataLakeStore
  - `Get-AzureRMDataLakeStoreItemContent` cmdlet의 시작과 끝 부분에 대한 지원을 추가했습니다. 이렇게 하면 표시될 상위 N개 또는 마지막 N개의 새 줄 구분 기호로 분리된 행을 반환할 수 있습니다.
* HDInsight
  - RServer 클러스터 유형 지원 추가
    + 에지 노드 VM 크기를 New-AzureRmHDInsightCluster 또는 New-AzureRmHDInsightClusterConfig의 RServer 클러스터에 지정할 수 있습니다.
    + 이제 RServer는 Add-AzureRmHDInsightConfigValues의 구성 옵션입니다. R Studio 설치를 수행해야 함을 나타내도록 RStudio 플래그를 설정할 수 있습니다.
* LogicApp
  - contentlink 문제(content 및 contentlink가 모두 설정되어 업데이트 실패가 발생함)로 인해 Set-AzureRmIntegrationAccountSchema 및 Set-AzureRmIntegrationAccountMap cmdlet을 수정했습니다 .
* 네트워크
  - Application Gateway에 대한 새 웹 응용 프로그램 방화벽 기능 지원 추가
    + New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig를 추가했습니다.
    + Get-AzureRmApplicationGatewayAvailableWafRuleSets(별칭: List-AzureRmApplicationGatewayAvailableWafRuleSets)를 추가했습니다.
    + New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration을 업데이트하고, -RuleSetType, -RuleSetVersion 및 -DisabledRuleGroups 매개 변수를 추가했습니다.
    + AzureRmApplicationGatewayWebApplicationFirewallConfiguration을 업데이트하고, -RuleSetType, -RuleSetVersion 및 -DisabledRuleGroups 매개 변수를 추가했습니다.
  - Virtual Network 게이트웨이 연결에 대한 IPSec 정책 지원 추가
  - New-AzureRmIpsecPolicy를 추가했습니다.
  - Updated New-AzureRmVirtualNetworkGatewayConnection 업데이트하고, -IpsecPolicies 및 -UsePolicyBasedTrafficSelectors 매개 변수를 추가했습니다.
* 프로필
  - *사용되지 않음*: Save-AzureRmProfile의 이름을 Save-AzureRmContext로 변경했으며, 이전 cmdlet 이름에 별칭이 있으면 다음 릴리스에서 이 별칭이 제거됩니다.
  - *사용되지 않음*: Select-AzureRmProfile의 이름을 Import-AzureRmContext로 변경했으며, 별칭이 이전 cmdlet 이름에 있으면 다음 릴리스에서 제거됩니다.
  - 프로필 cmdlet의 PSAzureContext 및 PSAzureProfile 출력 형식은 다음 릴리스에서 변경됩니다.
  - Save-AzureRmContext cmdlet에는 다음 릴리스에서 OutputType이 제공되지 않습니다.
  - 데이터 해시에 FIPS 규격 알고리즘을 사용하는 cmdlet 공용 코드의 버그를 수정했습니다(https://github.com/Azure/azure-powershell/issues/3651).
* Sql
  - Azure 장애 조치(failover) 그룹 cmdlet 버그 수정
  - 작업 폴링을 수정했습니다.
  - FailoverPolicy를 Manual로 설정하는 경우 GracePeriodWithDataLossHour 값을 수정했습니다.
* TrafficManager
  - 지리적 트래픽 라우팅 방법 지원
    + New-AzureRmTrafficManagerProfile의 TrafficRoutingMethod 매개 변수에 대한 새 값 'Geographic'
    + New-AzureRmTrafficManagerEndpoint 및 Add-AzureRmTrafficManagerEndpointConfig에 대한 새로운 매개 변수 'GeoMapping'
    + 프로필 컬렉션을 반환할 때 Get-AzureRmTrafficManagerProfile에 대한 파이핑을 수정했습니다.
* ServiceManagement
  - Restart-AzureVM: VM을 다시 시작하는 동안 유지 관리를 수행하기 위한 InitiateMaintenance 매개 변수를 추가했습니다.
  - Get-AzureVM: 유지 관리 상태 필드를 추가했습니다.
  - Recovery Services 자격 증명 모음 업그레이드를 지원하는 새 cmdlet 추가
    + Test-AzureRecoveryServicesVaultUpgrade
    + Invoke-AzureRecoveryServicesVaultUpgrade
