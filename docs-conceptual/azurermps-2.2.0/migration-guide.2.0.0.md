# <a name="table-of-contents"></a><span data-ttu-id="ad385-101">목차</span><span class="sxs-lookup"><span data-stu-id="ad385-101">Table of Contents</span></span>
1. [<span data-ttu-id="ad385-102">Force 매개 변수 제거</span><span class="sxs-lookup"><span data-stu-id="ad385-102">Removal of Force parameters</span></span>](#removal-of-force-parameters)
2. [<span data-ttu-id="ad385-103">Tag 매개 변수 변경</span><span class="sxs-lookup"><span data-stu-id="ad385-103">Change of Tag parameters</span></span>](#change-of-tag-parameters)
3. [<span data-ttu-id="ad385-104">Storage cmdlet의 주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="ad385-104">Breaking changes to Storage cmdlets</span></span>](#breaking-changes-to-storage-cmdlets)
4. [<span data-ttu-id="ad385-105">AD cmdlet의 주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="ad385-105">Breaking changes to AD cmdlets</span></span>](#breaking-changes-to-ad-cmdlets)

## <a name="removal-of-force-parameters"></a><span data-ttu-id="ad385-106">Force 매개 변수 제거</span><span class="sxs-lookup"><span data-stu-id="ad385-106">Removal of Force parameters</span></span>

<span data-ttu-id="ad385-107">이 릴리스에서는 cmdlet에서 사용되지 않는 `Force` 매개 변수를 모두 제거했으며 향후 릴리스에서 매개 변수가 제거될 것이라는 해당 경고를 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-107">This release, we removed all Obsolete `Force` parameters from cmdlets and the corresponding warnings that the parameter would be removed in a future release.</span></span>

<span data-ttu-id="ad385-108">다음 cmdlet은 이러한 변경에 의해 영향을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-108">The following cmdlets are affected by this change:</span></span>

<span data-ttu-id="ad385-109">**ApiManagement**</span><span class="sxs-lookup"><span data-stu-id="ad385-109">**ApiManagement**</span></span>
- <span data-ttu-id="ad385-110">Remove-AzureRmApiManagement</span><span class="sxs-lookup"><span data-stu-id="ad385-110">Remove-AzureRmApiManagement</span></span>
- <span data-ttu-id="ad385-111">Remove-AzureRmApiManagementApi</span><span class="sxs-lookup"><span data-stu-id="ad385-111">Remove-AzureRmApiManagementApi</span></span>
- <span data-ttu-id="ad385-112">Remove-AzureRmApiManagementGroup</span><span class="sxs-lookup"><span data-stu-id="ad385-112">Remove-AzureRmApiManagementGroup</span></span>
- <span data-ttu-id="ad385-113">Remove-AzureRmApiManagementLogger</span><span class="sxs-lookup"><span data-stu-id="ad385-113">Remove-AzureRmApiManagementLogger</span></span>
- <span data-ttu-id="ad385-114">Remove-AzureRmApiManagementOpenIdConnectProvider</span><span class="sxs-lookup"><span data-stu-id="ad385-114">Remove-AzureRmApiManagementOpenIdConnectProvider</span></span>
- <span data-ttu-id="ad385-115">Remove-AzureRmApiManagementOperation</span><span class="sxs-lookup"><span data-stu-id="ad385-115">Remove-AzureRmApiManagementOperation</span></span>
- <span data-ttu-id="ad385-116">Remove-AzureRmApiManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="ad385-116">Remove-AzureRmApiManagementPolicy</span></span>
- <span data-ttu-id="ad385-117">Remove-AzureRmApiManagementProduct</span><span class="sxs-lookup"><span data-stu-id="ad385-117">Remove-AzureRmApiManagementProduct</span></span>
- <span data-ttu-id="ad385-118">Remove-AzureRmApiManagementProperty</span><span class="sxs-lookup"><span data-stu-id="ad385-118">Remove-AzureRmApiManagementProperty</span></span>
- <span data-ttu-id="ad385-119">Remove-AzureRmApiManagementSubscription</span><span class="sxs-lookup"><span data-stu-id="ad385-119">Remove-AzureRmApiManagementSubscription</span></span>
- <span data-ttu-id="ad385-120">Remove-AzureRmApiManagementUser</span><span class="sxs-lookup"><span data-stu-id="ad385-120">Remove-AzureRmApiManagementUser</span></span>

<span data-ttu-id="ad385-121">**Automation**</span><span class="sxs-lookup"><span data-stu-id="ad385-121">**Automation**</span></span>
- <span data-ttu-id="ad385-122">Remove-AzureRmAutomationCertificate</span><span class="sxs-lookup"><span data-stu-id="ad385-122">Remove-AzureRmAutomationCertificate</span></span>
- <span data-ttu-id="ad385-123">Remove-AzureRmAutomationCredential</span><span class="sxs-lookup"><span data-stu-id="ad385-123">Remove-AzureRmAutomationCredential</span></span>
- <span data-ttu-id="ad385-124">Remove-AzureRmAutomationVariable</span><span class="sxs-lookup"><span data-stu-id="ad385-124">Remove-AzureRmAutomationVariable</span></span>
- <span data-ttu-id="ad385-125">Remove-AzureRmAutomationWebhook</span><span class="sxs-lookup"><span data-stu-id="ad385-125">Remove-AzureRmAutomationWebhook</span></span>

<span data-ttu-id="ad385-126">**Batch**</span><span class="sxs-lookup"><span data-stu-id="ad385-126">**Batch**</span></span>
- <span data-ttu-id="ad385-127">Remove-AzureBatchCertificate</span><span class="sxs-lookup"><span data-stu-id="ad385-127">Remove-AzureBatchCertificate</span></span>
- <span data-ttu-id="ad385-128">Remove-AzureBatchComputeNode</span><span class="sxs-lookup"><span data-stu-id="ad385-128">Remove-AzureBatchComputeNode</span></span>
- <span data-ttu-id="ad385-129">Remove-AzureBatchComputeNodeUser</span><span class="sxs-lookup"><span data-stu-id="ad385-129">Remove-AzureBatchComputeNodeUser</span></span>

<span data-ttu-id="ad385-130">**DataFactories**</span><span class="sxs-lookup"><span data-stu-id="ad385-130">**DataFactories**</span></span>
- <span data-ttu-id="ad385-131">Resume-AzureRmDataFactoryPipeline</span><span class="sxs-lookup"><span data-stu-id="ad385-131">Resume-AzureRmDataFactoryPipeline</span></span>
- <span data-ttu-id="ad385-132">Set-AzureRmDataFactoryPipelineActivePeriod</span><span class="sxs-lookup"><span data-stu-id="ad385-132">Set-AzureRmDataFactoryPipelineActivePeriod</span></span>
- <span data-ttu-id="ad385-133">Suspend-AzureRmDataFactoryPipeline</span><span class="sxs-lookup"><span data-stu-id="ad385-133">Suspend-AzureRmDataFactoryPipeline</span></span>

<span data-ttu-id="ad385-134">**DataLakeStore**</span><span class="sxs-lookup"><span data-stu-id="ad385-134">**DataLakeStore**</span></span>
- <span data-ttu-id="ad385-135">Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="ad385-135">Remove-AzureRmDataLakeStoreItemAclEntry</span></span>
- <span data-ttu-id="ad385-136">Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="ad385-136">Set-AzureRmDataLakeStoreItemAcl</span></span>
- <span data-ttu-id="ad385-137">Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="ad385-137">Set-AzureRmDataLakeStoreItemAclEntry</span></span>
- <span data-ttu-id="ad385-138">Set-AzureRmDataLakeStoreItemOwner</span><span class="sxs-lookup"><span data-stu-id="ad385-138">Set-AzureRmDataLakeStoreItemOwner</span></span>

<span data-ttu-id="ad385-139">**OperationalInsights**</span><span class="sxs-lookup"><span data-stu-id="ad385-139">**OperationalInsights**</span></span>
- <span data-ttu-id="ad385-140">Remove-AzureRmOperationalInsightsSavedSearch</span><span class="sxs-lookup"><span data-stu-id="ad385-140">Remove-AzureRmOperationalInsightsSavedSearch</span></span>

<span data-ttu-id="ad385-141">**프로필**</span><span class="sxs-lookup"><span data-stu-id="ad385-141">**Profile**</span></span>
- <span data-ttu-id="ad385-142">Remove-AzureRmEnvironment</span><span class="sxs-lookup"><span data-stu-id="ad385-142">Remove-AzureRmEnvironment</span></span>

<span data-ttu-id="ad385-143">**RedisCache**</span><span class="sxs-lookup"><span data-stu-id="ad385-143">**RedisCache**</span></span>
- <span data-ttu-id="ad385-144">Remove-AzureRmRedisCacheDiagnostics</span><span class="sxs-lookup"><span data-stu-id="ad385-144">Remove-AzureRmRedisCacheDiagnostics</span></span>

<span data-ttu-id="ad385-145">**리소스**</span><span class="sxs-lookup"><span data-stu-id="ad385-145">**Resources**</span></span>
- <span data-ttu-id="ad385-146">Register-AzureRmProviderFeature</span><span class="sxs-lookup"><span data-stu-id="ad385-146">Register-AzureRmProviderFeature</span></span>
- <span data-ttu-id="ad385-147">Register-AzureRmResourceProvider</span><span class="sxs-lookup"><span data-stu-id="ad385-147">Register-AzureRmResourceProvider</span></span>
- <span data-ttu-id="ad385-148">Remove-AzureRmADServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="ad385-148">Remove-AzureRmADServicePrincipal</span></span>
- <span data-ttu-id="ad385-149">Remove-AzureRmPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ad385-149">Remove-AzureRmPolicyAssignment</span></span>
- <span data-ttu-id="ad385-150">Remove-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="ad385-150">Remove-AzureRmResourceGroupDeployment</span></span>
- <span data-ttu-id="ad385-151">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ad385-151">Remove-AzureRmRoleAssignment</span></span>
- <span data-ttu-id="ad385-152">Stop-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="ad385-152">Stop-AzureRmResourceGroupDeployment</span></span>
- <span data-ttu-id="ad385-153">Unregister-AzureRmResourceProvider</span><span class="sxs-lookup"><span data-stu-id="ad385-153">Unregister-AzureRmResourceProvider</span></span>

<span data-ttu-id="ad385-154">**Storage**</span><span class="sxs-lookup"><span data-stu-id="ad385-154">**Storage**</span></span>
- <span data-ttu-id="ad385-155">Remove-AzureStorageContainerStoredAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ad385-155">Remove-AzureStorageContainerStoredAccessPolicy</span></span>
- <span data-ttu-id="ad385-156">Remove-AzureStorageQueueStoredAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ad385-156">Remove-AzureStorageQueueStoredAccessPolicy</span></span>
- <span data-ttu-id="ad385-157">Remove-AzureStorageShareStoredAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ad385-157">Remove-AzureStorageShareStoredAccessPolicy</span></span>
- <span data-ttu-id="ad385-158">Remove-AzureStorageTableStoredAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ad385-158">Remove-AzureStorageTableStoredAccessPolicy</span></span>

<span data-ttu-id="ad385-159">**StreamAnalytics**</span><span class="sxs-lookup"><span data-stu-id="ad385-159">**StreamAnalytics**</span></span>
- <span data-ttu-id="ad385-160">Remove-AzureRmStreamAnalyticsFunction</span><span class="sxs-lookup"><span data-stu-id="ad385-160">Remove-AzureRmStreamAnalyticsFunction</span></span>
- <span data-ttu-id="ad385-161">Remove-AzureRmStreamAnalyticsInput</span><span class="sxs-lookup"><span data-stu-id="ad385-161">Remove-AzureRmStreamAnalyticsInput</span></span>
- <span data-ttu-id="ad385-162">Remove-AzureRmStreamAnalyticsJob</span><span class="sxs-lookup"><span data-stu-id="ad385-162">Remove-AzureRmStreamAnalyticsJob</span></span>
- <span data-ttu-id="ad385-163">Remove-AzureRmStreamAnalyticsOutput</span><span class="sxs-lookup"><span data-stu-id="ad385-163">Remove-AzureRmStreamAnalyticsOutput</span></span>

<span data-ttu-id="ad385-164">**Tag**</span><span class="sxs-lookup"><span data-stu-id="ad385-164">**Tag**</span></span>
- <span data-ttu-id="ad385-165">Remove-AzureRmTag</span><span class="sxs-lookup"><span data-stu-id="ad385-165">Remove-AzureRmTag</span></span>

<br>

<span data-ttu-id="ad385-166">위의 cmdlet 중 하나를 사용하는 스크립트가 있는 경우 `Force` 매개 변수를 제거하기만 하면 주요 변경 내용이 해결될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-166">If you have a script that uses any of the above cmdlets, the breaking change can be fixed by simply removing the `Force` parameter.</span></span>

```powershell
# Old
New-AzureRmResourceGroup -Name $resourceGroupName -Location $location -Force

# New
New-AzureRmResourceGroup -Name $resourceGroupName -Location $location
```

<br>

## <a name="change-of-tag-parameters"></a><span data-ttu-id="ad385-167">Tag 매개 변수 변경</span><span class="sxs-lookup"><span data-stu-id="ad385-167">Change of Tag parameters</span></span>

<span data-ttu-id="ad385-168">이 릴리스에서는 `Tags` 매개 변수 이름이 `Tag`로, 형식은 `Hashtable[]`에서 `Hashtable`로 변경되어, 키-값 쌍의 형식이 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-168">This release, the `Tags` parameter name was changed to `Tag`, and the type was changed from `Hashtable[]` to `Hashtable`, changing the format of the key-value pairings.</span></span>

<span data-ttu-id="ad385-169">이전에는 `Hashtable[]`의 각 항목이 단일 키-값 쌍을 나타냈습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-169">Previously, each entry in the `Hashtable[]` represented a single key-value pairing:</span></span>

```powershell
$tags = @{ Name = "test1"; Value = "testval1" }, @{ Name = "test2", Value = "testval2" }
$tags[0].Name  # Key for the first entry, "test1"
$tags[0].Value # Value for the first entry, "testval1"
$tags[1].Name  # Key for the second entry, "test2"
$tags[1].Value # Value for the second entry, "testval2"
```

<span data-ttu-id="ad385-170">이제 `Name` 및 `Value`가 더 이상 필요하지 않으며 `Hashtable`에서 `Key = "Value"`를 할당하여 키-값 쌍을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-170">Now, `Name` and `Value` are no longer necessary, allowing for key-value pairings to be created by assigning `Key = "Value"` in the `Hashtable`:</span></span>

```powershell
$tag = @{ test1 = "testval1"; test2 = "testval2" }
$tag["test1"] # Gets the value associated with the key "test1"
$tag["test2"] # Gets the value associated with the key "test2"
```

<span data-ttu-id="ad385-171">다음 cmdlet은 이러한 변경에 의해 영향을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-171">The following cmdlets are affected by this change:</span></span>

<span data-ttu-id="ad385-172">**Batch**</span><span class="sxs-lookup"><span data-stu-id="ad385-172">**Batch**</span></span>
- <span data-ttu-id="ad385-173">Get-AzureRmBatchAccount</span><span class="sxs-lookup"><span data-stu-id="ad385-173">Get-AzureRmBatchAccount</span></span>
- <span data-ttu-id="ad385-174">New-AzureRmBatchAccount</span><span class="sxs-lookup"><span data-stu-id="ad385-174">New-AzureRmBatchAccount</span></span>
- <span data-ttu-id="ad385-175">Set-AzureRmBatchAccount</span><span class="sxs-lookup"><span data-stu-id="ad385-175">Set-AzureRmBatchAccount</span></span>

<span data-ttu-id="ad385-176">**Compute**</span><span class="sxs-lookup"><span data-stu-id="ad385-176">**Compute**</span></span>
- <span data-ttu-id="ad385-177">New-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="ad385-177">New-AzureRmVM</span></span>
- <span data-ttu-id="ad385-178">Update-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="ad385-178">Update-AzureRmVM</span></span>

<span data-ttu-id="ad385-179">**DataLakeAnalytics**</span><span class="sxs-lookup"><span data-stu-id="ad385-179">**DataLakeAnalytics**</span></span>
- <span data-ttu-id="ad385-180">New-AzureRmDataLakeAnalyticsAccount</span><span class="sxs-lookup"><span data-stu-id="ad385-180">New-AzureRmDataLakeAnalyticsAccount</span></span>
- <span data-ttu-id="ad385-181">Set-AzureRmDataLakeAnalyticsAccount</span><span class="sxs-lookup"><span data-stu-id="ad385-181">Set-AzureRmDataLakeAnalyticsAccount</span></span>

<span data-ttu-id="ad385-182">**DataLakeStore**</span><span class="sxs-lookup"><span data-stu-id="ad385-182">**DataLakeStore**</span></span>
- <span data-ttu-id="ad385-183">New-AzureRmDataLakeStoreAccount</span><span class="sxs-lookup"><span data-stu-id="ad385-183">New-AzureRmDataLakeStoreAccount</span></span>
- <span data-ttu-id="ad385-184">Set-AzureRmDataLakeStoreAccount</span><span class="sxs-lookup"><span data-stu-id="ad385-184">Set-AzureRmDataLakeStoreAccount</span></span>

<span data-ttu-id="ad385-185">**Dns**</span><span class="sxs-lookup"><span data-stu-id="ad385-185">**Dns**</span></span>
- <span data-ttu-id="ad385-186">New-AzureRmDnsZone</span><span class="sxs-lookup"><span data-stu-id="ad385-186">New-AzureRmDnsZone</span></span>
- <span data-ttu-id="ad385-187">Set-AzureRmDnsZone</span><span class="sxs-lookup"><span data-stu-id="ad385-187">Set-AzureRmDnsZone</span></span>

<span data-ttu-id="ad385-188">**KeyVault**</span><span class="sxs-lookup"><span data-stu-id="ad385-188">**KeyVault**</span></span>
- <span data-ttu-id="ad385-189">Get-AzureRmKeyVault</span><span class="sxs-lookup"><span data-stu-id="ad385-189">Get-AzureRmKeyVault</span></span>
- <span data-ttu-id="ad385-190">New-AzureRmKeyVault</span><span class="sxs-lookup"><span data-stu-id="ad385-190">New-AzureRmKeyVault</span></span>

<span data-ttu-id="ad385-191">**네트워크**</span><span class="sxs-lookup"><span data-stu-id="ad385-191">**Network**</span></span>
- <span data-ttu-id="ad385-192">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="ad385-192">New-AzureRmApplicationGateway</span></span>
- <span data-ttu-id="ad385-193">New-AzureRmExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="ad385-193">New-AzureRmExpressRouteCircuit</span></span>
- <span data-ttu-id="ad385-194">New-AzureRmLoadBalancer</span><span class="sxs-lookup"><span data-stu-id="ad385-194">New-AzureRmLoadBalancer</span></span>
- <span data-ttu-id="ad385-195">New-AzureRmLocalNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="ad385-195">New-AzureRmLocalNetworkGateway</span></span>
- <span data-ttu-id="ad385-196">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="ad385-196">New-AzureRmNetworkInterface</span></span>
- <span data-ttu-id="ad385-197">New-AzureRmNetworkSecurityGroup</span><span class="sxs-lookup"><span data-stu-id="ad385-197">New-AzureRmNetworkSecurityGroup</span></span>
- <span data-ttu-id="ad385-198">New-AzureRmPublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="ad385-198">New-AzureRmPublicIpAddress</span></span>
- <span data-ttu-id="ad385-199">New-AzureRmRouteTable</span><span class="sxs-lookup"><span data-stu-id="ad385-199">New-AzureRmRouteTable</span></span>
- <span data-ttu-id="ad385-200">New-AzureRmVirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="ad385-200">New-AzureRmVirtualNetwork</span></span>
- <span data-ttu-id="ad385-201">New-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="ad385-201">New-AzureRmVirtualNetworkGateway</span></span>
- <span data-ttu-id="ad385-202">New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="ad385-202">New-AzureRmVirtualNetworkGatewayConnection</span></span>
- <span data-ttu-id="ad385-203">New-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="ad385-203">New-AzureRmVirtualNetworkPeering</span></span>

<span data-ttu-id="ad385-204">**리소스**</span><span class="sxs-lookup"><span data-stu-id="ad385-204">**Resources**</span></span>
- <span data-ttu-id="ad385-205">Find-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="ad385-205">Find-AzureRmResource</span></span>
- <span data-ttu-id="ad385-206">Find-AzureRmResourceGroup</span><span class="sxs-lookup"><span data-stu-id="ad385-206">Find-AzureRmResourceGroup</span></span>
- <span data-ttu-id="ad385-207">New-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="ad385-207">New-AzureRmResource</span></span>
- <span data-ttu-id="ad385-208">New-AzureRmResourceGroup</span><span class="sxs-lookup"><span data-stu-id="ad385-208">New-AzureRmResourceGroup</span></span>
- <span data-ttu-id="ad385-209">Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="ad385-209">Set-AzureRmResource</span></span>
- <span data-ttu-id="ad385-210">Set-AzureRmResourceGroup</span><span class="sxs-lookup"><span data-stu-id="ad385-210">Set-AzureRmResourceGroup</span></span>

<span data-ttu-id="ad385-211">**SQL**</span><span class="sxs-lookup"><span data-stu-id="ad385-211">**SQL**</span></span>
- <span data-ttu-id="ad385-212">New-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="ad385-212">New-AzureRmSqlDatabase</span></span>
- <span data-ttu-id="ad385-213">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="ad385-213">New-AzureRmSqlDatabaseCopy</span></span>
- <span data-ttu-id="ad385-214">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="ad385-214">New-AzureRmSqlDatabaseSecondary</span></span>
- <span data-ttu-id="ad385-215">New-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="ad385-215">New-AzureRmSqlElasticPool</span></span>
- <span data-ttu-id="ad385-216">New-AzureRmSqlServer</span><span class="sxs-lookup"><span data-stu-id="ad385-216">New-AzureRmSqlServer</span></span>
- <span data-ttu-id="ad385-217">Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="ad385-217">Set-AzureRmSqlDatabase</span></span>
- <span data-ttu-id="ad385-218">Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="ad385-218">Set-AzureRmSqlElasticPool</span></span>
- <span data-ttu-id="ad385-219">Set-AzureRmSqlServer</span><span class="sxs-lookup"><span data-stu-id="ad385-219">Set-AzureRmSqlServer</span></span>

<span data-ttu-id="ad385-220">**Storage**</span><span class="sxs-lookup"><span data-stu-id="ad385-220">**Storage**</span></span>
- <span data-ttu-id="ad385-221">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ad385-221">New-AzureRmStorageAccount</span></span>
- <span data-ttu-id="ad385-222">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ad385-222">Set-AzureRmStorageAccount</span></span>

<span data-ttu-id="ad385-223">**TrafficManager**</span><span class="sxs-lookup"><span data-stu-id="ad385-223">**TrafficManager**</span></span>
- <span data-ttu-id="ad385-224">New-AzureRmTrafficManagerProfile</span><span class="sxs-lookup"><span data-stu-id="ad385-224">New-AzureRmTrafficManagerProfile</span></span>

<br>

<span data-ttu-id="ad385-225">위의 cmdlet 중 하나를 사용하는 스크립트가 있는 경우 `Tags` 매개 변수를 `Tag`로 변경하고 `Tag`를 새 형식으로 변경하여 주요 변경 내용을 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-225">If you have a script that uses any of the above cmdlets, the breaking change can be fixed by changing the `Tags` parameter to `Tag`, as well as changing the `Tag` to the new format.</span></span>

```powershell
# Old
New-AzureRmResourceGroup -Name $resourceGroupName -Location -location -Tags @{ Name = "testtag"; Value = "testval" }

# New
New-AzureRmResourceGroup -Name $resourceGroupName -Location -location -Tag @{ testtag = "testval" }
```

<br>

## <a name="breaking-changes-to-storage-cmdlets"></a><span data-ttu-id="ad385-226">Storage cmdlet의 주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="ad385-226">Breaking changes to Storage cmdlets</span></span>

<span data-ttu-id="ad385-227">이 릴리스에는 다음과 같은 cmdlet이 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-227">The following cmdlets were affected this release:</span></span>

<span data-ttu-id="ad385-228">**Get-AzureRmStorageAccountKey**</span><span class="sxs-lookup"><span data-stu-id="ad385-228">**Get-AzureRmStorageAccountKey**</span></span>
- <span data-ttu-id="ad385-229">cmdlet은 이제 각 키에 대한 속성을 포함하는 개체보다는 키의 목록을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-229">The cmdlet now returns a list of keys, rather than an object with properties for each key</span></span>

```powershell
# Old
$key = (Get-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName).Key1

# New
$key = (Get-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName)[0].Value
```

<span data-ttu-id="ad385-230">**New-AzureRmStorageAccountKey**</span><span class="sxs-lookup"><span data-stu-id="ad385-230">**New-AzureRmStorageAccountKey**</span></span>
- <span data-ttu-id="ad385-231">이 cmdlet의 출력에 있는 `StorageAccountRegenerateKeyResponse` 필드의 이름이 `StorageAccountListKeysResults`로 바뀌었으며 각 키에 대한 속성을 포함하는 개체보다는 키 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-231">`StorageAccountRegenerateKeyResponse` field in output of this cmdlet is renamed to `StorageAccountListKeysResults`, which is now a list of keys rather than an object with properties for each key</span></span>

```powershell
# Old
$key = (New-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName).StorageAccountKeys.Key1

# New
$key = (New-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName).Keys[0].Value
```

<span data-ttu-id="ad385-232">**New/Get/Set-AzureRmStorageAccount**</span><span class="sxs-lookup"><span data-stu-id="ad385-232">**New/Get/Set-AzureRmStorageAccount**</span></span>
- <span data-ttu-id="ad385-233">이 cmdlet의 출력에 있는 `AccountType` 필드의 이름이 `Sku.Name`으로 바뀌었습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-233">`AccountType` field in output of this cmdlet is renamed to `Sku.Name`</span></span>
- <span data-ttu-id="ad385-234">주 끝점/보조 끝점 blob/테이블/큐/파일에 대한 출력 형식이 `Uri`에서 `String`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-234">Output type for PrimaryEndpoints/Secondary endpoints blob/table/queue/file changed from `Uri` to `String`</span></span>

```powershell
# Old
$accountType = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).AccountType

# New
$accountType = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).Sku.Name
```

```powershell
# Old 
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob.ToString()
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob.AbsolutePath

# New
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob.ToString()
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob
```

<br>

## <a name="breaking-changes-to-ad-cmdlets"></a><span data-ttu-id="ad385-235">AD cmdlet의 주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="ad385-235">Breaking changes to AD cmdlets</span></span>

<span data-ttu-id="ad385-236">이 릴리스에는 다음과 같은 cmdlet이 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-236">The following cmdlets were affected this release:</span></span>

<span data-ttu-id="ad385-237">**Get-AzureRMADServicePrincipal**</span><span class="sxs-lookup"><span data-stu-id="ad385-237">**Get-AzureRMADServicePrincipal**</span></span>
- <span data-ttu-id="ad385-238">이 cmdlet의 출력에 있는 `ServicePrincipalName` 필드의 이름이 `ServicePrincipalNames`로 바뀌었고 이제 컬렉션입니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-238">`ServicePrincipalName` field in output of this cmdlet is renamed to `ServicePrincipalNames` and is now a collection.</span></span> <span data-ttu-id="ad385-239">이제 identifierUri와 함께 SPN 중 하나로 `ApplicationId`를 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-239">It now displays `ApplicationId` also as one of the SPN, along with the identifierUri.</span></span>

```powershell
# Old
$servicePrincipals = Get-AzureRmADServicePrincipal -SearchString $displayName
$spn = $servicePrincipals[0].ServicePrincipalName

# New
$servicePrincipals = Get-AzureRmADServicePrincipal -SearchString $displayName
$spn = $servicePrincipals[0].ServicePrincipalNames[0]
```

<span data-ttu-id="ad385-240">**Get-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="ad385-240">**Get-AzureRmADApplication**</span></span>
- <span data-ttu-id="ad385-241">매개 변수 `ApplicationObjectId`의 이름이 `ObjectId`로 바뀌었습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-241">Parameter `ApplicationObjectId` is renamed to `ObjectId`.</span></span>
- <span data-ttu-id="ad385-242">이 cmdlet의 출력에서 `ApplicationObjectId`의 이름이 `ObjectId`로 바뀌었습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-242">In output of this cmdlet, `ApplicationObjectId` is renamed to `ObjectId`.</span></span>

```powershell
# Old
$app = Get-AzureRmADApplication -ApplicationObjectId $applicationObjectId
$objectId = $app.ApplicationObjectId

# New
$app = Get-AzureRmADApplication -ObjectId $objectId
$objectId = $app.ObjectId
```

<span data-ttu-id="ad385-243">**Remove-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="ad385-243">**Remove-AzureRmADApplication**</span></span>
- <span data-ttu-id="ad385-244">매개 변수 `ApplicationObjectId`의 이름이 `ObjectId`로 바뀌었습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-244">Parameter `ApplicationObjectId` is renamed to `ObjectId`.</span></span>

```powershell
# Old
$app = Remove-AzureRmADApplication -ApplicationObjectId $applicationObjectId -Force

# New
$app = Remove-AzureRmADApplication -ObjectId $objectId -Force
```

<span data-ttu-id="ad385-245">**New-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="ad385-245">**New-AzureRmADApplication**</span></span>
- <span data-ttu-id="ad385-246">이 cmdlet의 출력에서 `ApplicationObjectId`의 이름이 `ObjectId`로 바뀌었습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-246">In output of this cmdlet, `ApplicationObjectId` is renamed to `ObjectId`.</span></span>
- <span data-ttu-id="ad385-247">`KeyValue`, `KeyUsage`, `KeyType` 매개 변수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-247">`KeyValue`, `KeyUsage`, `KeyType` parameters are removed.</span></span>

```powershell
# Old
$app = New-AzureRmADApplication -DisplayName $displayName -HomePage $homePage -IdentifierUris $identifierUris -KeyValue $kv -KeyType $kt -KeyUsage $ku
$id = $app.ApplicationObjectId

# New
$app = New-AzureRmADApplication -DisplayName $displayName -HomePage $homePage -IdentifierUris $identifierUris
$id = $app.ObjectId
New-AzureRmADAppCredential -ObjectId $id -Password $kv
```

<span data-ttu-id="ad385-248">**Get-AzureRmADGroup**</span><span class="sxs-lookup"><span data-stu-id="ad385-248">**Get-AzureRmADGroup**</span></span>
- <span data-ttu-id="ad385-249">출력에서 `Mail` 필드가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-249">`Mail` field is removed from the output.</span></span>

<span data-ttu-id="ad385-250">**Get-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="ad385-250">**Get-AzureRmADUser**</span></span>
- <span data-ttu-id="ad385-251">출력에서 `Mail` 필드가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-251">`Mail` field is removed from the output.</span></span>

<span data-ttu-id="ad385-252">**New-AzureRmADServicePrincipal**</span><span class="sxs-lookup"><span data-stu-id="ad385-252">**New-AzureRmADServicePrincipal**</span></span>
- <span data-ttu-id="ad385-253">`DisableAccount` 매개 변수를 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="ad385-253">Removed `DisableAccount` parameter.</span></span>

```powershell
# Old
$servicePrincipal = New-AzureRmADServicePrincipal -DisplayName $displayName -Password $password -DisableAccount true

# New
$servicePrincipal = New-AzureRmADServicePrincipal -DisplayName $displayName -Password $password
Remove-AzureRmADServicePrincipal -ObjectId $servicePrincipal.ObjectId
```