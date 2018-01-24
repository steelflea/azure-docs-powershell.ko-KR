# <a name="breaking-changes-for-microsoft-azure-powershell-300"></a><span data-ttu-id="5e739-101">Microsoft Azure PowerShell 3.0.0의 주요 변경 내용입니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-101">Breaking changes for Microsoft Azure PowerShell 3.0.0.</span></span>

<span data-ttu-id="5e739-102">이 문서는 Microsoft Azure PowerShell cmdlet의 소비자를 위한 주요 변경 내용 알림 및 마이그레이션 가이드 역할을 합니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-102">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span>  <span data-ttu-id="5e739-103">각 섹션에서는 주요 변경에 대한 원동력과 최소 저항의 마이그레이션 경로에 대해 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-103">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span>  <span data-ttu-id="5e739-104">심층적인 맥락에서는 각 변경 내용과 관련된 끌어오기 요청을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="5e739-104">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="5e739-105">목차</span><span class="sxs-lookup"><span data-stu-id="5e739-105">Table of Contents</span></span>
1. [<span data-ttu-id="5e739-106">Data Lake Store cmdlet의 주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="5e739-106">Breaking changes to Data Lake Store cmdlets</span></span>](#breaking-changes-to-data-lake-store-cmdlets)
2. [<span data-ttu-id="5e739-107">ApiManagement cmdlet의 주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="5e739-107">Breaking changes to ApiManagement cmdlets</span></span>](#breaking-changes-to-apimanagement-cmdlets)
3. [<span data-ttu-id="5e739-108">Network cmdlet의 주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="5e739-108">Breaking changes to Network cmdlets</span></span>](#breaking-changes-to-network-cmdlets)

## <a name="breaking-changes-to-data-lake-store-cmdlets"></a><span data-ttu-id="5e739-109">Data Lake Store cmdlet의 주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="5e739-109">Breaking changes to Data Lake Store cmdlets</span></span>

<span data-ttu-id="5e739-110">이 릴리스에는 다음과 같은 cmdlet이 적용됩니다([PR 2965](https://github.com/Azure/azure-powershell/pull/2965)).</span><span class="sxs-lookup"><span data-stu-id="5e739-110">The following cmdlets were affected this release ([PR 2965](https://github.com/Azure/azure-powershell/pull/2965)):</span></span>

<span data-ttu-id="5e739-111">**Get-AzureRmDataLakeStoreItemAcl(Get-AdlStoreItemAcl)**</span><span class="sxs-lookup"><span data-stu-id="5e739-111">**Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)**</span></span>
- <span data-ttu-id="5e739-112">이 cmdlet이 제거되었고 ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``로 대체되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-112">This cmdlet was removed and replaced with ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``.</span></span>
- <span data-ttu-id="5e739-113">이전 cmdlet에서는 ACL(액세스 제어 목록)을 나타내는 복합 개체를 반환했습니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-113">The old cmdlet returned a complex object representing the access control list (ACL).</span></span> <span data-ttu-id="5e739-114">새 cmdlet은 선택한 경로의 ACL에 간단한 항목 목록을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-114">The new cmdlet returns a simple list of entries in the chosen path's ACL.</span></span>

```powershell
# Old
Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo

# New
Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
```

<span data-ttu-id="5e739-115">**Get-AzureRmDataLakeStoreItemAclEntry(Get-AdlStoreItemAclEntry)**</span><span class="sxs-lookup"><span data-stu-id="5e739-115">**Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)**</span></span>
- <span data-ttu-id="5e739-116">이 cmdlet이 이전 cmdlet ``Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)``을 대체합니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-116">This cmdlet replaces the old cmdlet ``Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)``.</span></span>
- <span data-ttu-id="5e739-117">이 새로운 cmdlet은 ``DataLakeStoreItemAce[]`` 형식을 포함하는 선택한 경로의 ACL에 간단한 항목 목록을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-117">This new cmdlet returns a simple list of entries in the chosen path's ACL, with type ``DataLakeStoreItemAce[]``.</span></span>
- <span data-ttu-id="5e739-118">이 cmdlet의 출력은 다음 cmdlet의 ``-Acl`` 매개 변수에 전달될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-118">The output of this cmdlet can be passed in to the ``-Acl`` parameter of the following cmdlets:</span></span>
   - ``Remove-AzureRmDataLakeStoreItemAcl``
   - ``Set-AzureRmDataLakeStoreItemAcl``
   - ``Set-AzureRmDataLakeStoreItemAclEntry``

```powershell
# Old
Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo

# New
Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
```

<span data-ttu-id="5e739-119">**Remove-AzureRmDataLakeStoreItemAcl(Remove-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAcl(Set-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAclEntry(Set-AdlStoreItemAclEntry)**</span><span class="sxs-lookup"><span data-stu-id="5e739-119">**Remove-AzureRmDataLakeStoreItemAcl (Remove-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAcl (Set-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAclEntry (Set-AdlStoreItemAclEntry)**</span></span>
- <span data-ttu-id="5e739-120">이러한 cmdlet은 ``-Acl`` 매개 변수에 대해 ``DataLakeStoreItemAce[]``를 수락합니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-120">These cmdlets now accept ``DataLakeStoreItemAce[]`` for the ``-Acl`` parameter.</span></span>
- <span data-ttu-id="5e739-121">``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``에서 ``DataLakeStoreItemAce[]``가 반환됩니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-121">``DataLakeStoreItemAce[]`` is returned by ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``.</span></span>

```powershell
# Old
$acl = Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo
Set-AdlStoreItemAcl -Account myadlsaccount -Path /foo -Acl $acl

# New
$aclEntries = Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
Set-AdlStoreItemAcl -Account myadlsaccount -Path /foo -Acl $aclEntries
```

## <a name="breaking-changes-to-apimanagement-cmdlets"></a><span data-ttu-id="5e739-122">ApiManagement cmdlet의 주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="5e739-122">Breaking changes to ApiManagement cmdlets</span></span>

<span data-ttu-id="5e739-123">이 릴리스에는 다음과 같은 cmdlet이 적용됩니다([PR 2971](https://github.com/Azure/azure-powershell/pull/2971)).</span><span class="sxs-lookup"><span data-stu-id="5e739-123">The following cmdlets were affected this release ([PR 2971](https://github.com/Azure/azure-powershell/pull/2971)):</span></span>

<span data-ttu-id="5e739-124">**New-AzureRmApiManagementVirtualNetwork**</span><span class="sxs-lookup"><span data-stu-id="5e739-124">**New-AzureRmApiManagementVirtualNetwork**</span></span>
- <span data-ttu-id="5e739-125">가상 네트워크를 참조하는 데 필요한 매개 변수가 필수 SubnetName 및 VnetId에서 ``/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ClassicNetwork/virtualNetworks/{virtualNetworkName}/subnets/{subnetName}`` 형식의 SubnetResourceId로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-125">The required parameters to reference a virtual network changed from requiring SubnetName and VnetId to SubnetResourceId in format ``/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ClassicNetwork/virtualNetworks/{virtualNetworkName}/subnets/{subnetName}``</span></span>

```powershell
# Old
$virtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetName <String> -VnetId <Guid>

# New
$virtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetResourceId <String>

```

<span data-ttu-id="5e739-126">**Cmdlet Set-AzureRmApiManagementVirtualNetworks 사용 중지**</span><span class="sxs-lookup"><span data-stu-id="5e739-126">**Deprecating Cmdlet Set-AzureRmApiManagementVirtualNetworks**</span></span>
- <span data-ttu-id="5e739-127">ApiManagement 배포와 관련된 Virtual Network 설정 방법이 둘 이상 있으므로 Cmdlet이 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-127">The Cmdlet is getting deprecated as there was more than one way to Set Virtual Network associated to ApiManagement deployment.</span></span>

```powershell
# Old
$networksList = @()
$networksList += New-AzureRmApiManagementVirtualNetwork -Location $vnetLocation -VnetId $vnetId -SubnetName $subnetName
Set-AzureRmApiManagementVirtualNetworks -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetworks $networksList

# New
$masterRegionVirtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetResourceId <String>
Update-AzureRmApiManagementDeployment -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetwork $masterRegionVirtualNetwork
```

## <a name="breaking-changes-to-network-cmdlets"></a><span data-ttu-id="5e739-128">Network cmdlet의 주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="5e739-128">Breaking changes to Network cmdlets</span></span>

<span data-ttu-id="5e739-129">이 릴리스에는 다음과 같은 cmdlet이 적용됩니다([PR 2982](https://github.com/Azure/azure-powershell/pull/2982)).</span><span class="sxs-lookup"><span data-stu-id="5e739-129">The following cmdlets were affected this release ([PR 2982](https://github.com/Azure/azure-powershell/pull/2982)):</span></span>

<span data-ttu-id="5e739-130">**New-AzureRmVirtualNetworkGateway**</span><span class="sxs-lookup"><span data-stu-id="5e739-130">**New-AzureRmVirtualNetworkGateway**</span></span>
- <span data-ttu-id="5e739-131">새로 생성된 가상 네트워크 게이트웨이에서 Active-Active 기능을 사용하기 위해 ``:- Bool parameter:-ActiveActive``가 제거되고 ``SwitchParameter:-EnableActiveActiveFeature``가 추가된 변경 내용에 대한 설명입니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-131">Description of what has changed ``:- Bool parameter:-ActiveActive`` is removed and ``SwitchParameter:-EnableActiveActiveFeature`` is added for enabling Active-Active feature on newly creating virtual network gateway.</span></span>

```powershell
# Old 
# Sample of how the cmdlet was previously called
New-AzureRmVirtualNetworkGateway -ResourceGroupName $rgname -name $rname -Location $location -IpConfigurations $vnetIpConfig1,$vnetIpConfig2 -GatewayType Vpn -VpnType RouteBased -EnableBgp $false -GatewaySku HighPerformance -ActiveActive $true

# New
# Sample of how the cmdlet should now be called
New-AzureRmVirtualNetworkGateway -ResourceGroupName $rgname -name $rname -Location $location -IpConfigurations $vnetIpConfig1,$vnetIpConfig2 -GatewayType Vpn -VpnType RouteBased -EnableBgp $false -GatewaySku HighPerformance -EnableActiveActiveFeature
```

<span data-ttu-id="5e739-132">Set-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="5e739-132">Set-AzureRmVirtualNetworkGateway</span></span>
- <span data-ttu-id="5e739-133">가상 네트워크 게이트웨이에서 Active-Active 기능을 사용 및 사용하지 않기 위해 ``:- Bool parameter:-ActiveActive``가 제거되고 두 ``SwitchParameters:-EnableActiveActiveFeature`` / ``DisableActiveActiveFeature``가 추가된 변경 내용에 대한 설명입니다.</span><span class="sxs-lookup"><span data-stu-id="5e739-133">Description of what has changed ``:- Bool parameter:-ActiveActive`` is removed and 2 ``SwitchParameters:-EnableActiveActiveFeature`` / ``DisableActiveActiveFeature`` are added for enabling and disabling Active-Active feature on virtual network gateway.</span></span>

```powershell
# Old
# Sample of how the cmdlet was previously called
Set-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $gw -ActiveActive $true
Set-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $gw -ActiveActive $false  

# New
# Sample of how the cmdlet should now be called
Set-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $gw -EnableActiveActiveFeature
Set-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $gw -DisableActiveActiveFeature
```