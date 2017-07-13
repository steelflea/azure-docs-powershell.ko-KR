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
ms.openlocfilehash: 04f89e8d47d0825d46cb1b8817efbcc0cafa0acd
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/29/2017
---
# <span data-ttu-id="a5cfb-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="a5cfb-103">Release notes</span></span>
<a id="release-notes" class="xliff"></a>

<span data-ttu-id="a5cfb-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <span data-ttu-id="a5cfb-105">3.8.0 버전</span><span class="sxs-lookup"><span data-stu-id="a5cfb-105">Version 3.8.0</span></span>
<a id="version-380" class="xliff"></a>
* <span data-ttu-id="a5cfb-106">Compute</span><span class="sxs-lookup"><span data-stu-id="a5cfb-106">Compute</span></span>
  - <span data-ttu-id="a5cfb-107">Get-* cmdlet의 버그를 수정하여 여러 페이지의 데이터(120개 이상 항목)를 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-107">Fix bug in Get-* cmdlets, to allow retrieving multiple pages of data (more than 120 items)</span></span>
* <span data-ttu-id="a5cfb-108">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="a5cfb-108">DataLakeAnalytics</span></span>
  - <span data-ttu-id="a5cfb-109">일부 명령어에 대한 도움말을 수정하여 적절한 verbage와 예제를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-109">Fix help for some commands to have the proper verbage and examples.</span></span>
* <span data-ttu-id="a5cfb-110">DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a5cfb-110">DataLakeStore</span></span>
  - <span data-ttu-id="a5cfb-111">`Get-AzureRMDataLakeStoreItemContent` cmdlet의 시작과 끝 부분에 대한 지원을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-111">Add support for head and tail to the `Get-AzureRMDataLakeStoreItemContent` cmdlet.</span></span> <span data-ttu-id="a5cfb-112">이렇게 하면 표시될 상위 N개 또는 마지막 N개의 새 줄 구분 기호로 분리된 행을 반환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-112">This enables returning the top N or last N new line delimited rows to be displayed.</span></span>
* <span data-ttu-id="a5cfb-113">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a5cfb-113">HDInsight</span></span>
  - <span data-ttu-id="a5cfb-114">RServer 클러스터 유형 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a5cfb-114">Added support for RServer cluster type</span></span>
    + <span data-ttu-id="a5cfb-115">에지 노드 VM 크기를 New-AzureRmHDInsightCluster 또는 New-AzureRmHDInsightClusterConfig의 RServer 클러스터에 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-115">Edgenode VM size can be specified for RServer cluster in New-AzureRmHDInsightCluster or New-AzureRmHDInsightClusterConfig</span></span>
    + <span data-ttu-id="a5cfb-116">이제 RServer는 Add-AzureRmHDInsightConfigValues의 구성 옵션입니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-116">RServer is now a configuration option in Add-AzureRmHDInsightConfigValues.</span></span> <span data-ttu-id="a5cfb-117">R Studio 설치를 수행해야 함을 나타내도록 RStudio 플래그를 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-117">It allows for RStudio flag to be set to indicate that R Studio installation should be done.</span></span>
* <span data-ttu-id="a5cfb-118">LogicApp</span><span class="sxs-lookup"><span data-stu-id="a5cfb-118">LogicApp</span></span>
  - <span data-ttu-id="a5cfb-119">contentlink 문제(content 및 contentlink가 모두 설정되어 업데이트 실패가 발생함)로 인해 Set-AzureRmIntegrationAccountSchema 및 Set-AzureRmIntegrationAccountMap cmdlet을 수정했습니다 .</span><span class="sxs-lookup"><span data-stu-id="a5cfb-119">Set-AzureRmIntegrationAccountSchema and Set-AzureRmIntegrationAccountMap cmdlets are fixed for the contentlink issue(Both content and contentlink were set resulting in update failure).</span></span>
* <span data-ttu-id="a5cfb-120">네트워크</span><span class="sxs-lookup"><span data-stu-id="a5cfb-120">Network</span></span>
  - <span data-ttu-id="a5cfb-121">Application Gateway에 대한 새 웹 응용 프로그램 방화벽 기능 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a5cfb-121">Added support for new web application firewall features to Application Gateways</span></span>
    + <span data-ttu-id="a5cfb-122">New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-122">Added New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig</span></span>
    + <span data-ttu-id="a5cfb-123">Get-AzureRmApplicationGatewayAvailableWafRuleSets(별칭: List-AzureRmApplicationGatewayAvailableWafRuleSets)를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-123">Added Get-AzureRmApplicationGatewayAvailableWafRuleSets (Alias: List-AzureRmApplicationGatewayAvailableWafRuleSets)</span></span>
    + <span data-ttu-id="a5cfb-124">New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration을 업데이트하고, -RuleSetType, -RuleSetVersion 및 -DisabledRuleGroups 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-124">Updated New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration: Added parameter -RuleSetType -RuleSetVersion and -DisabledRuleGroups</span></span>
    + <span data-ttu-id="a5cfb-125">AzureRmApplicationGatewayWebApplicationFirewallConfiguration을 업데이트하고, -RuleSetType, -RuleSetVersion 및 -DisabledRuleGroups 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-125">Updated Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration: Added parameter -RuleSetType -RuleSetVersion and -DisabledRuleGroups</span></span>
  - <span data-ttu-id="a5cfb-126">가상 네트워크 게이트웨이 연결에 대한 IPSec 정책 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a5cfb-126">Added support for IPSec policies to Virtual Network Gateway Connections</span></span>
  - <span data-ttu-id="a5cfb-127">New-AzureRmIpsecPolicy를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-127">Added New-AzureRmIpsecPolicy</span></span>
  - <span data-ttu-id="a5cfb-128">Updated New-AzureRmVirtualNetworkGatewayConnection 업데이트하고, -IpsecPolicies 및 -UsePolicyBasedTrafficSelectors 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-128">Updated New-AzureRmVirtualNetworkGatewayConnection: Added parameter -IpsecPolicies and -UsePolicyBasedTrafficSelectors</span></span>
* <span data-ttu-id="a5cfb-129">프로필</span><span class="sxs-lookup"><span data-stu-id="a5cfb-129">Profile</span></span>
  - <span data-ttu-id="a5cfb-130">*사용되지 않음*: Save-AzureRmProfile의 이름을 Save-AzureRmContext로 변경했으며, 이전 cmdlet 이름에 별칭이 있으면 다음 릴리스에서 이 별칭이 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-130">*Obsolete*: Save-AzureRmProfile is renamed to Save-AzureRmContext, there is an alias to the old cmdlet name, the alias will be removed in the next release.</span></span>
  - <span data-ttu-id="a5cfb-131">*사용되지 않음*: Select-AzureRmProfile의 이름을 Import-AzureRmContext로 변경했으며, 별칭이 이전 cmdlet 이름에 있으면 다음 릴리스에서 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-131">*Obsolete*: Select-AzureRmProfile is renamed to Import-AzureRmContext, there is an alias to the old cmdlet name, the alias will be removed in the next release.</span></span>
  - <span data-ttu-id="a5cfb-132">프로필 cmdlet의 PSAzureContext 및 PSAzureProfile 출력 형식은 다음 릴리스에서 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-132">The PSAzureContext and PSAzureProfile output types of profile cmdlets will be changed in the next release.</span></span>
  - <span data-ttu-id="a5cfb-133">Save-AzureRmContext cmdlet에는 다음 릴리스에서 OutputType이 제공되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-133">The Save-AzureRmContext cmdlet will have no OutputType in the next release.</span></span>
  - <span data-ttu-id="a5cfb-134">데이터 해시에 FIPS 규격 알고리즘을 사용하는 cmdlet 공용 코드의 버그를 수정했습니다(https://github.com/Azure/azure-powershell/issues/3651).</span><span class="sxs-lookup"><span data-stu-id="a5cfb-134">Fix bug in cmdlet common code to use FIPS-compliant algorithm for data hashes: https://github.com/Azure/azure-powershell/issues/3651</span></span>
* <span data-ttu-id="a5cfb-135">Sql</span><span class="sxs-lookup"><span data-stu-id="a5cfb-135">Sql</span></span>
  - <span data-ttu-id="a5cfb-136">Azure 장애 조치(failover) 그룹 cmdlet 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a5cfb-136">Bug fixes on Azure Failover Group Cmdlets</span></span>
  - <span data-ttu-id="a5cfb-137">작업 폴링을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-137">Fix for operation polling</span></span>
  - <span data-ttu-id="a5cfb-138">FailoverPolicy를 Manual로 설정하는 경우 GracePeriodWithDataLossHour 값을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-138">Fix GracePeriodWithDataLossHour value when setting FailoverPolicy to Manual</span></span>
* <span data-ttu-id="a5cfb-139">TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a5cfb-139">TrafficManager</span></span>
  - <span data-ttu-id="a5cfb-140">지리적 트래픽 라우팅 방법 지원</span><span class="sxs-lookup"><span data-stu-id="a5cfb-140">Support for the Geographic traffic routing method</span></span>
    + <span data-ttu-id="a5cfb-141">New-AzureRmTrafficManagerProfile의 TrafficRoutingMethod 매개 변수에 대한 새 값 'Geographic'</span><span class="sxs-lookup"><span data-stu-id="a5cfb-141">New value 'Geographic' for the TrafficRoutingMethod parameter of New-AzureRmTrafficManagerProfile</span></span>
    + <span data-ttu-id="a5cfb-142">New-AzureRmTrafficManagerEndpoint 및 Add-AzureRmTrafficManagerEndpointConfig에 대한 새로운 매개 변수 'GeoMapping'</span><span class="sxs-lookup"><span data-stu-id="a5cfb-142">New parameter 'GeoMapping' for the New-AzureRmTrafficManagerEndpoint and Add-AzureRmTrafficManagerEndpointConfig</span></span>
    + <span data-ttu-id="a5cfb-143">프로필 컬렉션을 반환할 때 Get-AzureRmTrafficManagerProfile에 대한 파이핑을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-143">Fix piping for Get-AzureRmTrafficManagerProfile when it returns a collection of profiles</span></span>
* <span data-ttu-id="a5cfb-144">ServiceManagement</span><span class="sxs-lookup"><span data-stu-id="a5cfb-144">ServiceManagement</span></span>
  - <span data-ttu-id="a5cfb-145">Restart-AzureVM: VM을 다시 시작하는 동안 유지 관리를 수행하기 위한 InitiateMaintenance 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-145">Restart-AzureVM: Added InitiateMaintenance parameter for performing maintenance during VM restart.</span></span>
  - <span data-ttu-id="a5cfb-146">Get-AzureVM: 유지 관리 상태 필드를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="a5cfb-146">Get-AzureVM: Added Maintenance Status field.</span></span>
  - <span data-ttu-id="a5cfb-147">Recovery Services 자격 증명 모음 업그레이드를 지원하는 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="a5cfb-147">Added new cmdlets to support Recovery Services vault upgrade</span></span>
    + <span data-ttu-id="a5cfb-148">Test-AzureRecoveryServicesVaultUpgrade</span><span class="sxs-lookup"><span data-stu-id="a5cfb-148">Test-AzureRecoveryServicesVaultUpgrade</span></span>
    + <span data-ttu-id="a5cfb-149">Invoke-AzureRecoveryServicesVaultUpgrade</span><span class="sxs-lookup"><span data-stu-id="a5cfb-149">Invoke-AzureRecoveryServicesVaultUpgrade</span></span>
