---
title: Azure PowerShell 변경 로그 | Microsoft Docs
description: Azure PowerShell에 대한 최신 릴리스의 변경 내용입니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 08/28/2018
ms.openlocfilehash: 6a33d1a85fc61d0281bf1183163185b0dc4d3a12
ms.sourcegitcommit: f6f5e256143aa6c097de3e57e930d8badea49f30
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/18/2018
ms.locfileid: "49399062"
---
# <a name="release-notes"></a><span data-ttu-id="f1ef5-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="f1ef5-103">Release notes</span></span>

<span data-ttu-id="f1ef5-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6100---october-2018"></a><span data-ttu-id="f1ef5-105">2018년 10월 - 6.10.0</span><span class="sxs-lookup"><span data-stu-id="f1ef5-105">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="f1ef5-106">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="f1ef5-106">Azure.Storage</span></span>
* <span data-ttu-id="f1ef5-107">대상에 메타데이터가 있을 때 Blob/파일이 메타 데이터를 복사하지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-107">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="f1ef5-108">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="f1ef5-108">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="f1ef5-109">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="f1ef5-109">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="f1ef5-110">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="f1ef5-110">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="f1ef5-111">기존 계정이 없는 Get-AzureRmCognitiveServicesAccountSkus를 지원</span><span class="sxs-lookup"><span data-stu-id="f1ef5-111">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="f1ef5-112">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f1ef5-112">AzureRM.Compute</span></span>
* <span data-ttu-id="f1ef5-113">Get-AzureRmVM -ResourceGroupName <rg>가 필요한 경우 50개가 넘는 결과를 반환하도록 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-113">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="f1ef5-114">'SimpleParameterSet' 예제가 New-AzureRmVmss cmdlet 도움말에 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-114">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="f1ef5-115">Azure Disk Encryption 진행률 메시지의 오타를 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-115">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="f1ef5-116">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="f1ef5-116">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="f1ef5-117">ADF.Net SDK 버전을 2.3.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-117">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="f1ef5-118">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f1ef5-118">AzureRM.Network</span></span>
* <span data-ttu-id="f1ef5-119">NetworkProfile 기능 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-119">Added NetworkProfile functionality.</span></span> <span data-ttu-id="f1ef5-120">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-120">new cmdlets added</span></span>
    - <span data-ttu-id="f1ef5-121">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-121">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="f1ef5-122">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-122">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="f1ef5-123">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-123">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="f1ef5-124">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-124">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="f1ef5-125">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-125">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="f1ef5-126">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-126">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="f1ef5-127">서브넷 모델에 서비스 연결 링크 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-127">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="f1ef5-128">New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-128">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="f1ef5-129">Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-129">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="f1ef5-130">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="f1ef5-130">AzureRM.RedisCache</span></span>
* <span data-ttu-id="f1ef5-131">모든 문자열을 Size 매개 변수로 진행되도록 허용</span><span class="sxs-lookup"><span data-stu-id="f1ef5-131">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="f1ef5-132">PSArgumentCompleter 팝업에 P5 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-132">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="f1ef5-133">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="f1ef5-133">AzureRM.Resources</span></span>
* <span data-ttu-id="f1ef5-134">-Mode 매개 변수를 Set-AzureRmPolicyDefinition에 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-134">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="f1ef5-135">사용자가 포함된 Origin 작업에서 Get-AzureRmProviderOperation commandlet 버그 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-135">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="f1ef5-136">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="f1ef5-136">AzureRM.Sql</span></span>
* <span data-ttu-id="f1ef5-137">일부 백업 cmdlet이 현재 azure 구독을 인식하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-137">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="f1ef5-138">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="f1ef5-138">AzureRM.Storage</span></span>
* <span data-ttu-id="f1ef5-139">특정 위치의 저장소 리소스 사용을 지원하고 글로벌 저장소 리소스 사용 가져오기는 더 이상 사용되지 않는다는 경고 메시지를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-139">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="f1ef5-140">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="f1ef5-140">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="f1ef5-141">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="f1ef5-141">AzureRM.Websites</span></span>
* <span data-ttu-id="f1ef5-142">새 cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - 컨테이너 지속적인 배포 Webhook URL을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-142">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="f1ef5-143">새 cmdlet 
New-AzureRMWebAppContainerPSSession 및 Enter-WebAppContainerPSSession -  windows 컨테이너 앱에 PowerShell 원격 세션을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-143">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="f1ef5-144">6.9.0 - 2018년 9월</span><span class="sxs-lookup"><span data-stu-id="f1ef5-144">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="f1ef5-145">일반</span><span class="sxs-lookup"><span data-stu-id="f1ef5-145">General</span></span>
* <span data-ttu-id="f1ef5-146">AzureRM.SignalR이 AzureRM 롤업 모듈에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-146">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="f1ef5-147">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-147">AzureRM.Profile</span></span>
* <span data-ttu-id="f1ef5-148">저장소 일반 코드에 대한 약간의 변경</span><span class="sxs-lookup"><span data-stu-id="f1ef5-148">Minor changes to the storage common code</span></span>
* <span data-ttu-id="f1ef5-149">전체 매개 변수 형식을 포함하도록 도움말 파일이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-149">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="f1ef5-150">-ServicePrincipal을 필수가 아닌 것으로 ServicePrincipalCertificateWithSubscriptionId 매개변수 집합에서 변경</span><span class="sxs-lookup"><span data-stu-id="f1ef5-150">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="f1ef5-151">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="f1ef5-151">Azure.Storage</span></span>
* <span data-ttu-id="f1ef5-152">OAuth를 사용하여 저장소 컨텍스트를 만드는 것을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-152">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="f1ef5-153">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="f1ef5-153">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="f1ef5-154">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="f1ef5-154">AzureRM.Cdn</span></span>
* <span data-ttu-id="f1ef5-155">Cdn 가격 책정 sku에서 Standard_Microsoft를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-155">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="f1ef5-156">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f1ef5-156">AzureRM.Compute</span></span>
* <span data-ttu-id="f1ef5-157">Keyvault 및 Storage에서 종속성을 일반 종속성으로 이동</span><span class="sxs-lookup"><span data-stu-id="f1ef5-157">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="f1ef5-158">AEM cmdlet에 더 많은 가상 머신 크기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-158">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="f1ef5-159">PublicIPPrefix 매개 변수를 New-AzureRmVmssIpConfig에 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-159">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="f1ef5-160">Invoke-AzureRmVMRunCommand cmdelt에 ResourceId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-160">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="f1ef5-161">Invoke-AzureRmVmssVMRunCommand cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-161">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="f1ef5-162">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="f1ef5-162">AzureRM.Dns</span></span>
* <span data-ttu-id="f1ef5-163">Dns 레코드를 만드는 동안 별칭 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-163">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="f1ef5-164">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="f1ef5-164">AzureRM.Insights</span></span>
* <span data-ttu-id="f1ef5-165">#6833 및 #7102 문제 수정(진단 설정 영역)</span><span class="sxs-lookup"><span data-stu-id="f1ef5-165">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="f1ef5-166">기본 이름, 즉 'service'에 진단 설정의 목록 생성 및 가져오는 동안에 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-166">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="f1ef5-167">범주를 사용하는 진단 설정 만들기 문제</span><span class="sxs-lookup"><span data-stu-id="f1ef5-167">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="f1ef5-168">메트릭 시간 조직 매개 변수에 대한 사용 중단 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-168">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="f1ef5-169">Timegrains 매개 변수는 여전히 받아들여지고 있습니다(이것은 호환성이 손상되는 변경이 아닙니다). 그러나 PT1M만 유효하므로 백엔드에서 무시됩니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-169">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="f1ef5-170">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f1ef5-170">AzureRM.Network</span></span>
* <span data-ttu-id="f1ef5-171">LoadBalancer cmdlet에 대한 변경</span><span class="sxs-lookup"><span data-stu-id="f1ef5-171">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="f1ef5-172">LoadBalancerInboundNatPoolConfig: IdleTimeoutInMinutes, EnableFloatingIp 및 EnableTcpReset 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-172">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="f1ef5-173">LoadBalancerInboundNatRuleConfig: EnableTcpReset 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-173">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="f1ef5-174">LoadBalancerRuleConfig: EnableTcpReset 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-174">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="f1ef5-175">LoadBalancerProbeConfig: 매개 변수 프로토콜에 대해 "Https" 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-175">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="f1ef5-176">새 LoadBalancer의 하위 리소스OutboundRule에 대한 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-176">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="f1ef5-177">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-177">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="f1ef5-178">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-178">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="f1ef5-179">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-179">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="f1ef5-180">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-180">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="f1ef5-181">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-181">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="f1ef5-182">PSNetworkInterface에 대한 새 HostedWorkloads 속성 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-182">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="f1ef5-183">기능에 대한 새 cmdlet 추가: ARM을 통한 Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="f1ef5-183">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="f1ef5-184">Get-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-184">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="f1ef5-185">Set-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-185">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="f1ef5-186">New-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-186">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="f1ef5-187">Remove-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-187">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="f1ef5-188">New-AzureRmFirewallApplicationRuleCollection 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-188">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="f1ef5-189">New-AzureRmFirewallApplicationRule 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-189">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="f1ef5-190">New-AzureRmFirewallNatRuleCollection 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-190">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="f1ef5-191">New-AzureRmFirewallNatRule 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-191">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="f1ef5-192">New-AzureRmFirewallNetworkRuleCollection 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-192">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="f1ef5-193">New-AzureRmFirewallNetworkRule 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-193">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="f1ef5-194">Application Gateway에서 신뢰할 수 있는 루트 인증서 및 크기 자동 조정 구성에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-194">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="f1ef5-195">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-195">New Cmdlets added:</span></span>
      - <span data-ttu-id="f1ef5-196">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f1ef5-196">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="f1ef5-197">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f1ef5-197">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="f1ef5-198">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f1ef5-198">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="f1ef5-199">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f1ef5-199">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="f1ef5-200">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f1ef5-200">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="f1ef5-201">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-201">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="f1ef5-202">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-202">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="f1ef5-203">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-203">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="f1ef5-204">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-204">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="f1ef5-205">옵션 매개 변수를 사용하도록 업데이트된 Cmdlet-TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f1ef5-205">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="f1ef5-206">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="f1ef5-206">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="f1ef5-207">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="f1ef5-207">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="f1ef5-208">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="f1ef5-208">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="f1ef5-209">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="f1ef5-209">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="f1ef5-210">옵션 매개 변수를 사용하도록 업데이트된 Cmdlet-AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-210">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="f1ef5-211">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="f1ef5-211">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="f1ef5-212">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="f1ef5-212">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="f1ef5-213">인터페이스 엔드포인트 Get-AzureInterfaceEndpoint에 대한 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-213">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="f1ef5-214">서브넷에서 여러 주소 접두사에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-214">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="f1ef5-215">다음 Cmdlet이 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-215">Updated cmdlets:</span></span>
  - <span data-ttu-id="f1ef5-216">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-216">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="f1ef5-217">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-217">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="f1ef5-218">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-218">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="f1ef5-219">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-219">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="f1ef5-220">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="f1ef5-220">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="f1ef5-221">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-221">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="f1ef5-222">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-222">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="f1ef5-223">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-223">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="f1ef5-224">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-224">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="f1ef5-225">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-225">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="f1ef5-226">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-226">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="f1ef5-227">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-227">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="f1ef5-228">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-228">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="f1ef5-229">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-229">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="f1ef5-230">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-230">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="f1ef5-231">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-231">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="f1ef5-232">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-232">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="f1ef5-233">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-233">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="f1ef5-234">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="f1ef5-234">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="f1ef5-235">서브넷 위임에 대한 cmdlet을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-235">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="f1ef5-236">New-AzureRmDelegation: 서브넷에 추가할 수 있는 새 위임을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-236">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="f1ef5-237">Remove-AzureRmDelegation: 서브넷에서 가져와서 해당 서브넷에서 제공된 위임 이름을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-237">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="f1ef5-238">Add-AzureRmDelegation: 서브넷에서 사용 및 제공된 서비스 이름을 해당 서브넷에 대한 위임으로 추가합니다</span><span class="sxs-lookup"><span data-stu-id="f1ef5-238">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="f1ef5-239">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="f1ef5-239">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="f1ef5-240">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="f1ef5-240">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="f1ef5-241">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="f1ef5-241">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="f1ef5-242">관리되는 관리 디스크에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="f1ef5-242">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="f1ef5-243">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="f1ef5-243">AzureRM.RedisCache</span></span>
* <span data-ttu-id="f1ef5-244">인사이트 종속성이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-244">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="f1ef5-245">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="f1ef5-245">AzureRM.Resources</span></span>
* <span data-ttu-id="f1ef5-246">New-AzureRmResourceGroupDeployment를 RollbackAction 새 매개 변수를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-246">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="f1ef5-247">새 매개 변수를 사용하여 OnErrorDeployment에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-247">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="f1ef5-248">정책 할당에서 관리되는 ID를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-248">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="f1ef5-249">'New-AzureRmPolicyAssignment'를 사용하여 정책을 할당할 때 기본값이 있는 매개 변수는 더 이상 필요하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-249">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="f1ef5-250">정책 별칭을 검색하기 위한 새 cmdlet Get-AzureRmPolicyAlias 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-250">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="f1ef5-251">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f1ef5-251">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="f1ef5-252">#7161 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-252">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="f1ef5-253">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="f1ef5-253">AzureRM.SignalR</span></span>
* <span data-ttu-id="f1ef5-254">SKU 이름을 Free_F1 및 Standard_S1로 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-254">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="f1ef5-255">버전 필드를 PSSignalRResource 개체에 추가하고 연결 문자열을 PSSignalRKeys개체에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-255">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="f1ef5-256">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="f1ef5-256">AzureRM.Storage</span></span>
* <span data-ttu-id="f1ef5-257">AzureRm.Storage에서 불변성 정책 지원</span><span class="sxs-lookup"><span data-stu-id="f1ef5-257">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="f1ef5-258">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="f1ef5-258">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="f1ef5-259">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="f1ef5-259">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="f1ef5-260">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="f1ef5-260">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="f1ef5-261">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="f1ef5-261">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="f1ef5-262">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="f1ef5-262">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="f1ef5-263">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="f1ef5-263">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="f1ef5-264">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="f1ef5-264">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="f1ef5-265">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="f1ef5-265">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="f1ef5-266">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="f1ef5-266">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="f1ef5-267">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="f1ef5-267">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="f1ef5-268">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="f1ef5-268">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="f1ef5-269">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="f1ef5-269">AzureRM.Websites</span></span>
* <span data-ttu-id="f1ef5-270">두 개의 새로운 cmdlet 추가: Get-AzureRmDeletedWebApp 및 Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="f1ef5-270">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="f1ef5-271">New-AzureRmAppServicePlan -HyperV 스위치가 창 컨테이너가 있는 앱 서비스 계획 작성용으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-271">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="f1ef5-272">New-AzureRmWebApp/New-AzureRmWebAppSlot/Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - Windows 컨테이너 앱을 만들고 관리하기 위한 새 매개 변수(-ContainerRegistryUser 문자열 -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment)가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-272">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="f1ef5-273">6.8.1 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="f1ef5-273">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="f1ef5-274">일반</span><span class="sxs-lookup"><span data-stu-id="f1ef5-274">General</span></span>
* <span data-ttu-id="f1ef5-275">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-275">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="f1ef5-276">공용 런타임 어셈블리가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-276">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="f1ef5-277">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f1ef5-277">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="f1ef5-278">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-278">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="f1ef5-279">문제 https://github.com/Azure/azure-powershell/issues/6603 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-279">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="f1ef5-280">Import-AzureRmApiManagementApi 및 \*-AzureRmApiManagementCertificate cmdlet은 이제 상대 경로를 처리합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-280">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="f1ef5-281">문제 https://github.com/Azure/azure-powershell/issues/6879 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-281">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="f1ef5-282">CertificateInformation은 Set-AzureRmApiManagement cmdlet이 제대로 작동 하게 하는 설정 가능한 속성입니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-282">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="f1ef5-283">4.0.4-preview nuget으로 업그레이드하여 해결됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-283">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="f1ef5-284">문제 https://github.com/Azure/azure-powershell/issues/6853 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-284">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="f1ef5-285">제품에서 이름별 검색에 대해 Odata 필터가 수정됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-285">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="f1ef5-286">문제 https://github.com/Azure/azure-powershell/issues/6814 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-286">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="f1ef5-287">API에서 이름별 검색에 대해 Odata 필터가 수정됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-287">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="f1ef5-288">AzureMonitor 로거에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-288">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="f1ef5-289">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f1ef5-289">AzureRM.Compute</span></span>
* <span data-ttu-id="f1ef5-290">오류 출력에 대상이 없는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-290">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="f1ef5-291">관리 디스크를 사용하는 VM에 대한 저장소 계정 유형 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-291">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="f1ef5-292">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-292">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="f1ef5-293">예를 들어 Azure 중국과 같이, 다른 환경에 대한 AEM 확장 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-293">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="f1ef5-294">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f1ef5-294">AzureRM.Network</span></span>
* <span data-ttu-id="f1ef5-295">기본 cmdlet 출력 표시를 테이블 뷰로 변경</span><span class="sxs-lookup"><span data-stu-id="f1ef5-295">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="f1ef5-296">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="f1ef5-296">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="f1ef5-297">일시 중지된 용량을 확장하려고 할 때 Update-AzureRmPowerBIEmbeddedCapacity 실패 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-297">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="f1ef5-298">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="f1ef5-298">AzureRM.Resources</span></span>
* <span data-ttu-id="f1ef5-299">MarketPlace에서 관리되는 응용 프로그램 생성 시의 문제 해결.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-299">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="f1ef5-300">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f1ef5-300">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="f1ef5-301">해결된 문제</span><span class="sxs-lookup"><span data-stu-id="f1ef5-301">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="f1ef5-302">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="f1ef5-302">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="f1ef5-303">다중값 라우팅 메서드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-303">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="f1ef5-304">다중값 라우팅에 대한 새 매개 변수 'MaxReturn'</span><span class="sxs-lookup"><span data-stu-id="f1ef5-304">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="f1ef5-305">서브넷 라우팅 메서드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-305">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="f1ef5-306">엔드포인트의 IP 주소 범위(서브넷)에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="f1ef5-306">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="f1ef5-307">프로필 내 사용자 지정 헤더에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-307">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="f1ef5-308">프로필 내 예상 상태 코드 범위에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-308">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="f1ef5-309">엔드포인트 내 사용자 지정 헤더에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-309">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="f1ef5-310">6.8.0 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="f1ef5-310">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="f1ef5-311">일반</span><span class="sxs-lookup"><span data-stu-id="f1ef5-311">General</span></span>
* <span data-ttu-id="f1ef5-312">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-312">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="f1ef5-313">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-313">AzureRM.Profile</span></span>
* <span data-ttu-id="f1ef5-314">Connect-AzureRmAccount 중에 반환된 토큰에 만료 속성 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-314">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="f1ef5-315">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f1ef5-315">AzureRM.Compute</span></span>
* <span data-ttu-id="f1ef5-316">오류 출력에 대상이 없는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-316">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="f1ef5-317">관리 디스크를 사용하는 VM에 대한 저장소 계정 유형 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-317">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="f1ef5-318">예를 들어 Azure 중국과 같이, 다른 환경에 대한 AEM 확장 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-318">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="f1ef5-319">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="f1ef5-319">AzureRM.IotHub</span></span>
* <span data-ttu-id="f1ef5-320">New-AzureRmIotHubExportDevices 및 New-AzureRmIotHubImportDevices에 대한 예제를 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-320">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="f1ef5-321">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f1ef5-321">AzureRM.Network</span></span>
* <span data-ttu-id="f1ef5-322">기본 모델 표시를 테이블 뷰로 변경</span><span class="sxs-lookup"><span data-stu-id="f1ef5-322">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="f1ef5-323">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="f1ef5-323">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="f1ef5-324">일시 중지된 용량을 확장하려고 할 때 Update-AzureRmPowerBIEmbeddedCapacity 실패 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-324">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="f1ef5-325">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="f1ef5-325">AzureRM.Resources</span></span>
* <span data-ttu-id="f1ef5-326">MarketPlace에서 관리되는 응용 프로그램 생성 시의 문제 해결.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-326">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="f1ef5-327">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f1ef5-327">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="f1ef5-328">문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-328">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="f1ef5-329">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="f1ef5-329">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="f1ef5-330">다중값 라우팅 메서드에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="f1ef5-330">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="f1ef5-331">다중값 라우팅에 대한 새 매개 변수 'MaxReturn'</span><span class="sxs-lookup"><span data-stu-id="f1ef5-331">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="f1ef5-332">서브넷 라우팅 메서드에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="f1ef5-332">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="f1ef5-333">엔드포인트의 IP 주소 범위(서브넷)에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="f1ef5-333">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="f1ef5-334">프로필 내 사용자 지정 헤더에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="f1ef5-334">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="f1ef5-335">프로필 내 예상 상태 코드 범위에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="f1ef5-335">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="f1ef5-336">엔드포인트 내 사용자 지정 헤더에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="f1ef5-336">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="f1ef5-337">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="f1ef5-337">AzureRM.Websites</span></span>
* <span data-ttu-id="f1ef5-338">기본 리소스 그룹이 잘못 설정되는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-338">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="f1ef5-339">6.7.0 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="f1ef5-339">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="f1ef5-340">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-340">AzureRM.Profile</span></span>
* <span data-ttu-id="f1ef5-341">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-341">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="f1ef5-342">충돌을 방지하려면 기본 컨텍스트 이름으로 사용자 ID를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-342">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="f1ef5-343">#6398 컨텍스트를 선택할 때 문제를 발생시킨 Clear-AzureRmContext 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-343">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="f1ef5-344">'Connect-AzureRmAccount'에 대한 '-TenantId' 매개 변수에 전달할 테넌트 도메인을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-344">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="f1ef5-345">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="f1ef5-345">Azure.Storage</span></span>
* <span data-ttu-id="f1ef5-346">Azure 파일 공유 할당량에 대한 5TB 제한 제거</span><span class="sxs-lookup"><span data-stu-id="f1ef5-346">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="f1ef5-347">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="f1ef5-347">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="f1ef5-348">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="f1ef5-348">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="f1ef5-349">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-349">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="f1ef5-350">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="f1ef5-350">Azure.AnalysisServices</span></span>
* <span data-ttu-id="f1ef5-351">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-351">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="f1ef5-352">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f1ef5-352">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="f1ef5-353">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-353">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="f1ef5-354">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="f1ef5-354">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="f1ef5-355">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-355">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="f1ef5-356">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="f1ef5-356">AzureRM.Automation</span></span>
* <span data-ttu-id="f1ef5-357">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-357">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="f1ef5-358">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="f1ef5-358">AzureRM.Backup</span></span>
* <span data-ttu-id="f1ef5-359">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-359">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="f1ef5-360">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="f1ef5-360">AzureRM.Batch</span></span>
* <span data-ttu-id="f1ef5-361">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-361">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="f1ef5-362">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="f1ef5-362">AzureRM.Billing</span></span>
* <span data-ttu-id="f1ef5-363">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-363">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="f1ef5-364">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="f1ef5-364">AzureRM.Cdn</span></span>
* <span data-ttu-id="f1ef5-365">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-365">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="f1ef5-366">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="f1ef5-366">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="f1ef5-367">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-367">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="f1ef5-368">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f1ef5-368">AzureRM.Compute</span></span>
* <span data-ttu-id="f1ef5-369">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-369">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="f1ef5-370">New-AzureRmVmssConfig에 EvictionPolicy 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-370">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="f1ef5-371">지정된 위치가 없는 경우에 New-AzureRmVm의 DiskFileParameterSet 내의 기본 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-371">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="f1ef5-372">Save-AzureRmVMImage에서 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-372">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="f1ef5-373">특정 singlepass 관련 시나리오에 대해 Get-AzureRmVMDiskEncryptionStatus cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-373">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="f1ef5-374">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="f1ef5-374">AzureRM.Consumption</span></span>
* <span data-ttu-id="f1ef5-375">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-375">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="f1ef5-376">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="f1ef5-376">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="f1ef5-377">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-377">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="f1ef5-378">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="f1ef5-378">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="f1ef5-379">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-379">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="f1ef5-380">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="f1ef5-380">AzureRM.DataFactories</span></span>
* <span data-ttu-id="f1ef5-381">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-381">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="f1ef5-382">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="f1ef5-382">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="f1ef5-383">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-383">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="f1ef5-384">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="f1ef5-384">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="f1ef5-385">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-385">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="f1ef5-386">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f1ef5-386">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="f1ef5-387">DebugPreference가 powershell 명령줄에서 설정된 경우 디버깅 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-387">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="f1ef5-388">Set-AzureRmDataLakeStoreItemAcl에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-388">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="f1ef5-389">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-389">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="f1ef5-390">Set-AzureRmDataLakeStoreItemAclEntry에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-390">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="f1ef5-391">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="f1ef5-391">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="f1ef5-392">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-392">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="f1ef5-393">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="f1ef5-393">AzureRM.Dns</span></span>
* <span data-ttu-id="f1ef5-394">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-394">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="f1ef5-395">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="f1ef5-395">AzureRM.EventGrid</span></span>
* <span data-ttu-id="f1ef5-396">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="f1ef5-397">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="f1ef5-397">AzureRM.EventHub</span></span>
* <span data-ttu-id="f1ef5-398">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-398">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="f1ef5-399">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="f1ef5-399">AzureRM.HDInsight</span></span>
* <span data-ttu-id="f1ef5-400">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-400">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="f1ef5-401">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="f1ef5-401">AzureRM.Insights</span></span>
* <span data-ttu-id="f1ef5-402">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-402">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="f1ef5-403">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="f1ef5-403">AzureRM.IotHub</span></span>
* <span data-ttu-id="f1ef5-404">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-404">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="f1ef5-405">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1ef5-405">AzureRM.KeyVault</span></span>
* <span data-ttu-id="f1ef5-406">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="f1ef5-407">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="f1ef5-407">AzureRM.LogicApp</span></span>
* <span data-ttu-id="f1ef5-408">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-408">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="f1ef5-409">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="f1ef5-409">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="f1ef5-410">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-410">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="f1ef5-411">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="f1ef5-411">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="f1ef5-412">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-412">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="f1ef5-413">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="f1ef5-413">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="f1ef5-414">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-414">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="f1ef5-415">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="f1ef5-415">AzureRM.Media</span></span>
* <span data-ttu-id="f1ef5-416">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-416">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="f1ef5-417">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f1ef5-417">AzureRM.Network</span></span>
* <span data-ttu-id="f1ef5-418">Set-AzureRmLocalNetworkGateway에 대한 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-418">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="f1ef5-419">Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey, New-AzureRmVirtualNetworkGatewayConnection에 대한 예제 및 설명 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-419">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="f1ef5-420">Remove-AzureRmVirtualNetworkGatewayIpConfig 및 Reset-AzureRmVirtualNetworkGateway에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-420">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="f1ef5-421">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-421">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="f1ef5-422">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-422">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="f1ef5-423">Set-AzureRmVirtualNetworkGatewayConnection에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-423">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="f1ef5-424">최신 코드 생성기를 사용하여 ApplicationSecurityGroup, RouteTable 및 Usage에 대한 cmdlet을 다시 생성함</span><span class="sxs-lookup"><span data-stu-id="f1ef5-424">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="f1ef5-425">Exitc 하지 않는 서브넷을 얻으려고 할 때의 Get-AzureRmVirtualNetworkSubnetConfig에 대한 오류 메시지를 설명</span><span class="sxs-lookup"><span data-stu-id="f1ef5-425">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="f1ef5-426">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="f1ef5-426">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="f1ef5-427">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="f1ef5-428">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="f1ef5-428">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="f1ef5-429">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="f1ef5-430">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="f1ef5-430">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="f1ef5-431">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="f1ef5-432">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="f1ef5-432">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="f1ef5-433">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="f1ef5-434">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f1ef5-434">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="f1ef5-435">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="f1ef5-436">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="f1ef5-436">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="f1ef5-437">Get-AzureRmRecoveryServicesBackItem cmdlet에 정책 필터 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-437">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="f1ef5-438">해당 명령은 지정된 정책 ID에 의해 보호되는 백업 항목의 목록을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-438">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="f1ef5-439">Microsoft.Azure.Management.RecoveryServices.Backup을 버전 3.0.0-preview로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="f1ef5-439">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="f1ef5-440">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-440">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="f1ef5-441">Restore-AzureRmRecoveryServicesBackupItem에 TargetResourceGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-441">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="f1ef5-442">관리 디스크가 복원될 리소스 그룹</span><span class="sxs-lookup"><span data-stu-id="f1ef5-442">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="f1ef5-443">관리 디스크가 있는 VM의 백업에 적용 가능</span><span class="sxs-lookup"><span data-stu-id="f1ef5-443">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="f1ef5-444">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="f1ef5-444">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="f1ef5-445">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-445">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="f1ef5-446">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="f1ef5-446">AzureRM.RedisCache</span></span>
* <span data-ttu-id="f1ef5-447">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-447">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="f1ef5-448">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="f1ef5-448">AzureRM.Relay</span></span>
* <span data-ttu-id="f1ef5-449">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-449">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="f1ef5-450">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="f1ef5-450">AzureRM.Resources</span></span>
* <span data-ttu-id="f1ef5-451">구독 범위에서 템플릿 배포를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-451">Support template deployment at subscription scope.</span></span> <span data-ttu-id="f1ef5-452">새 cmdlet 추가:</span><span class="sxs-lookup"><span data-stu-id="f1ef5-452">Add new Cmdlets:</span></span>
    - <span data-ttu-id="f1ef5-453">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="f1ef5-453">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="f1ef5-454">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="f1ef5-454">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="f1ef5-455">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="f1ef5-455">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="f1ef5-456">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="f1ef5-456">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="f1ef5-457">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="f1ef5-457">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="f1ef5-458">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="f1ef5-458">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="f1ef5-459">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="f1ef5-459">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="f1ef5-460">Set-AzureRmResource에 컨텍스트를 전달할 때 오류가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-460">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="f1ef5-461">New-AzureRmResourceGroupDeployment의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-461">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="f1ef5-462">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-462">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="f1ef5-463">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="f1ef5-463">AzureRM.Scheduler</span></span>
* <span data-ttu-id="f1ef5-464">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-464">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="f1ef5-465">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f1ef5-465">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="f1ef5-466">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-466">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="f1ef5-467">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f1ef5-467">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="f1ef5-468">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-468">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="f1ef5-469">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="f1ef5-469">AzureRM.Sql</span></span>
* <span data-ttu-id="f1ef5-470">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-470">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="f1ef5-471">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="f1ef5-471">AzureRM.Storage</span></span>
* <span data-ttu-id="f1ef5-472">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-472">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="f1ef5-473">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="f1ef5-473">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="f1ef5-474">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-474">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="f1ef5-475">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="f1ef5-475">AzureRM.Tags</span></span>
* <span data-ttu-id="f1ef5-476">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-476">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="f1ef5-477">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="f1ef5-477">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="f1ef5-478">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-478">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="f1ef5-479">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="f1ef5-479">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="f1ef5-480">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-480">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="f1ef5-481">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="f1ef5-481">AzureRM.Websites</span></span>
* <span data-ttu-id="f1ef5-482">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-482">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="f1ef5-483">6.6.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="f1ef5-483">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="f1ef5-484">일반</span><span class="sxs-lookup"><span data-stu-id="f1ef5-484">General</span></span>
* <span data-ttu-id="f1ef5-485">전체 매개 변수 형식 및 올바른 입/출력 형식을 포함하도록 모든 도움말 파일을 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-485">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="f1ef5-486">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-486">AzureRM.Profile</span></span>
* <span data-ttu-id="f1ef5-487">Common.Strategy 라이브러리가 리소스에 대한 현재 구성이 대상 리소스와 호환되는지 유효성을 검사할 수 있도록 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-487">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="f1ef5-488">Common.Storage에 ps1xml 형식 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-488">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="f1ef5-489">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="f1ef5-489">Azure.Storage</span></span>
* <span data-ttu-id="f1ef5-490">DefaultProfile에서 저장소 컨텍스트를 가져오기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-490">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="f1ef5-491">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-491">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="f1ef5-492">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f1ef5-492">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="f1ef5-493">문제 https://github.com/Azure/azure-powershell/issues/6370 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-493">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="f1ef5-494">PsApiManagementApi를 ApiContract로 좌표 이동하도록 Automapper 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-494">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="f1ef5-495">문제 https://github.com/Azure/azure-powershell/issues/6515 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-495">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="f1ef5-496">인코딩 형식을 사용하여 오버로드하지 않도록 File.Save 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-496">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="f1ef5-497">문제 https://github.com/Azure/azure-powershell/issues/6560 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-497">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="f1ef5-498">apiId에서 패턴 예외를 수정하는 4.0.3 Nuget 버전으로 업그레이드됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-498">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="f1ef5-499">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f1ef5-499">AzureRM.Compute</span></span>
* <span data-ttu-id="f1ef5-500">PremiumLRS 저장소 계정 형식 이름 바꾸기로 인해 New-AzureRmVm에서 DiskFileParameterSet를 사용하여 vm 생성 시 실패하는 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-500">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="f1ef5-501">Invoke-AzureRmVMRunCommand cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-501">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="f1ef5-502">Get-AzureRmAvailabilitySet를 업데이트하여 구독에서 모든 가용성 집합 리스트를 사용하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-502">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="f1ef5-503">(ResouceGroupName 매개 변수는 이제 선택적 요소입니다.)</span><span class="sxs-lookup"><span data-stu-id="f1ef5-503">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="f1ef5-504">vm 선별에 가속화된 네트워크를 사용하도록 'New-AzureRmVm'의 SimpleParameterSet를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-504">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="f1ef5-505">New-AzureRmVmss 간단 매개 변수가 사용자 지정 LB가 이미 존재할 때 vms 생성에 실패하도록 설정하여 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-505">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="f1ef5-506">New-AzureRmDisk에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-506">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="f1ef5-507">'New-AzureRmVM'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-507">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="f1ef5-508">Set-AzureRmVMOSDisk에 대한 설명 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-508">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="f1ef5-509">Set-AzureRmVMBginfoExtension 맞춤법 및 접두사를 수정하도록 예제 1을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-509">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="f1ef5-510">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="f1ef5-510">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="f1ef5-511">ADF.Net SDK 버전을 1.1.0으로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-511">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="f1ef5-512">데이터 팩터리를 공유하는 자체 호스팅된 통합 런타임을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-512">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="f1ef5-513">새 매개 변수 -SharedIntegrationRuntimeResourceId를 Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-513">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="f1ef5-514">새로운 선택적 매개 변수 -LinkedDataFactoryName을 Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-514">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="f1ef5-515">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f1ef5-515">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="f1ef5-516">DataPlane SDK(Microsoft.Azure.DataLake.Store) 버전을 1.1.9로 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-516">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="f1ef5-517">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="f1ef5-517">AzureRM.EventHub</span></span>
* <span data-ttu-id="f1ef5-518">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-518">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="f1ef5-519">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="f1ef5-519">AzureRM.Insights</span></span>
* <span data-ttu-id="f1ef5-520">도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-520">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="f1ef5-521">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview를 사용</span><span class="sxs-lookup"><span data-stu-id="f1ef5-521">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="f1ef5-522">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1ef5-522">AzureRM.KeyVault</span></span>
* <span data-ttu-id="f1ef5-523">Set-AzureRmKeyVaultAccessPolicy 내 파이핑 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-523">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="f1ef5-524">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f1ef5-524">AzureRM.Network</span></span>
* <span data-ttu-id="f1ef5-525">LoadBalancerInboundNatPoolConfig cmdlet에 대한 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-525">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="f1ef5-526">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="f1ef5-526">AzureRM.Resources</span></span>
* <span data-ttu-id="f1ef5-527">'Get-AzureRmResource'에 대한 태그 이름 및 값을 제공할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-527">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="f1ef5-528">'Set-AzureRmResource'를 사용하여 파이핑 시나리오 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-528">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="f1ef5-529">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f1ef5-529">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="f1ef5-530">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-530">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="f1ef5-531">몇 가지 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-531">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="f1ef5-532">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="f1ef5-532">AzureRM.Sql</span></span>
* <span data-ttu-id="f1ef5-533">다음 cmdlet 사용하여 서버 Advanced Threat Protection 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-533">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="f1ef5-534">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="f1ef5-534">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="f1ef5-535">다음 cmdlet을 사용하여 취약성 평가 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-535">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="f1ef5-536">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="f1ef5-536">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="f1ef5-537">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="f1ef5-537">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="f1ef5-538">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="f1ef5-538">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="f1ef5-539">Remove-AzureRmSqlServerFirewallRule의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-539">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="f1ef5-540">Get-AzureSqlSyncGroupLog에서 미국이 아닌 문화권에서 날짜/시간을 올바르지 않게 다루는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-540">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="f1ef5-541">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="f1ef5-541">AzureRM.Storage</span></span>
* <span data-ttu-id="f1ef5-542">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-542">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="f1ef5-543">StorageAccount cmdlet 출력을 테이블 뷰로 표시</span><span class="sxs-lookup"><span data-stu-id="f1ef5-543">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="f1ef5-544">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="f1ef5-544">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="f1ef5-545">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="f1ef5-545">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="f1ef5-546">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="f1ef5-546">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="f1ef5-547">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="f1ef5-547">AzureRM.Tags</span></span>
* <span data-ttu-id="f1ef5-548">태그 cmdlet 도움말에서 잘못된 문을 제거합니다</span><span class="sxs-lookup"><span data-stu-id="f1ef5-548">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="f1ef5-549">6.5.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="f1ef5-549">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="f1ef5-550">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-550">AzureRM.Profile</span></span>
* <span data-ttu-id="f1ef5-551">'Get-AzureRmContextAutosaveSetting'에 대한 도움말이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-551">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="f1ef5-552">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="f1ef5-552">Azure.Storage</span></span>
* <span data-ttu-id="f1ef5-553">쓰기 전용 SaS 토큰을 사용하는 Blob 또는 파일 업로드 지원</span><span class="sxs-lookup"><span data-stu-id="f1ef5-553">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="f1ef5-554">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="f1ef5-554">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="f1ef5-555">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="f1ef5-555">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="f1ef5-556">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="f1ef5-556">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="f1ef5-557">필수 속성 ResourceGroupName을 AS에 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-557">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="f1ef5-558">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="f1ef5-558">AzureRM.Automation</span></span>
* <span data-ttu-id="f1ef5-559">도움말을 업데이트하고 'New-AzureRMAutomationSchedule'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-559">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="f1ef5-560">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f1ef5-560">AzureRM.Compute</span></span>
* <span data-ttu-id="f1ef5-561">-Tag 매개 변수를 Update/New-AzureRmAvailabilitySet에 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-561">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="f1ef5-562">‘Add-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-562">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="f1ef5-563">‘Remove-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-563">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="f1ef5-564">‘Set-AzureRmVMAccessExtension’에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-564">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="f1ef5-565">기본으로 SinglePlacementGroup을 false로 설정하고 단일 배치 그룹에 VMSS를 만들 수 있는 스위치 매개 변수 'SinglePlacementGroup'을 추가하도록 New-AzureRmVmss에 대한 SimpleParameterSet을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-565">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="f1ef5-566">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="f1ef5-566">AzureRM.EventHub</span></span>
* <span data-ttu-id="f1ef5-567">PSEventHubDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="f1ef5-567">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="f1ef5-568">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1ef5-568">AzureRM.KeyVault</span></span>
* <span data-ttu-id="f1ef5-569">Set-AzureRmKeyVaultAccessPolicy에 대한 오류 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-569">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="f1ef5-570">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="f1ef5-570">AzureRM.LogicApp</span></span>
* <span data-ttu-id="f1ef5-571">New-AzureRmLogicApp에서 "매개 변수 집합을 확인할 수 없습니다" 오류 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-571">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="f1ef5-572">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f1ef5-572">AzureRM.Network</span></span>
* <span data-ttu-id="f1ef5-573">Set/Add-AzureRmVirtualNetworkPeering에 대한 여러 테넌트의 가상 네트워크에서 피어링을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-573">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="f1ef5-574">Application Gateway에 대한 아래 cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-574">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="f1ef5-575">New-AzureRmApplicationGateway: EnableFIPS 플래그 및 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-575">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="f1ef5-576">New-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-576">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="f1ef5-577">Set-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-577">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="f1ef5-578">최신 생성기를 사용하여 RouteTable cmdlet을 재생성</span><span class="sxs-lookup"><span data-stu-id="f1ef5-578">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="f1ef5-579">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="f1ef5-579">AzureRM.Relay</span></span>
* <span data-ttu-id="f1ef5-580">markdown 파일을 업데이트하여 예제에서 매개 변수 이름 문제에 대해 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-580">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="f1ef5-581">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="f1ef5-581">AzureRM.Resources</span></span>
* <span data-ttu-id="f1ef5-582">Roledefinition 및 Roleassignment cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-582">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="f1ef5-583">페이징의 일부분으로 수행하는 추가 roledefinition 호출을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-583">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="f1ef5-584">Get-AzureRmRoleAssignment cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-584">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="f1ef5-585">-ExpandPrincipalGroups 명령 매개 변수 기능 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-585">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="f1ef5-586">'Get-AzureRmResource'에서 '-ResourceType' 매개 변수가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-586">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="f1ef5-587">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f1ef5-587">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="f1ef5-588">top 및 skip 매개 변수가 cmdlet 목록을 나열하도록 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-588">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="f1ef5-589">표준을 프리미엄 네임스페이스 마이그레이션 cmdlet에 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-589">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="f1ef5-590">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-590">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="f1ef5-591">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-591">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="f1ef5-592">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-592">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="f1ef5-593">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-593">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="f1ef5-594">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-594">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="f1ef5-595">PSServiceBusDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="f1ef5-595">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="f1ef5-596">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f1ef5-596">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="f1ef5-597">‘New-AzureRmServiceFabricCluster’에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-597">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="f1ef5-598">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="f1ef5-598">AzureRM.Sql</span></span>
* <span data-ttu-id="f1ef5-599">Management.Sql에 대한 새 cmdlet을 추가하여 고객이 TDE 인증서를 SQL Server 인스턴스 또는 Managed Instance에 추가할 수 있도록 허용</span><span class="sxs-lookup"><span data-stu-id="f1ef5-599">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="f1ef5-600">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="f1ef5-600">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="f1ef5-601">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="f1ef5-601">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="f1ef5-602">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="f1ef5-602">AzureRM.Websites</span></span>
* <span data-ttu-id="f1ef5-603">`Set-AzureRmWebApp -AssignIdentity` 및 `Set-AzureRmWebAppSlot -AssignIdentity`가 false로 설정되면 사이트 개체에서 Identity 속성이 제거됩니다. 미리보기 태그도 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-603">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="f1ef5-604">`Get-AzureRmWebAppMetrics`, `Get-AzureRmAppServicePlanMetrics` 예제가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-604">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="f1ef5-605">`Set-AzureRmWebApp -PhpVersion`이 유효한 php 버전으로 해제 지원</span><span class="sxs-lookup"><span data-stu-id="f1ef5-605">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="f1ef5-606">6.4.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="f1ef5-606">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="f1ef5-607">일반</span><span class="sxs-lookup"><span data-stu-id="f1ef5-607">General</span></span>
* <span data-ttu-id="f1ef5-608">대부분의 모듈에 대한 도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-608">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="f1ef5-609">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-609">AzureRM.Profile</span></span>
* <span data-ttu-id="f1ef5-610">기본 출력 형식에 추가된 Ps1Xml 특성</span><span class="sxs-lookup"><span data-stu-id="f1ef5-610">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="f1ef5-611">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f1ef5-611">AzureRM.Compute</span></span>
* <span data-ttu-id="f1ef5-612">VMSS에 대한 IP 태그 기능</span><span class="sxs-lookup"><span data-stu-id="f1ef5-612">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="f1ef5-613">'New-AzureRmVmssIpTagConfig' cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-613">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="f1ef5-614">New-AzureRmVmssIpConfig에 IpTag 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-614">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="f1ef5-615">VMSS에 대한 자동 OS 롤백 기능</span><span class="sxs-lookup"><span data-stu-id="f1ef5-615">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="f1ef5-616">New-AzureRmVmssConfig 및 Update-AzureRmVmss에 DisableAutoRollback 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-616">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="f1ef5-617">Vmss에 대한 OS 업그레이드 기록 기능</span><span class="sxs-lookup"><span data-stu-id="f1ef5-617">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="f1ef5-618">Get-AzureRmVmss에 OSUpgradeHistory 스위치 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-618">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="f1ef5-619">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="f1ef5-619">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="f1ef5-620">다음 명령을 통해 카탈로그 액세스 제어 목록에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-620">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="f1ef5-621">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="f1ef5-621">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="f1ef5-622">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="f1ef5-622">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="f1ef5-623">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="f1ef5-623">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="f1ef5-624">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f1ef5-624">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="f1ef5-625">Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl에 대한 취소 지원 및 진행률 추적 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-625">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="f1ef5-626">Export-AzureRmDataLakeStoreChildItemProperties에 대한 취소 지원 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-626">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="f1ef5-627">재귀 작업을 수행하는 cmdlet에 대한 디버그 메시지 플러시 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-627">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="f1ef5-628">DataLake cmdlet의 테스트 위치 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-628">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="f1ef5-629">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="f1ef5-629">AzureRM.EventHub</span></span>
* <span data-ttu-id="f1ef5-630">목록 작업 cmdlet Get-AzureRmEventHub 및 Get-AzureRmEventHubConsumerGroup에 선택적 MaxCount 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-630">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="f1ef5-631">새 EventHub 만드는 동안 하나 이상의 매개 변수가 필요한 New-AzureRmEventHub cmdlet 문제를 해결.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-631">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="f1ef5-632">기본 매개 변수 집합을 제공.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-632">Provided Default Parameter set.</span></span>
* <span data-ttu-id="f1ef5-633">선택적 매개 변수 -KeyValue를 New-AzureRmEventHubKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-633">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="f1ef5-634">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1ef5-634">AzureRM.KeyVault</span></span>
* <span data-ttu-id="f1ef5-635">Get-AzureRmKeyVault -Tag 실행 시 모든 리소스가 리턴되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-635">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="f1ef5-636">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f1ef5-636">AzureRM.Network</span></span>
* <span data-ttu-id="f1ef5-637">영역 중복 VirtualNetworkGateways에 대한 새 Sku를 노출합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-637">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="f1ef5-638">기능에 대한 새 명령이 추가됨: ARM을 통한 ExpressRoute Partner APIs</span><span class="sxs-lookup"><span data-stu-id="f1ef5-638">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="f1ef5-639">Get- AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-639">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="f1ef5-640">Set-AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-640">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="f1ef5-641">Add-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-641">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="f1ef5-642">Get-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-642">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="f1ef5-643">Remove-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-643">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="f1ef5-644">Get-AzureRMExpressRouteCrossConnectionArpTable 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-644">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="f1ef5-645">Get-AzureRMExpressRouteCrossConnectionRouteTable 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-645">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="f1ef5-646">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-646">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="f1ef5-647">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="f1ef5-647">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="f1ef5-648">Get-AzureRmRecoveryServicesBackupStatus cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-648">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="f1ef5-649">이 cmdlet은 VM ID를 가져와서 VM이 구독에서 일부 자격 증명 모음으로 보호되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-649">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="f1ef5-650">이러한 자격 증명 모음이 존재하는 경우 cmdlet은 자격 증명 모음 세부 정보를 출력 합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-650">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="f1ef5-651">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="f1ef5-651">AzureRM.Resources</span></span>
* <span data-ttu-id="f1ef5-652">Get-AzureRmPolicyAssignment cmdlet을 다음과 같이 업데이트함.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-652">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="f1ef5-653">관리 그룹 수준에서 -Scope 값 리스팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-653">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="f1ef5-654">관리 그룹 수준에서 -Scope 값을 사용하여 개별 할당값을 검색하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-654">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="f1ef5-655">제어 매개 변수에 -Effective 및 -All 스위치 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-655">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="f1ef5-656">Get/New/Remove/Set-AzureRmPolicyDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-656">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="f1ef5-657">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-657">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="f1ef5-658">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-658">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="f1ef5-659">Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-659">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="f1ef5-660">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-660">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="f1ef5-661">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-661">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="f1ef5-662">'New-AzureRmResourceGroupDeployment'에서 'TemplateParameterObject'를 사용하는 경우 매개 변수에 KeyVault 비밀 참조 지원 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-662">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="f1ef5-663">'New-AzureRmADAppCredential'에 대해 '-EndDate' 매개 변수가 무시되는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-663">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="f1ef5-664">'Add-AzureRmADGroupMember'가 요청에 잘못된 URL을 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-664">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="f1ef5-665">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f1ef5-665">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="f1ef5-666">선택적 매개 변수 -KeyValue를 New-AzureRmServiceBusKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-666">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="f1ef5-667">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="f1ef5-667">AzureRM.Sql</span></span>
* <span data-ttu-id="f1ef5-668">New-AzureRmSqlDatabaseRestorePoint 도움말에서 SQLDW에 대한 사용자 정의 복원 지점 명시</span><span class="sxs-lookup"><span data-stu-id="f1ef5-668">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="f1ef5-669">몇 가지 cmdlet에서-ComputeGeneration 매개 변수의 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-669">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="f1ef5-670">6.3.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="f1ef5-670">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="f1ef5-671">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-671">AzureRM.Profile</span></span>
* <span data-ttu-id="f1ef5-672">Enable-AzureRmContextAutoSave에 대한 오류 메시지 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-672">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="f1ef5-673">이전 컨텍스트 없이 'Connect-AzureRmAccount' 실행 시 각 구독에 대한 컨텍스트 생성</span><span class="sxs-lookup"><span data-stu-id="f1ef5-673">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="f1ef5-674">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="f1ef5-674">Azure.Storage</span></span>
* <span data-ttu-id="f1ef5-675">도움말 파일 내 -Permissions 매개 변수에 대한 추가 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-675">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="f1ef5-676">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f1ef5-676">AzureRM.Compute</span></span>
* <span data-ttu-id="f1ef5-677">'Get-AzureRmVmDiskEncryptionStatus'가 데이터 디스크가 없는 VM에 대해 관찰된 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-677">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="f1ef5-678">Compute 클라이언트 라이브러리 버전을 업데이트하여 다음 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-678">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="f1ef5-679">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="f1ef5-679">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="f1ef5-680">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="f1ef5-680">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="f1ef5-681">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="f1ef5-681">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="f1ef5-682">다음 cmdlet이 '작업 ID' 및 '작업 상태'를 올바르게 표시하도록 수정:</span><span class="sxs-lookup"><span data-stu-id="f1ef5-682">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="f1ef5-683">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="f1ef5-683">Start-AzureRmVM</span></span>
    - <span data-ttu-id="f1ef5-684">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="f1ef5-684">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="f1ef5-685">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="f1ef5-685">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="f1ef5-686">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="f1ef5-686">Set-AzureRmVM</span></span>
    - <span data-ttu-id="f1ef5-687">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="f1ef5-687">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="f1ef5-688">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="f1ef5-688">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="f1ef5-689">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="f1ef5-689">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="f1ef5-690">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="f1ef5-690">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="f1ef5-691">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="f1ef5-691">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="f1ef5-692">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="f1ef5-692">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="f1ef5-693">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="f1ef5-693">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="f1ef5-694">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="f1ef5-694">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="f1ef5-695">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="f1ef5-695">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="f1ef5-696">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="f1ef5-696">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="f1ef5-697">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="f1ef5-697">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="f1ef5-698">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="f1ef5-698">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="f1ef5-699">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="f1ef5-699">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="f1ef5-700">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="f1ef5-700">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="f1ef5-701">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="f1ef5-701">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="f1ef5-702">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="f1ef5-702">AzureRM.EventGrid</span></span>
* <span data-ttu-id="f1ef5-703">Update-AzureRmEventGridSubscription cmdlet의 SubjectBeginsWith/SubjectEndsWith에 대한 ValidateNotNullOrEmpty 유효성 검사 조건을 제거하여 필요에 따라 이러한 매개 변수를 빈 문자열로 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-703">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="f1ef5-704">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1ef5-704">AzureRM.KeyVault</span></span>
* <span data-ttu-id="f1ef5-705">Get-AzureRmKeyVault -Tag 실행 시 태그가 리턴되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-705">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="f1ef5-706">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="f1ef5-706">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="f1ef5-707">Policy Insights cmdlet의 공개 릴리스</span><span class="sxs-lookup"><span data-stu-id="f1ef5-707">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="f1ef5-708">API 버전 2018-04-04 사용</span><span class="sxs-lookup"><span data-stu-id="f1ef5-708">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="f1ef5-709">PolicyDefinitionReferenceId를 Get-AzureRmPolicyStateSummary의 결과 집합에 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-709">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="f1ef5-710">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="f1ef5-710">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="f1ef5-711">-Vault 매개 변수를 RecoveryServices.Backup cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-711">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="f1ef5-712">전달되는 경우 이는 Set-AzureRmRecoveryServicesContext cmdlet을 재정의함.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-712">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="f1ef5-713">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="f1ef5-713">AzureRM.Sql</span></span>
* <span data-ttu-id="f1ef5-714">Get-AzureRmSqlDatabaseExpanded에 대한 도움말 파일의 예가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-714">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="f1ef5-715">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="f1ef5-715">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="f1ef5-716">Add-AzureRmTrafficManagerEndpointConfig에대한 도움말 파일이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-716">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="f1ef5-717">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="f1ef5-717">AzureRM.Websites</span></span>
* <span data-ttu-id="f1ef5-718">-AssignIdentity를 사용할 때 AppSetting을 덮어쓰지 않도록 'Set-AzureRmWebApp'이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-718">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="f1ef5-719">'New-AzureRmWebAppSlot'이 AppServicePlan을 옵션 매개변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-719">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="f1ef5-720">6.2.1 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="f1ef5-720">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="f1ef5-721">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="f1ef5-721">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="f1ef5-722">PSWorkspace 모델이 Network 형식을 매개 변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-722">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="f1ef5-723">6.2.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="f1ef5-723">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="f1ef5-724">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-724">AzureRM.Profile</span></span>
* <span data-ttu-id="f1ef5-725">Newtonsoft.Json의 버전 10.0.3이 모듈 가져오기에 로드되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-725">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="f1ef5-726">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f1ef5-726">AzureRM.Compute</span></span>
* <span data-ttu-id="f1ef5-727">VMSS VM 업데이트 기능</span><span class="sxs-lookup"><span data-stu-id="f1ef5-727">VMSS VM Update feature</span></span>
    - <span data-ttu-id="f1ef5-728">'Update-AzureRmVmssVM' 및 'New-AzureRmVMDataDisk' cmdlets 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-728">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="f1ef5-729">데이터 디스크를 Vmss VM에 추가할 수 있도록 지원하기 위해 VirtualMachineScaleSetVM 매개변수를 'Add-AzureRmVMDataDisk' cmdlet에 추가하였습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-729">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="f1ef5-730">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="f1ef5-730">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="f1ef5-731">ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.8.0-preview로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-731">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="f1ef5-732">팩터리 리포지토리 작업 구성 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-732">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="f1ef5-733">QuickBooks LinkedService가 ConsumerKey 및 consumerSecret 속성을 노출하도록 업데이트됨 </span><span class="sxs-lookup"><span data-stu-id="f1ef5-733">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="f1ef5-734">여러 모델 유형을 SecretBase에서 개체로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="f1ef5-734">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="f1ef5-735">Blob 이벤트 트리거 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-735">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="f1ef5-736">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1ef5-736">AzureRM.KeyVault</span></span>
* <span data-ttu-id="f1ef5-737">예제 출력으로 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-737">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="f1ef5-738">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f1ef5-738">AzureRM.Network</span></span>
* <span data-ttu-id="f1ef5-739">Network Watcher cmdlet에서 트래픽 분석 매개 변수를 사용가능하도록 설정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-739">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="f1ef5-740">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="f1ef5-740">AzureRM.Resources</span></span>
* <span data-ttu-id="f1ef5-741">'Get AzureRmResource'에서 반환된 'PSResource' 개체의 'Properties' 속성의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-741">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="f1ef5-742">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="f1ef5-742">AzureRM.Scheduler</span></span>
* <span data-ttu-id="f1ef5-743">ServiceBusQueueJob 업데이트가 새 인증 값을 설정하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f1ef5-743">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="f1ef5-744">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="f1ef5-744">AzureRM.Sql</span></span>
* <span data-ttu-id="f1ef5-745">옵션 LicenseType 매개 변수를 사용하여 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="f1ef5-745">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="f1ef5-746">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="f1ef5-746">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="f1ef5-747">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="f1ef5-747">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="f1ef5-748">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="f1ef5-748">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="f1ef5-749">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="f1ef5-749">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="f1ef5-750">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="f1ef5-750">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="f1ef5-751">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="f1ef5-751">AzureRM.Websites</span></span>
* <span data-ttu-id="f1ef5-752">'New-AzureRMWebApp'이 전략 라이브러리의 공통 알고리즘을 사용하도록 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-752">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="f1ef5-753">6.1.0 - 2018년 5월</span><span class="sxs-lookup"><span data-stu-id="f1ef5-753">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="f1ef5-754">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f1ef5-754">AzureRM.Profile</span></span>
* <span data-ttu-id="f1ef5-755">'Clear-AzureRmContext'를 실행하면 이전 기본 컨텍스트의 이름으로 빈 컨텍스트가 유지되어 사용자가 이전 이름으로 새 컨텍스트를 만들지 못하게 되는 문제를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-755">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="f1ef5-756">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="f1ef5-756">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="f1ef5-757">AS에서 게이트웨이가 작업을 연결하거나 연결 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-757">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="f1ef5-758">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f1ef5-758">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="f1ef5-759">ApiVersions, ApiReleases 및 ApiRevisions에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-759">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="f1ef5-760">ServiceFabric 백 엔드에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-760">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="f1ef5-761">Application Insights 로거에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-761">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="f1ef5-762">'기본' SKU를 API Management 서비스의 유효한 SKU로 인식하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-762">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="f1ef5-763">개인 CA가 발급한 인증서를 루트 또는 CA로 설치하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-763">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="f1ef5-764">KeyVault 및 다중 프록시 호스트 이름을 통한 사용자 정의 SSL 인증서를 수락하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-764">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="f1ef5-765">MSI ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="f1ef5-765">Added support for MSI identity</span></span>
* <span data-ttu-id="f1ef5-766">URL을 통한 정책을 수락하는 지원 추가됨 참고: 다음 cmdlet은 이후 릴리스에서 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-766">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="f1ef5-767">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="f1ef5-767">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="f1ef5-768">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-768">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="f1ef5-769">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="f1ef5-769">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="f1ef5-770">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="f1ef5-770">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="f1ef5-771">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="f1ef5-771">AzureRM.Batch</span></span>
* <span data-ttu-id="f1ef5-772">새 cmdlet Get AzureBatchPoolNodeCounts 릴리스</span><span class="sxs-lookup"><span data-stu-id="f1ef5-772">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="f1ef5-773">새 cmdlet Start-AzureBatchComputeNodeServiceLogUpload 릴리스</span><span class="sxs-lookup"><span data-stu-id="f1ef5-773">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="f1ef5-774">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="f1ef5-774">AzureRM.Consumption</span></span>
* <span data-ttu-id="f1ef5-775">Expand, ResourceGroup, InstanceName, InstanceId, Tags, Top on Cmdlet Get-AzureRmConsumptionUsageDetail 등 새 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="f1ef5-775">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="f1ef5-776">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f1ef5-776">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="f1ef5-777">Export-AzureRmDataLakeStoreChildItemProperties에 대한 예제 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-777">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="f1ef5-778">Set-AzureRmDataLakeStoreItemAclEntry에서 재귀 사례에 대한 null 매개 변수 예외 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-778">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="f1ef5-779">Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry에 대한 도움말 파일 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-779">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="f1ef5-780">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f1ef5-780">AzureRM.Network</span></span>
* <span data-ttu-id="f1ef5-781">18.0.0-preview에서 19.0.0-preview로 네트워크 SDK 버전 업그레이드</span><span class="sxs-lookup"><span data-stu-id="f1ef5-781">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="f1ef5-782">프로토콜 구성을 만들기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="f1ef5-782">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="f1ef5-783">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ef5-783">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="f1ef5-784">기존 Express 경로 회로에 새 회로 연결을 추가하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="f1ef5-784">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="f1ef5-785">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-785">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="f1ef5-786">기존 Express 경로 회로에서 회로 연결을 제거하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="f1ef5-786">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="f1ef5-787">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-787">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="f1ef5-788">회로 연결을 검색하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="f1ef5-788">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="f1ef5-789">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="f1ef5-789">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="f1ef5-790">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f1ef5-790">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="f1ef5-791">생성된 인증서로 고정 서버 인증 사용(문제 # 5998)</span><span class="sxs-lookup"><span data-stu-id="f1ef5-791">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="f1ef5-792">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="f1ef5-792">AzureRM.Sql</span></span>
* <span data-ttu-id="f1ef5-793">AuditActions 또는 AuditActionGroups를 제거할 수 있도록 업데이트된 감사 cmdlet</span><span class="sxs-lookup"><span data-stu-id="f1ef5-793">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="f1ef5-794">'Azure 복구 서비스 자격 증명 모음을 사용하여 장기 보존 정책을 구성하면 정책이 더 이상 지원되지 않습니다. 새로운 유연 보유 정책으로 요청을 제출하십시오.'라는 메시지와 함께 명령이 실패하는 새로운 유연 보유 정책을 설정할 때</span><span class="sxs-lookup"><span data-stu-id="f1ef5-794">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="f1ef5-795">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy의 문제 수정</span><span class="sxs-lookup"><span data-stu-id="f1ef5-795">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="f1ef5-796">Azure SQL Database/ElasticPool Creation/Update 관련 cmdlet을 모두 업데이트하여 규모 및 계층 관련 속성에 대한 SKU 속성을 지원하는 새 데이터베이스 API를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-796">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="f1ef5-797">업데이트된 cmdlet는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-797">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="f1ef5-798">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="f1ef5-798">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="f1ef5-799">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="f1ef5-799">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="f1ef5-800">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="f1ef5-800">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="f1ef5-801">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="f1ef5-801">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="f1ef5-802">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="f1ef5-802">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="f1ef5-803">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="f1ef5-803">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="f1ef5-804">-Name 매개 변수를 사용할 때 -ResourceGroupName 매개 변수가 필요하도록 'Get-AzureRmTrafficManagerProfile'에 대한 매개 변수를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="f1ef5-804">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
