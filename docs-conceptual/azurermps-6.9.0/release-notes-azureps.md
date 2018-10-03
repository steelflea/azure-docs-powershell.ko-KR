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
ms.openlocfilehash: 3cb71087a61a0fcd06c014394e8f9e5654d4c1a8
ms.sourcegitcommit: 19dffee617477001f98d43e39a50ce1fad087b74
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/27/2018
ms.locfileid: "47179006"
---
# <a name="release-notes"></a><span data-ttu-id="1ef66-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="1ef66-103">Release notes</span></span>

<span data-ttu-id="1ef66-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="690---september-2018"></a><span data-ttu-id="1ef66-105">6.9.0 - 2018년 9월</span><span class="sxs-lookup"><span data-stu-id="1ef66-105">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="1ef66-106">일반</span><span class="sxs-lookup"><span data-stu-id="1ef66-106">General</span></span>
* <span data-ttu-id="1ef66-107">AzureRM.SignalR이 AzureRM 롤업 모듈에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-107">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="1ef66-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1ef66-108">AzureRM.Profile</span></span>
* <span data-ttu-id="1ef66-109">저장소 일반 코드에 대한 약간의 변경</span><span class="sxs-lookup"><span data-stu-id="1ef66-109">Minor changes to the storage common code</span></span>
* <span data-ttu-id="1ef66-110">전체 매개 변수 형식을 포함하도록 도움말 파일이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-110">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="1ef66-111">-ServicePrincipal을 필수가 아닌 것으로 ServicePrincipalCertificateWithSubscriptionId 매개변수 집합에서 변경</span><span class="sxs-lookup"><span data-stu-id="1ef66-111">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="1ef66-112">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1ef66-112">Azure.Storage</span></span>
* <span data-ttu-id="1ef66-113">OAuth를 사용하여 저장소 컨텍스트를 만드는 것을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-113">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="1ef66-114">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="1ef66-114">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="1ef66-115">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="1ef66-115">AzureRM.Cdn</span></span>
* <span data-ttu-id="1ef66-116">Cdn 가격 책정 sku에서 Standard_Microsoft를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-116">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="1ef66-117">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1ef66-117">AzureRM.Compute</span></span>
* <span data-ttu-id="1ef66-118">Keyvault 및 Storage에서 종속성을 일반 종속성으로 이동</span><span class="sxs-lookup"><span data-stu-id="1ef66-118">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="1ef66-119">AEM cmdlet에 더 많은 가상 머신 크기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-119">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="1ef66-120">PublicIPPrefix 매개 변수를 New-AzureRmVmssIpConfig에 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-120">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="1ef66-121">Invoke-AzureRmVMRunCommand cmdelt에 ResourceId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-121">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="1ef66-122">Invoke-AzureRmVmssVMRunCommand cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-122">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="1ef66-123">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="1ef66-123">AzureRM.Dns</span></span>
* <span data-ttu-id="1ef66-124">Dns 레코드를 만드는 동안 별칭 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-124">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="1ef66-125">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="1ef66-125">AzureRM.Insights</span></span>
* <span data-ttu-id="1ef66-126">#6833 및 #7102 문제 수정(진단 설정 영역)</span><span class="sxs-lookup"><span data-stu-id="1ef66-126">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="1ef66-127">기본 이름, 즉 'service'에 진단 설정의 목록 생성 및 가져오는 동안에 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-127">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="1ef66-128">범주를 사용하는 진단 설정 만들기 문제</span><span class="sxs-lookup"><span data-stu-id="1ef66-128">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="1ef66-129">메트릭 시간 조직 매개 변수에 대한 사용 중단 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-129">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="1ef66-130">Timegrains 매개 변수는 여전히 받아들여지고 있습니다(이것은 호환성이 손상되는 변경이 아닙니다). 그러나 PT1M만 유효하므로 백엔드에서 무시됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-130">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="1ef66-131">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1ef66-131">AzureRM.Network</span></span>
* <span data-ttu-id="1ef66-132">LoadBalancer cmdlet에 대한 변경</span><span class="sxs-lookup"><span data-stu-id="1ef66-132">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="1ef66-133">LoadBalancerInboundNatPoolConfig: IdleTimeoutInMinutes, EnableFloatingIp 및 EnableTcpReset 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-133">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="1ef66-134">LoadBalancerInboundNatRuleConfig: EnableTcpReset 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-134">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="1ef66-135">LoadBalancerRuleConfig: EnableTcpReset 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-135">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="1ef66-136">LoadBalancerProbeConfig: 매개 변수 프로토콜에 대해 "Https" 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-136">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="1ef66-137">새 LoadBalancer의 하위 리소스OutboundRule에 대한 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-137">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="1ef66-138">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-138">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="1ef66-139">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-139">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="1ef66-140">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-140">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="1ef66-141">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-141">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="1ef66-142">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-142">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="1ef66-143">PSNetworkInterface에 대한 새 HostedWorkloads 속성 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-143">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="1ef66-144">기능에 대한 새 cmdlet 추가: ARM을 통한 Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="1ef66-144">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="1ef66-145">Get-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-145">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="1ef66-146">Set-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-146">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="1ef66-147">New-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-147">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="1ef66-148">Remove-AzureRmFirewall 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-148">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="1ef66-149">New-AzureRmFirewallApplicationRuleCollection 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-149">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="1ef66-150">New-AzureRmFirewallApplicationRule 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-150">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="1ef66-151">New-AzureRmFirewallNatRuleCollection 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-151">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="1ef66-152">New-AzureRmFirewallNatRule 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-152">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="1ef66-153">New-AzureRmFirewallNetworkRuleCollection 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-153">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="1ef66-154">New-AzureRmFirewallNetworkRule 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-154">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="1ef66-155">Application Gateway에서 신뢰할 수 있는 루트 인증서 및 크기 자동 조정 구성에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-155">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="1ef66-156">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-156">New Cmdlets added:</span></span>
      - <span data-ttu-id="1ef66-157">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1ef66-157">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="1ef66-158">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1ef66-158">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="1ef66-159">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1ef66-159">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="1ef66-160">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1ef66-160">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="1ef66-161">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1ef66-161">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="1ef66-162">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ef66-162">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="1ef66-163">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ef66-163">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="1ef66-164">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ef66-164">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="1ef66-165">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ef66-165">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="1ef66-166">옵션 매개 변수를 사용하도록 업데이트된 Cmdlet-TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1ef66-166">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="1ef66-167">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="1ef66-167">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="1ef66-168">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="1ef66-168">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="1ef66-169">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="1ef66-169">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="1ef66-170">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="1ef66-170">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="1ef66-171">옵션 매개 변수를 사용하도록 업데이트된 Cmdlet-AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ef66-171">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="1ef66-172">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="1ef66-172">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="1ef66-173">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="1ef66-173">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="1ef66-174">인터페이스 엔드포인트 Get-AzureInterfaceEndpoint에 대한 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-174">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="1ef66-175">서브넷에서 여러 주소 접두사에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-175">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="1ef66-176">다음 Cmdlet이 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-176">Updated cmdlets:</span></span>
  - <span data-ttu-id="1ef66-177">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-177">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="1ef66-178">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-178">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="1ef66-179">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-179">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="1ef66-180">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-180">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="1ef66-181">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="1ef66-181">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="1ef66-182">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-182">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="1ef66-183">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-183">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="1ef66-184">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-184">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="1ef66-185">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ef66-185">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="1ef66-186">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ef66-186">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="1ef66-187">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ef66-187">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="1ef66-188">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-188">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="1ef66-189">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-189">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="1ef66-190">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-190">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="1ef66-191">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-191">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="1ef66-192">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-192">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="1ef66-193">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-193">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="1ef66-194">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-194">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="1ef66-195">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="1ef66-195">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="1ef66-196">서브넷 위임에 대한 cmdlet을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-196">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="1ef66-197">New-AzureRmDelegation: 서브넷에 추가할 수 있는 새 위임을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-197">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="1ef66-198">Remove-AzureRmDelegation: 서브넷에서 가져와서 해당 서브넷에서 제공된 위임 이름을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-198">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="1ef66-199">Add-AzureRmDelegation: 서브넷에서 사용 및 제공된 서비스 이름을 해당 서브넷에 대한 위임으로 추가합니다</span><span class="sxs-lookup"><span data-stu-id="1ef66-199">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="1ef66-200">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="1ef66-200">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="1ef66-201">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="1ef66-201">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="1ef66-202">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="1ef66-202">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="1ef66-203">관리되는 관리 디스크에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="1ef66-203">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="1ef66-204">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1ef66-204">AzureRM.RedisCache</span></span>
* <span data-ttu-id="1ef66-205">인사이트 종속성이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-205">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="1ef66-206">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="1ef66-206">AzureRM.Resources</span></span>
* <span data-ttu-id="1ef66-207">New-AzureRmResourceGroupDeployment를 RollbackAction 새 매개 변수를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-207">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="1ef66-208">새 매개 변수를 사용하여 OnErrorDeployment에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-208">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="1ef66-209">정책 할당에서 관리되는 ID를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-209">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="1ef66-210">'New-AzureRmPolicyAssignment'를 사용하여 정책을 할당할 때 기본값이 있는 매개 변수는 더 이상 필요하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-210">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="1ef66-211">정책 별칭을 검색하기 위한 새 cmdlet Get-AzureRmPolicyAlias 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-211">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="1ef66-212">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1ef66-212">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="1ef66-213">#7161 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-213">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="1ef66-214">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="1ef66-214">AzureRM.SignalR</span></span>
* <span data-ttu-id="1ef66-215">SKU 이름을 Free_F1 및 Standard_S1로 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-215">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="1ef66-216">버전 필드를 PSSignalRResource 개체에 추가하고 연결 문자열을 PSSignalRKeys개체에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-216">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="1ef66-217">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="1ef66-217">AzureRM.Storage</span></span>
* <span data-ttu-id="1ef66-218">AzureRm.Storage에서 불변성 정책 지원</span><span class="sxs-lookup"><span data-stu-id="1ef66-218">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="1ef66-219">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="1ef66-219">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="1ef66-220">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="1ef66-220">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="1ef66-221">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="1ef66-221">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="1ef66-222">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="1ef66-222">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="1ef66-223">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="1ef66-223">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="1ef66-224">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="1ef66-224">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="1ef66-225">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="1ef66-225">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="1ef66-226">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="1ef66-226">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="1ef66-227">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="1ef66-227">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="1ef66-228">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="1ef66-228">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="1ef66-229">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="1ef66-229">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="1ef66-230">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="1ef66-230">AzureRM.Websites</span></span>
* <span data-ttu-id="1ef66-231">두 개의 새로운 cmdlet 추가: Get-AzureRmDeletedWebApp 및 Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="1ef66-231">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="1ef66-232">New-AzureRmAppServicePlan -HyperV 스위치가 창 컨테이너가 있는 앱 서비스 계획 작성용으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-232">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="1ef66-233">New-AzureRmWebApp/New-AzureRmWebAppSlot/Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - Windows 컨테이너 앱을 만들고 관리하기 위한 새 매개 변수(-ContainerRegistryUser 문자열 -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment)가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-233">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="1ef66-234">6.8.1 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="1ef66-234">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="1ef66-235">일반</span><span class="sxs-lookup"><span data-stu-id="1ef66-235">General</span></span>
* <span data-ttu-id="1ef66-236">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-236">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="1ef66-237">공용 런타임 어셈블리가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-237">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="1ef66-238">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1ef66-238">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="1ef66-239">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-239">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="1ef66-240">문제 https://github.com/Azure/azure-powershell/issues/6603 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-240">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="1ef66-241">Import-AzureRmApiManagementApi 및 \*-AzureRmApiManagementCertificate cmdlet은 이제 상대 경로를 처리합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-241">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="1ef66-242">문제 https://github.com/Azure/azure-powershell/issues/6879 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-242">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="1ef66-243">CertificateInformation은 Set-AzureRmApiManagement cmdlet이 제대로 작동 하게 하는 설정 가능한 속성입니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-243">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="1ef66-244">4.0.4-preview nuget으로 업그레이드하여 해결됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-244">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="1ef66-245">문제 https://github.com/Azure/azure-powershell/issues/6853 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-245">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="1ef66-246">제품에서 이름별 검색에 대해 Odata 필터가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-246">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="1ef66-247">문제 https://github.com/Azure/azure-powershell/issues/6814 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-247">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="1ef66-248">API에서 이름별 검색에 대해 Odata 필터가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-248">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="1ef66-249">AzureMonitor 로거에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-249">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="1ef66-250">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1ef66-250">AzureRM.Compute</span></span>
* <span data-ttu-id="1ef66-251">오류 출력에 대상이 없는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-251">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="1ef66-252">관리 디스크를 사용하는 VM에 대한 저장소 계정 유형 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-252">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="1ef66-253">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-253">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="1ef66-254">예를 들어 Azure 중국과 같이, 다른 환경에 대한 AEM 확장 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-254">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="1ef66-255">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1ef66-255">AzureRM.Network</span></span>
* <span data-ttu-id="1ef66-256">기본 cmdlet 출력 표시를 테이블 뷰로 변경</span><span class="sxs-lookup"><span data-stu-id="1ef66-256">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="1ef66-257">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="1ef66-257">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="1ef66-258">일시 중지된 용량을 확장하려고 할 때 Update-AzureRmPowerBIEmbeddedCapacity 실패 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-258">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="1ef66-259">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="1ef66-259">AzureRM.Resources</span></span>
* <span data-ttu-id="1ef66-260">MarketPlace에서 관리되는 응용 프로그램 생성 시의 문제 해결.</span><span class="sxs-lookup"><span data-stu-id="1ef66-260">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="1ef66-261">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1ef66-261">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="1ef66-262">해결된 문제</span><span class="sxs-lookup"><span data-stu-id="1ef66-262">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="1ef66-263">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="1ef66-263">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="1ef66-264">다중값 라우팅 메서드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-264">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="1ef66-265">다중값 라우팅에 대한 새 매개 변수 'MaxReturn'</span><span class="sxs-lookup"><span data-stu-id="1ef66-265">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="1ef66-266">서브넷 라우팅 메서드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-266">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="1ef66-267">엔드포인트의 IP 주소 범위(서브넷)에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="1ef66-267">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="1ef66-268">프로필 내 사용자 지정 헤더에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-268">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="1ef66-269">프로필 내 예상 상태 코드 범위에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-269">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="1ef66-270">엔드포인트 내 사용자 지정 헤더에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-270">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="1ef66-271">6.8.0 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="1ef66-271">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="1ef66-272">일반</span><span class="sxs-lookup"><span data-stu-id="1ef66-272">General</span></span>
* <span data-ttu-id="1ef66-273">기본 리소스 그룹이 설정되지 않는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-273">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="1ef66-274">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1ef66-274">AzureRM.Profile</span></span>
* <span data-ttu-id="1ef66-275">Connect-AzureRmAccount 중에 반환된 토큰에 만료 속성 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-275">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="1ef66-276">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1ef66-276">AzureRM.Compute</span></span>
* <span data-ttu-id="1ef66-277">오류 출력에 대상이 없는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-277">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="1ef66-278">관리 디스크를 사용하는 VM에 대한 저장소 계정 유형 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-278">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="1ef66-279">예를 들어 Azure 중국과 같이, 다른 환경에 대한 AEM 확장 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-279">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="1ef66-280">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="1ef66-280">AzureRM.IotHub</span></span>
* <span data-ttu-id="1ef66-281">New-AzureRmIotHubExportDevices 및 New-AzureRmIotHubImportDevices에 대한 예제를 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-281">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="1ef66-282">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1ef66-282">AzureRM.Network</span></span>
* <span data-ttu-id="1ef66-283">기본 모델 표시를 테이블 뷰로 변경</span><span class="sxs-lookup"><span data-stu-id="1ef66-283">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="1ef66-284">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="1ef66-284">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="1ef66-285">일시 중지된 용량을 확장하려고 할 때 Update-AzureRmPowerBIEmbeddedCapacity 실패 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-285">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="1ef66-286">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="1ef66-286">AzureRM.Resources</span></span>
* <span data-ttu-id="1ef66-287">MarketPlace에서 관리되는 응용 프로그램 생성 시의 문제 해결.</span><span class="sxs-lookup"><span data-stu-id="1ef66-287">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="1ef66-288">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1ef66-288">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="1ef66-289">문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-289">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="1ef66-290">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="1ef66-290">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="1ef66-291">다중값 라우팅 메서드에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="1ef66-291">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="1ef66-292">다중값 라우팅에 대한 새 매개 변수 'MaxReturn'</span><span class="sxs-lookup"><span data-stu-id="1ef66-292">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="1ef66-293">서브넷 라우팅 메서드에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="1ef66-293">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="1ef66-294">엔드포인트의 IP 주소 범위(서브넷)에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="1ef66-294">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="1ef66-295">프로필 내 사용자 지정 헤더에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="1ef66-295">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="1ef66-296">프로필 내 예상 상태 코드 범위에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="1ef66-296">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="1ef66-297">엔드포인트 내 사용자 지정 헤더에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="1ef66-297">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="1ef66-298">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="1ef66-298">AzureRM.Websites</span></span>
* <span data-ttu-id="1ef66-299">기본 리소스 그룹이 잘못 설정되는 문제를 해결했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-299">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="1ef66-300">6.7.0 - 2018년 8월</span><span class="sxs-lookup"><span data-stu-id="1ef66-300">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="1ef66-301">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1ef66-301">AzureRM.Profile</span></span>
* <span data-ttu-id="1ef66-302">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-302">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="1ef66-303">충돌을 방지하려면 기본 컨텍스트 이름으로 사용자 ID를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-303">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="1ef66-304">#6398 컨텍스트를 선택할 때 문제를 발생시킨 Clear-AzureRmContext 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-304">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="1ef66-305">'Connect-AzureRmAccount'에 대한 '-TenantId' 매개 변수에 전달할 테넌트 도메인을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="1ef66-305">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="1ef66-306">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1ef66-306">Azure.Storage</span></span>
* <span data-ttu-id="1ef66-307">Azure 파일 공유 할당량에 대한 5TB 제한 제거</span><span class="sxs-lookup"><span data-stu-id="1ef66-307">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="1ef66-308">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="1ef66-308">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="1ef66-309">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1ef66-309">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="1ef66-310">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-310">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="1ef66-311">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1ef66-311">Azure.AnalysisServices</span></span>
* <span data-ttu-id="1ef66-312">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-312">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="1ef66-313">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1ef66-313">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="1ef66-314">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-314">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="1ef66-315">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="1ef66-315">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="1ef66-316">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-316">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="1ef66-317">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="1ef66-317">AzureRM.Automation</span></span>
* <span data-ttu-id="1ef66-318">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-318">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="1ef66-319">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="1ef66-319">AzureRM.Backup</span></span>
* <span data-ttu-id="1ef66-320">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-320">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="1ef66-321">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="1ef66-321">AzureRM.Batch</span></span>
* <span data-ttu-id="1ef66-322">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-322">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="1ef66-323">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="1ef66-323">AzureRM.Billing</span></span>
* <span data-ttu-id="1ef66-324">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-324">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="1ef66-325">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="1ef66-325">AzureRM.Cdn</span></span>
* <span data-ttu-id="1ef66-326">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-326">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="1ef66-327">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1ef66-327">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="1ef66-328">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-328">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="1ef66-329">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1ef66-329">AzureRM.Compute</span></span>
* <span data-ttu-id="1ef66-330">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-330">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="1ef66-331">New-AzureRmVmssConfig에 EvictionPolicy 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-331">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="1ef66-332">지정된 위치가 없는 경우에 New-AzureRmVm의 DiskFileParameterSet 내의 기본 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-332">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="1ef66-333">Save-AzureRmVMImage에서 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-333">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="1ef66-334">특정 singlepass 관련 시나리오에 대해 Get-AzureRmVMDiskEncryptionStatus cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-334">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="1ef66-335">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="1ef66-335">AzureRM.Consumption</span></span>
* <span data-ttu-id="1ef66-336">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-336">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="1ef66-337">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1ef66-337">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="1ef66-338">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-338">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="1ef66-339">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="1ef66-339">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="1ef66-340">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-340">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="1ef66-341">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="1ef66-341">AzureRM.DataFactories</span></span>
* <span data-ttu-id="1ef66-342">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-342">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="1ef66-343">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="1ef66-343">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="1ef66-344">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-344">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="1ef66-345">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="1ef66-345">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="1ef66-346">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-346">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="1ef66-347">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1ef66-347">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="1ef66-348">DebugPreference가 powershell 명령줄에서 설정된 경우 디버깅 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-348">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="1ef66-349">Set-AzureRmDataLakeStoreItemAcl에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-349">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="1ef66-350">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-350">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="1ef66-351">Set-AzureRmDataLakeStoreItemAclEntry에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-351">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="1ef66-352">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="1ef66-352">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="1ef66-353">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-353">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="1ef66-354">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="1ef66-354">AzureRM.Dns</span></span>
* <span data-ttu-id="1ef66-355">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-355">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="1ef66-356">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1ef66-356">AzureRM.EventGrid</span></span>
* <span data-ttu-id="1ef66-357">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-357">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="1ef66-358">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="1ef66-358">AzureRM.EventHub</span></span>
* <span data-ttu-id="1ef66-359">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-359">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="1ef66-360">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="1ef66-360">AzureRM.HDInsight</span></span>
* <span data-ttu-id="1ef66-361">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-361">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="1ef66-362">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="1ef66-362">AzureRM.Insights</span></span>
* <span data-ttu-id="1ef66-363">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-363">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="1ef66-364">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="1ef66-364">AzureRM.IotHub</span></span>
* <span data-ttu-id="1ef66-365">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-365">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="1ef66-366">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1ef66-366">AzureRM.KeyVault</span></span>
* <span data-ttu-id="1ef66-367">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-367">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="1ef66-368">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1ef66-368">AzureRM.LogicApp</span></span>
* <span data-ttu-id="1ef66-369">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-369">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="1ef66-370">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="1ef66-370">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="1ef66-371">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-371">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="1ef66-372">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="1ef66-372">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="1ef66-373">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-373">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="1ef66-374">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="1ef66-374">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="1ef66-375">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-375">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="1ef66-376">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="1ef66-376">AzureRM.Media</span></span>
* <span data-ttu-id="1ef66-377">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-377">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="1ef66-378">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1ef66-378">AzureRM.Network</span></span>
* <span data-ttu-id="1ef66-379">Set-AzureRmLocalNetworkGateway에 대한 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-379">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="1ef66-380">Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey, New-AzureRmVirtualNetworkGatewayConnection에 대한 예제 및 설명 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-380">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="1ef66-381">Remove-AzureRmVirtualNetworkGatewayIpConfig 및 Reset-AzureRmVirtualNetworkGateway에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-381">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="1ef66-382">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-382">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="1ef66-383">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-383">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="1ef66-384">Set-AzureRmVirtualNetworkGatewayConnection에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-384">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="1ef66-385">최신 코드 생성기를 사용하여 ApplicationSecurityGroup, RouteTable 및 Usage에 대한 cmdlet을 다시 생성함</span><span class="sxs-lookup"><span data-stu-id="1ef66-385">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="1ef66-386">Exitc 하지 않는 서브넷을 얻으려고 할 때의 Get-AzureRmVirtualNetworkSubnetConfig에 대한 오류 메시지를 설명</span><span class="sxs-lookup"><span data-stu-id="1ef66-386">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="1ef66-387">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="1ef66-387">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="1ef66-388">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-388">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="1ef66-389">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1ef66-389">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="1ef66-390">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-390">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="1ef66-391">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1ef66-391">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="1ef66-392">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-392">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="1ef66-393">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="1ef66-393">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="1ef66-394">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-394">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="1ef66-395">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1ef66-395">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="1ef66-396">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="1ef66-397">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="1ef66-397">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="1ef66-398">Get-AzureRmRecoveryServicesBackItem cmdlet에 정책 필터 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-398">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="1ef66-399">해당 명령은 지정된 정책 ID에 의해 보호되는 백업 항목의 목록을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-399">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="1ef66-400">Microsoft.Azure.Management.RecoveryServices.Backup을 버전 3.0.0-preview로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="1ef66-400">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="1ef66-401">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-401">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="1ef66-402">Restore-AzureRmRecoveryServicesBackupItem에 TargetResourceGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-402">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="1ef66-403">관리 디스크가 복원될 리소스 그룹</span><span class="sxs-lookup"><span data-stu-id="1ef66-403">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="1ef66-404">관리 디스크가 있는 VM의 백업에 적용 가능</span><span class="sxs-lookup"><span data-stu-id="1ef66-404">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="1ef66-405">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="1ef66-405">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="1ef66-406">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="1ef66-407">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1ef66-407">AzureRM.RedisCache</span></span>
* <span data-ttu-id="1ef66-408">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-408">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="1ef66-409">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="1ef66-409">AzureRM.Relay</span></span>
* <span data-ttu-id="1ef66-410">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-410">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="1ef66-411">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="1ef66-411">AzureRM.Resources</span></span>
* <span data-ttu-id="1ef66-412">구독 범위에서 템플릿 배포를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-412">Support template deployment at subscription scope.</span></span> <span data-ttu-id="1ef66-413">새 cmdlet 추가:</span><span class="sxs-lookup"><span data-stu-id="1ef66-413">Add new Cmdlets:</span></span>
    - <span data-ttu-id="1ef66-414">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="1ef66-414">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="1ef66-415">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="1ef66-415">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="1ef66-416">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="1ef66-416">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="1ef66-417">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="1ef66-417">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="1ef66-418">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="1ef66-418">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="1ef66-419">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="1ef66-419">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="1ef66-420">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="1ef66-420">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="1ef66-421">Set-AzureRmResource에 컨텍스트를 전달할 때 오류가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-421">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="1ef66-422">New-AzureRmResourceGroupDeployment의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-422">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="1ef66-423">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-423">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="1ef66-424">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="1ef66-424">AzureRM.Scheduler</span></span>
* <span data-ttu-id="1ef66-425">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-425">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="1ef66-426">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1ef66-426">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="1ef66-427">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="1ef66-428">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1ef66-428">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="1ef66-429">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="1ef66-430">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1ef66-430">AzureRM.Sql</span></span>
* <span data-ttu-id="1ef66-431">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="1ef66-432">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="1ef66-432">AzureRM.Storage</span></span>
* <span data-ttu-id="1ef66-433">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="1ef66-434">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="1ef66-434">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="1ef66-435">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="1ef66-436">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="1ef66-436">AzureRM.Tags</span></span>
* <span data-ttu-id="1ef66-437">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-437">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="1ef66-438">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="1ef66-438">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="1ef66-439">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-439">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="1ef66-440">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="1ef66-440">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="1ef66-441">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-441">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="1ef66-442">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="1ef66-442">AzureRM.Websites</span></span>
* <span data-ttu-id="1ef66-443">최신 버전의 Azure ClientRuntime으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-443">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="1ef66-444">6.6.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="1ef66-444">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="1ef66-445">일반</span><span class="sxs-lookup"><span data-stu-id="1ef66-445">General</span></span>
* <span data-ttu-id="1ef66-446">전체 매개 변수 형식 및 올바른 입/출력 형식을 포함하도록 모든 도움말 파일을 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-446">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="1ef66-447">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1ef66-447">AzureRM.Profile</span></span>
* <span data-ttu-id="1ef66-448">Common.Strategy 라이브러리가 리소스에 대한 현재 구성이 대상 리소스와 호환되는지 유효성을 검사할 수 있도록 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-448">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="1ef66-449">Common.Storage에 ps1xml 형식 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-449">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="1ef66-450">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1ef66-450">Azure.Storage</span></span>
* <span data-ttu-id="1ef66-451">DefaultProfile에서 저장소 컨텍스트를 가져오기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-451">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="1ef66-452">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-452">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="1ef66-453">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1ef66-453">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="1ef66-454">문제 https://github.com/Azure/azure-powershell/issues/6370 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-454">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="1ef66-455">PsApiManagementApi를 ApiContract로 좌표 이동하도록 Automapper 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-455">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="1ef66-456">문제 https://github.com/Azure/azure-powershell/issues/6515 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-456">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="1ef66-457">인코딩 형식을 사용하여 오버로드하지 않도록 File.Save 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-457">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="1ef66-458">문제 https://github.com/Azure/azure-powershell/issues/6560 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-458">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="1ef66-459">apiId에서 패턴 예외를 수정하는 4.0.3 Nuget 버전으로 업그레이드됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-459">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="1ef66-460">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1ef66-460">AzureRM.Compute</span></span>
* <span data-ttu-id="1ef66-461">PremiumLRS 저장소 계정 형식 이름 바꾸기로 인해 New-AzureRmVm에서 DiskFileParameterSet를 사용하여 vm 생성 시 실패하는 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-461">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="1ef66-462">Invoke-AzureRmVMRunCommand cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-462">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="1ef66-463">Get-AzureRmAvailabilitySet를 업데이트하여 구독에서 모든 가용성 집합 리스트를 사용하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-463">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="1ef66-464">(ResouceGroupName 매개 변수는 이제 선택적 요소입니다.)</span><span class="sxs-lookup"><span data-stu-id="1ef66-464">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="1ef66-465">vm 선별에 가속화된 네트워크를 사용하도록 'New-AzureRmVm'의 SimpleParameterSet를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-465">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="1ef66-466">New-AzureRmVmss 간단 매개 변수가 사용자 지정 LB가 이미 존재할 때 vms 생성에 실패하도록 설정하여 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-466">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="1ef66-467">New-AzureRmDisk에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-467">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="1ef66-468">'New-AzureRmVM'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-468">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="1ef66-469">Set-AzureRmVMOSDisk에 대한 설명 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-469">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="1ef66-470">Set-AzureRmVMBginfoExtension 맞춤법 및 접두사를 수정하도록 예제 1을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-470">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="1ef66-471">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="1ef66-471">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="1ef66-472">ADF.Net SDK 버전을 1.1.0으로 업데이트했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-472">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="1ef66-473">데이터 팩터리를 공유하는 자체 호스팅된 통합 런타임을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-473">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="1ef66-474">새 매개 변수 -SharedIntegrationRuntimeResourceId를 Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="1ef66-474">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="1ef66-475">새로운 선택적 매개 변수 -LinkedDataFactoryName을 Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="1ef66-475">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="1ef66-476">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1ef66-476">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="1ef66-477">DataPlane SDK(Microsoft.Azure.DataLake.Store) 버전을 1.1.9로 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-477">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="1ef66-478">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="1ef66-478">AzureRM.EventHub</span></span>
* <span data-ttu-id="1ef66-479">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-479">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="1ef66-480">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="1ef66-480">AzureRM.Insights</span></span>
* <span data-ttu-id="1ef66-481">도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-481">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="1ef66-482">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview를 사용</span><span class="sxs-lookup"><span data-stu-id="1ef66-482">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="1ef66-483">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1ef66-483">AzureRM.KeyVault</span></span>
* <span data-ttu-id="1ef66-484">Set-AzureRmKeyVaultAccessPolicy 내 파이핑 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-484">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="1ef66-485">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1ef66-485">AzureRM.Network</span></span>
* <span data-ttu-id="1ef66-486">LoadBalancerInboundNatPoolConfig cmdlet에 대한 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-486">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="1ef66-487">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="1ef66-487">AzureRM.Resources</span></span>
* <span data-ttu-id="1ef66-488">'Get-AzureRmResource'에 대한 태그 이름 및 값을 제공할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-488">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="1ef66-489">'Set-AzureRmResource'를 사용하여 파이핑 시나리오 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-489">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="1ef66-490">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1ef66-490">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="1ef66-491">cmdlet 제거에서 InputObject 및 ResourceId에 대한 파이핑이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-491">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="1ef66-492">몇 가지 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-492">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="1ef66-493">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1ef66-493">AzureRM.Sql</span></span>
* <span data-ttu-id="1ef66-494">다음 cmdlet 사용하여 서버 Advanced Threat Protection 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-494">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="1ef66-495">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="1ef66-495">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="1ef66-496">다음 cmdlet을 사용하여 취약성 평가 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-496">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="1ef66-497">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="1ef66-497">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="1ef66-498">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="1ef66-498">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="1ef66-499">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="1ef66-499">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="1ef66-500">Remove-AzureRmSqlServerFirewallRule의 예제 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-500">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="1ef66-501">Get-AzureSqlSyncGroupLog에서 미국이 아닌 문화권에서 날짜/시간을 올바르지 않게 다루는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-501">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="1ef66-502">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="1ef66-502">AzureRM.Storage</span></span>
* <span data-ttu-id="1ef66-503">Ps1XmlAttribute를 cmdlet 출력 형식 속성에 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-503">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="1ef66-504">StorageAccount cmdlet 출력을 테이블 뷰로 표시</span><span class="sxs-lookup"><span data-stu-id="1ef66-504">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="1ef66-505">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1ef66-505">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="1ef66-506">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1ef66-506">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="1ef66-507">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1ef66-507">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="1ef66-508">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="1ef66-508">AzureRM.Tags</span></span>
* <span data-ttu-id="1ef66-509">태그 cmdlet 도움말에서 잘못된 문을 제거합니다</span><span class="sxs-lookup"><span data-stu-id="1ef66-509">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="1ef66-510">6.5.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="1ef66-510">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="1ef66-511">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1ef66-511">AzureRM.Profile</span></span>
* <span data-ttu-id="1ef66-512">'Get-AzureRmContextAutosaveSetting'에 대한 도움말이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-512">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="1ef66-513">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1ef66-513">Azure.Storage</span></span>
* <span data-ttu-id="1ef66-514">쓰기 전용 SaS 토큰을 사용하는 Blob 또는 파일 업로드 지원</span><span class="sxs-lookup"><span data-stu-id="1ef66-514">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="1ef66-515">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1ef66-515">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="1ef66-516">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1ef66-516">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="1ef66-517">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1ef66-517">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="1ef66-518">필수 속성 ResourceGroupName을 AS에 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-518">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="1ef66-519">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="1ef66-519">AzureRM.Automation</span></span>
* <span data-ttu-id="1ef66-520">도움말을 업데이트하고 'New-AzureRMAutomationSchedule'에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-520">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="1ef66-521">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1ef66-521">AzureRM.Compute</span></span>
* <span data-ttu-id="1ef66-522">-Tag 매개 변수를 Update/New-AzureRmAvailabilitySet에 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-522">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="1ef66-523">‘Add-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-523">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="1ef66-524">‘Remove-AzureRmVmssExtension’에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-524">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="1ef66-525">‘Set-AzureRmVMAccessExtension’에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-525">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="1ef66-526">기본으로 SinglePlacementGroup을 false로 설정하고 단일 배치 그룹에 VMSS를 만들 수 있는 스위치 매개 변수 'SinglePlacementGroup'을 추가하도록 New-AzureRmVmss에 대한 SimpleParameterSet을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-526">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="1ef66-527">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="1ef66-527">AzureRM.EventHub</span></span>
* <span data-ttu-id="1ef66-528">PSEventHubDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="1ef66-528">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="1ef66-529">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1ef66-529">AzureRM.KeyVault</span></span>
* <span data-ttu-id="1ef66-530">Set-AzureRmKeyVaultAccessPolicy에 대한 오류 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-530">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="1ef66-531">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1ef66-531">AzureRM.LogicApp</span></span>
* <span data-ttu-id="1ef66-532">New-AzureRmLogicApp에서 "매개 변수 집합을 확인할 수 없습니다" 오류 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-532">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="1ef66-533">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1ef66-533">AzureRM.Network</span></span>
* <span data-ttu-id="1ef66-534">Set/Add-AzureRmVirtualNetworkPeering에 대한 여러 테넌트의 가상 네트워크에서 피어링을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="1ef66-534">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="1ef66-535">Application Gateway에 대한 아래 cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-535">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="1ef66-536">New-AzureRmApplicationGateway: EnableFIPS 플래그 및 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-536">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="1ef66-537">New-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-537">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="1ef66-538">Set-AzureRmApplicationGatewaySku: 새 sku Standard_v2 및 WAF_v2 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-538">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="1ef66-539">최신 생성기를 사용하여 RouteTable cmdlet을 재생성</span><span class="sxs-lookup"><span data-stu-id="1ef66-539">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="1ef66-540">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="1ef66-540">AzureRM.Relay</span></span>
* <span data-ttu-id="1ef66-541">markdown 파일을 업데이트하여 예제에서 매개 변수 이름 문제에 대해 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-541">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="1ef66-542">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="1ef66-542">AzureRM.Resources</span></span>
* <span data-ttu-id="1ef66-543">Roledefinition 및 Roleassignment cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-543">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="1ef66-544">페이징의 일부분으로 수행하는 추가 roledefinition 호출을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-544">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="1ef66-545">Get-AzureRmRoleAssignment cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-545">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="1ef66-546">-ExpandPrincipalGroups 명령 매개 변수 기능 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-546">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="1ef66-547">'Get-AzureRmResource'에서 '-ResourceType' 매개 변수가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-547">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="1ef66-548">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1ef66-548">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="1ef66-549">top 및 skip 매개 변수가 cmdlet 목록을 나열하도록 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-549">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="1ef66-550">표준을 프리미엄 네임스페이스 마이그레이션 cmdlet에 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-550">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="1ef66-551">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="1ef66-551">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="1ef66-552">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="1ef66-552">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="1ef66-553">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="1ef66-553">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="1ef66-554">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="1ef66-554">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="1ef66-555">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="1ef66-555">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="1ef66-556">PSServiceBusDRConfigurationAttributes 클래스에 읽기 전용 속성 'PendingReplicationOperationsCount'를 추가하여 복제가 진행되는 동안 보류 중인 복제 작업 수를 제공</span><span class="sxs-lookup"><span data-stu-id="1ef66-556">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="1ef66-557">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1ef66-557">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="1ef66-558">‘New-AzureRmServiceFabricCluster’에 대한 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-558">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="1ef66-559">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1ef66-559">AzureRM.Sql</span></span>
* <span data-ttu-id="1ef66-560">Management.Sql에 대한 새 cmdlet을 추가하여 고객이 TDE 인증서를 SQL Server 인스턴스 또는 Managed Instance에 추가할 수 있도록 허용</span><span class="sxs-lookup"><span data-stu-id="1ef66-560">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="1ef66-561">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="1ef66-561">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="1ef66-562">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="1ef66-562">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="1ef66-563">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="1ef66-563">AzureRM.Websites</span></span>
* <span data-ttu-id="1ef66-564">`Set-AzureRmWebApp -AssignIdentity` 및 `Set-AzureRmWebAppSlot -AssignIdentity`가 false로 설정되면 사이트 개체에서 Identity 속성이 제거됩니다. 미리보기 태그도 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-564">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="1ef66-565">`Get-AzureRmWebAppMetrics`, `Get-AzureRmAppServicePlanMetrics` 예제가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-565">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="1ef66-566">`Set-AzureRmWebApp -PhpVersion`이 유효한 php 버전으로 해제 지원</span><span class="sxs-lookup"><span data-stu-id="1ef66-566">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="1ef66-567">6.4.0 - 2018년 7월</span><span class="sxs-lookup"><span data-stu-id="1ef66-567">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="1ef66-568">일반</span><span class="sxs-lookup"><span data-stu-id="1ef66-568">General</span></span>
* <span data-ttu-id="1ef66-569">대부분의 모듈에 대한 도움말 파일에서 OutputType 서식 지정 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-569">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="1ef66-570">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1ef66-570">AzureRM.Profile</span></span>
* <span data-ttu-id="1ef66-571">기본 출력 형식에 추가된 Ps1Xml 특성</span><span class="sxs-lookup"><span data-stu-id="1ef66-571">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="1ef66-572">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1ef66-572">AzureRM.Compute</span></span>
* <span data-ttu-id="1ef66-573">VMSS에 대한 IP 태그 기능</span><span class="sxs-lookup"><span data-stu-id="1ef66-573">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="1ef66-574">'New-AzureRmVmssIpTagConfig' cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-574">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="1ef66-575">New-AzureRmVmssIpConfig에 IpTag 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-575">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="1ef66-576">VMSS에 대한 자동 OS 롤백 기능</span><span class="sxs-lookup"><span data-stu-id="1ef66-576">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="1ef66-577">New-AzureRmVmssConfig 및 Update-AzureRmVmss에 DisableAutoRollback 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-577">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="1ef66-578">Vmss에 대한 OS 업그레이드 기록 기능</span><span class="sxs-lookup"><span data-stu-id="1ef66-578">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="1ef66-579">Get-AzureRmVmss에 OSUpgradeHistory 스위치 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-579">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="1ef66-580">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="1ef66-580">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="1ef66-581">다음 명령을 통해 카탈로그 액세스 제어 목록에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-581">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="1ef66-582">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="1ef66-582">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="1ef66-583">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="1ef66-583">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="1ef66-584">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="1ef66-584">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="1ef66-585">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1ef66-585">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="1ef66-586">Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl에 대한 취소 지원 및 진행률 추적 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-586">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="1ef66-587">Export-AzureRmDataLakeStoreChildItemProperties에 대한 취소 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-587">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="1ef66-588">재귀 작업을 수행하는 cmdlet에 대한 디버그 메시지 플러시 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-588">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="1ef66-589">DataLake cmdlet의 테스트 위치 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-589">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="1ef66-590">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="1ef66-590">AzureRM.EventHub</span></span>
* <span data-ttu-id="1ef66-591">목록 작업 cmdlet Get-AzureRmEventHub 및 Get-AzureRmEventHubConsumerGroup에 선택적 MaxCount 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-591">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="1ef66-592">새 EventHub 만드는 동안 하나 이상의 매개 변수가 필요한 New-AzureRmEventHub cmdlet 문제를 해결.</span><span class="sxs-lookup"><span data-stu-id="1ef66-592">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="1ef66-593">기본 매개 변수 집합을 제공.</span><span class="sxs-lookup"><span data-stu-id="1ef66-593">Provided Default Parameter set.</span></span>
* <span data-ttu-id="1ef66-594">선택적 매개 변수 -KeyValue를 New-AzureRmEventHubKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-594">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="1ef66-595">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1ef66-595">AzureRM.KeyVault</span></span>
* <span data-ttu-id="1ef66-596">Get-AzureRmKeyVault -Tag 실행 시 모든 리소스가 리턴되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-596">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="1ef66-597">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1ef66-597">AzureRM.Network</span></span>
* <span data-ttu-id="1ef66-598">영역 중복 VirtualNetworkGateways에 대한 새 Sku를 노출합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-598">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="1ef66-599">기능에 대한 새 명령이 추가됨: ARM을 통한 ExpressRoute Partner APIs</span><span class="sxs-lookup"><span data-stu-id="1ef66-599">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="1ef66-600">Get- AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-600">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="1ef66-601">Set-AzureRmExpressRouteCrossConnection 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-601">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="1ef66-602">Add-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-602">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="1ef66-603">Get-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-603">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="1ef66-604">Remove-AzureRmExpressRouteCrossConnectionPeering 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-604">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="1ef66-605">Get-AzureRMExpressRouteCrossConnectionArpTable 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-605">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="1ef66-606">Get-AzureRMExpressRouteCrossConnectionRouteTable 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-606">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="1ef66-607">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-607">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="1ef66-608">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="1ef66-608">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="1ef66-609">Get-AzureRmRecoveryServicesBackupStatus cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-609">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="1ef66-610">이 cmdlet은 VM ID를 가져와서 VM이 구독에서 일부 자격 증명 모음으로 보호되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-610">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="1ef66-611">이러한 자격 증명 모음이 존재하는 경우 cmdlet은 자격 증명 모음 세부 정보를 출력 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-611">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="1ef66-612">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="1ef66-612">AzureRM.Resources</span></span>
* <span data-ttu-id="1ef66-613">Get-AzureRmPolicyAssignment cmdlet을 다음과 같이 업데이트함.</span><span class="sxs-lookup"><span data-stu-id="1ef66-613">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="1ef66-614">관리 그룹 수준에서 -Scope 값 리스팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-614">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="1ef66-615">관리 그룹 수준에서 -Scope 값을 사용하여 개별 할당값을 검색하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-615">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="1ef66-616">제어 매개 변수에 -Effective 및 -All 스위치 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-616">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="1ef66-617">Get/New/Remove/Set-AzureRmPolicyDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-617">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="1ef66-618">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-618">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="1ef66-619">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-619">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="1ef66-620">Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlet 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-620">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="1ef66-621">지정된 관리 그룹에 작업을 적용할 -ManagementGroupName 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-621">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="1ef66-622">지정된 구독에 작업을 적용할 -SubscriptionId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-622">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="1ef66-623">'New-AzureRmResourceGroupDeployment'에서 'TemplateParameterObject'를 사용하는 경우 매개 변수에 KeyVault 비밀 참조 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-623">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="1ef66-624">'New-AzureRmADAppCredential'에 대해 '-EndDate' 매개 변수가 무시되는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-624">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="1ef66-625">'Add-AzureRmADGroupMember'가 요청에 잘못된 URL을 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-625">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="1ef66-626">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1ef66-626">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="1ef66-627">선택적 매개 변수 -KeyValue를 New-AzureRmServiceBusKey cmdlet에 추가 하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-627">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="1ef66-628">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1ef66-628">AzureRM.Sql</span></span>
* <span data-ttu-id="1ef66-629">New-AzureRmSqlDatabaseRestorePoint 도움말에서 SQLDW에 대한 사용자 정의 복원 지점 명시</span><span class="sxs-lookup"><span data-stu-id="1ef66-629">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="1ef66-630">몇 가지 cmdlet에서-ComputeGeneration 매개 변수의 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-630">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="1ef66-631">6.3.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="1ef66-631">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="1ef66-632">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1ef66-632">AzureRM.Profile</span></span>
* <span data-ttu-id="1ef66-633">Enable-AzureRmContextAutoSave에 대한 오류 메시지 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-633">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="1ef66-634">이전 컨텍스트 없이 'Connect-AzureRmAccount' 실행 시 각 구독에 대한 컨텍스트 생성</span><span class="sxs-lookup"><span data-stu-id="1ef66-634">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="1ef66-635">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1ef66-635">Azure.Storage</span></span>
* <span data-ttu-id="1ef66-636">도움말 파일 내 -Permissions 매개 변수에 대한 추가 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-636">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="1ef66-637">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1ef66-637">AzureRM.Compute</span></span>
* <span data-ttu-id="1ef66-638">'Get-AzureRmVmDiskEncryptionStatus'가 데이터 디스크가 없는 VM에 대해 관찰된 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-638">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="1ef66-639">Compute 클라이언트 라이브러리 버전을 업데이트하여 다음 cmdlet 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-639">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="1ef66-640">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="1ef66-640">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="1ef66-641">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="1ef66-641">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="1ef66-642">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="1ef66-642">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="1ef66-643">다음 cmdlet이 '작업 ID' 및 '작업 상태'를 올바르게 표시하도록 수정:</span><span class="sxs-lookup"><span data-stu-id="1ef66-643">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="1ef66-644">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="1ef66-644">Start-AzureRmVM</span></span>
    - <span data-ttu-id="1ef66-645">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="1ef66-645">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="1ef66-646">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="1ef66-646">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="1ef66-647">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="1ef66-647">Set-AzureRmVM</span></span>
    - <span data-ttu-id="1ef66-648">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="1ef66-648">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="1ef66-649">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="1ef66-649">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="1ef66-650">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="1ef66-650">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="1ef66-651">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="1ef66-651">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="1ef66-652">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="1ef66-652">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="1ef66-653">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="1ef66-653">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="1ef66-654">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="1ef66-654">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="1ef66-655">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="1ef66-655">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="1ef66-656">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="1ef66-656">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="1ef66-657">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="1ef66-657">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="1ef66-658">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="1ef66-658">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="1ef66-659">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="1ef66-659">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="1ef66-660">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="1ef66-660">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="1ef66-661">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="1ef66-661">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="1ef66-662">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="1ef66-662">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="1ef66-663">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1ef66-663">AzureRM.EventGrid</span></span>
* <span data-ttu-id="1ef66-664">Update-AzureRmEventGridSubscription cmdlet의 SubjectBeginsWith/SubjectEndsWith에 대한 ValidateNotNullOrEmpty 유효성 검사 조건을 제거하여 필요에 따라 이러한 매개 변수를 빈 문자열로 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-664">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="1ef66-665">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1ef66-665">AzureRM.KeyVault</span></span>
* <span data-ttu-id="1ef66-666">Get-AzureRmKeyVault -Tag 실행 시 태그가 리턴되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-666">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="1ef66-667">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1ef66-667">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="1ef66-668">Policy Insights cmdlet의 공개 릴리스</span><span class="sxs-lookup"><span data-stu-id="1ef66-668">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="1ef66-669">API 버전 2018-04-04 사용</span><span class="sxs-lookup"><span data-stu-id="1ef66-669">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="1ef66-670">PolicyDefinitionReferenceId를 Get-AzureRmPolicyStateSummary의 결과 집합에 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-670">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="1ef66-671">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="1ef66-671">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="1ef66-672">-Vault 매개 변수를 RecoveryServices.Backup cmdlet에 추가.</span><span class="sxs-lookup"><span data-stu-id="1ef66-672">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="1ef66-673">전달되는 경우 이는 Set-AzureRmRecoveryServicesContext cmdlet을 재정의함.</span><span class="sxs-lookup"><span data-stu-id="1ef66-673">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="1ef66-674">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1ef66-674">AzureRM.Sql</span></span>
* <span data-ttu-id="1ef66-675">Get-AzureRmSqlDatabaseExpanded에 대한 도움말 파일의 예가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-675">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="1ef66-676">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="1ef66-676">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="1ef66-677">Add-AzureRmTrafficManagerEndpointConfig에대한 도움말 파일이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-677">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="1ef66-678">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="1ef66-678">AzureRM.Websites</span></span>
* <span data-ttu-id="1ef66-679">-AssignIdentity를 사용할 때 AppSetting을 덮어쓰지 않도록 'Set-AzureRmWebApp'이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-679">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="1ef66-680">'New-AzureRmWebAppSlot'이 AppServicePlan을 옵션 매개변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-680">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="1ef66-681">6.2.1 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="1ef66-681">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="1ef66-682">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1ef66-682">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="1ef66-683">PSWorkspace 모델이 Network 형식을 매개 변수로 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-683">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="1ef66-684">6.2.0 - 2018년 6월</span><span class="sxs-lookup"><span data-stu-id="1ef66-684">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="1ef66-685">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1ef66-685">AzureRM.Profile</span></span>
* <span data-ttu-id="1ef66-686">Newtonsoft.Json의 버전 10.0.3이 모듈 가져오기에 로드되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-686">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="1ef66-687">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1ef66-687">AzureRM.Compute</span></span>
* <span data-ttu-id="1ef66-688">VMSS VM 업데이트 기능</span><span class="sxs-lookup"><span data-stu-id="1ef66-688">VMSS VM Update feature</span></span>
    - <span data-ttu-id="1ef66-689">'Update-AzureRmVmssVM' 및 'New-AzureRmVMDataDisk' cmdlets 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-689">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="1ef66-690">데이터 디스크를 Vmss VM에 추가할 수 있도록 지원하기 위해 VirtualMachineScaleSetVM 매개변수를 'Add-AzureRmVMDataDisk' cmdlet에 추가하였습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-690">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="1ef66-691">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="1ef66-691">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="1ef66-692">ADF .Net SDK 버전이 다음 변경 내용이 포함된 0.8.0-preview로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-692">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="1ef66-693">팩터리 리포지토리 작업 구성 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-693">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="1ef66-694">QuickBooks LinkedService가 ConsumerKey 및 consumerSecret 속성을 노출하도록 업데이트됨 </span><span class="sxs-lookup"><span data-stu-id="1ef66-694">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="1ef66-695">여러 모델 유형을 SecretBase에서 개체로 업데이트함</span><span class="sxs-lookup"><span data-stu-id="1ef66-695">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="1ef66-696">Blob 이벤트 트리거 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-696">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="1ef66-697">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1ef66-697">AzureRM.KeyVault</span></span>
* <span data-ttu-id="1ef66-698">예제 출력으로 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-698">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="1ef66-699">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1ef66-699">AzureRM.Network</span></span>
* <span data-ttu-id="1ef66-700">Network Watcher cmdlet에서 트래픽 분석 매개 변수를 사용가능하도록 설정</span><span class="sxs-lookup"><span data-stu-id="1ef66-700">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="1ef66-701">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="1ef66-701">AzureRM.Resources</span></span>
* <span data-ttu-id="1ef66-702">'Get AzureRmResource'에서 반환된 'PSResource' 개체의 'Properties' 속성의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-702">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="1ef66-703">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="1ef66-703">AzureRM.Scheduler</span></span>
* <span data-ttu-id="1ef66-704">ServiceBusQueueJob 업데이트가 새 인증 값을 설정하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef66-704">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="1ef66-705">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1ef66-705">AzureRM.Sql</span></span>
* <span data-ttu-id="1ef66-706">옵션 LicenseType 매개 변수를 사용하여 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ef66-706">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="1ef66-707">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="1ef66-707">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="1ef66-708">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="1ef66-708">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="1ef66-709">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="1ef66-709">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="1ef66-710">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="1ef66-710">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="1ef66-711">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="1ef66-711">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="1ef66-712">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="1ef66-712">AzureRM.Websites</span></span>
* <span data-ttu-id="1ef66-713">'New-AzureRMWebApp'이 전략 라이브러리의 공통 알고리즘을 사용하도록 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-713">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="1ef66-714">6.1.0 - 2018년 5월</span><span class="sxs-lookup"><span data-stu-id="1ef66-714">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="1ef66-715">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1ef66-715">AzureRM.Profile</span></span>
* <span data-ttu-id="1ef66-716">'Clear-AzureRmContext'를 실행하면 이전 기본 컨텍스트의 이름으로 빈 컨텍스트가 유지되어 사용자가 이전 이름으로 새 컨텍스트를 만들지 못하게 되는 문제를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-716">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="1ef66-717">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1ef66-717">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="1ef66-718">AS에서 게이트웨이가 작업을 연결하거나 연결 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-718">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="1ef66-719">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1ef66-719">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="1ef66-720">ApiVersions, ApiReleases 및 ApiRevisions에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-720">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="1ef66-721">ServiceFabric 백 엔드에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-721">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="1ef66-722">Application Insights 로거에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-722">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="1ef66-723">'기본' SKU를 API Management 서비스의 유효한 SKU로 인식하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-723">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="1ef66-724">개인 CA가 발급한 인증서를 루트 또는 CA로 설치하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-724">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="1ef66-725">KeyVault 및 다중 프록시 호스트 이름을 통한 사용자 정의 SSL 인증서를 수락하는 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-725">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="1ef66-726">MSI ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1ef66-726">Added support for MSI identity</span></span>
* <span data-ttu-id="1ef66-727">URL을 통한 정책을 수락하는 지원 추가됨 참고: 다음 cmdlet은 이후 릴리스에서 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-727">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="1ef66-728">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="1ef66-728">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="1ef66-729">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ef66-729">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="1ef66-730">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="1ef66-730">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="1ef66-731">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="1ef66-731">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="1ef66-732">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="1ef66-732">AzureRM.Batch</span></span>
* <span data-ttu-id="1ef66-733">새 cmdlet Get AzureBatchPoolNodeCounts 릴리스</span><span class="sxs-lookup"><span data-stu-id="1ef66-733">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="1ef66-734">새 cmdlet Start-AzureBatchComputeNodeServiceLogUpload 릴리스</span><span class="sxs-lookup"><span data-stu-id="1ef66-734">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="1ef66-735">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="1ef66-735">AzureRM.Consumption</span></span>
* <span data-ttu-id="1ef66-736">Expand, ResourceGroup, InstanceName, InstanceId, Tags, Top on Cmdlet Get-AzureRmConsumptionUsageDetail 등 새 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1ef66-736">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="1ef66-737">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1ef66-737">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="1ef66-738">Export-AzureRmDataLakeStoreChildItemProperties에 대한 예제 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-738">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="1ef66-739">Set-AzureRmDataLakeStoreItemAclEntry에서 재귀 사례에 대한 null 매개 변수 예외 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-739">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="1ef66-740">Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry에 대한 도움말 파일 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-740">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="1ef66-741">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1ef66-741">AzureRM.Network</span></span>
* <span data-ttu-id="1ef66-742">18.0.0-preview에서 19.0.0-preview로 네트워크 SDK 버전 업그레이드</span><span class="sxs-lookup"><span data-stu-id="1ef66-742">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="1ef66-743">프로토콜 구성을 만들기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="1ef66-743">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="1ef66-744">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ef66-744">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="1ef66-745">기존 Express 경로 회로에 새 회로 연결을 추가하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="1ef66-745">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="1ef66-746">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-746">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="1ef66-747">기존 Express 경로 회로에서 회로 연결을 제거하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="1ef66-747">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="1ef66-748">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-748">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="1ef66-749">회로 연결을 검색하기 위해 추가된 cmdlet</span><span class="sxs-lookup"><span data-stu-id="1ef66-749">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="1ef66-750">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="1ef66-750">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="1ef66-751">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1ef66-751">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="1ef66-752">생성된 인증서로 고정 서버 인증 사용(문제 # 5998)</span><span class="sxs-lookup"><span data-stu-id="1ef66-752">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="1ef66-753">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1ef66-753">AzureRM.Sql</span></span>
* <span data-ttu-id="1ef66-754">AuditActions 또는 AuditActionGroups를 제거할 수 있도록 업데이트된 감사 cmdlet</span><span class="sxs-lookup"><span data-stu-id="1ef66-754">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="1ef66-755">'Azure 복구 서비스 자격 증명 모음을 사용하여 장기 보존 정책을 구성하면 정책이 더 이상 지원되지 않습니다. 새로운 유연 보유 정책으로 요청을 제출하십시오.'라는 메시지와 함께 명령이 실패하는 새로운 유연 보유 정책을 설정할 때</span><span class="sxs-lookup"><span data-stu-id="1ef66-755">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="1ef66-756">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy의 문제 수정</span><span class="sxs-lookup"><span data-stu-id="1ef66-756">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="1ef66-757">Azure SQL Database/ElasticPool Creation/Update 관련 cmdlet을 모두 업데이트하여 규모 및 계층 관련 속성에 대한 SKU 속성을 지원하는 새 데이터베이스 API를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-757">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="1ef66-758">업데이트된 cmdlet는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-758">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="1ef66-759">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="1ef66-759">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="1ef66-760">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="1ef66-760">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="1ef66-761">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="1ef66-761">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="1ef66-762">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="1ef66-762">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="1ef66-763">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="1ef66-763">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="1ef66-764">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="1ef66-764">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="1ef66-765">-Name 매개 변수를 사용할 때 -ResourceGroupName 매개 변수가 필요하도록 'Get-AzureRmTrafficManagerProfile'에 대한 매개 변수를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef66-765">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
