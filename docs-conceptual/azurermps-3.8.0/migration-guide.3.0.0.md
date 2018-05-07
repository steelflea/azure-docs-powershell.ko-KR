# <a name="breaking-changes-for-microsoft-azure-powershell-300"></a>Microsoft Azure PowerShell 3.0.0의 주요 변경 내용입니다.

이 문서는 Microsoft Azure PowerShell cmdlet의 소비자를 위한 주요 변경 내용 알림 및 마이그레이션 가이드 역할을 합니다.  각 섹션에서는 주요 변경에 대한 원동력과 최소 저항의 마이그레이션 경로에 대해 설명합니다.  심층적인 맥락에서는 각 변경 내용과 관련된 끌어오기 요청을 참조하세요.

## <a name="table-of-contents"></a>목차
1. [Data Lake Store cmdlet의 주요 변경 내용](#breaking-changes-to-data-lake-store-cmdlets)
2. [ApiManagement cmdlet의 주요 변경 내용](#breaking-changes-to-apimanagement-cmdlets)
3. [Network cmdlet의 주요 변경 내용](#breaking-changes-to-network-cmdlets)

## <a name="breaking-changes-to-data-lake-store-cmdlets"></a>Data Lake Store cmdlet의 주요 변경 내용

이 릴리스에는 다음과 같은 cmdlet이 적용됩니다([PR 2965](https://github.com/Azure/azure-powershell/pull/2965)).

**Get-AzureRmDataLakeStoreItemAcl(Get-AdlStoreItemAcl)**
- 이 cmdlet이 제거되었고 ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``로 대체되었습니다.
- 이전 cmdlet에서는 ACL(액세스 제어 목록)을 나타내는 복합 개체를 반환했습니다. 새 cmdlet은 선택한 경로의 ACL에 간단한 항목 목록을 반환합니다.

```powershell
# Old
Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo

# New
Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
```

**Get-AzureRmDataLakeStoreItemAclEntry(Get-AdlStoreItemAclEntry)**
- 이 cmdlet이 이전 cmdlet ``Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)``을 대체합니다.
- 이 새로운 cmdlet은 ``DataLakeStoreItemAce[]`` 형식을 포함하는 선택한 경로의 ACL에 간단한 항목 목록을 반환합니다.
- 이 cmdlet의 출력은 다음 cmdlet의 ``-Acl`` 매개 변수에 전달될 수 있습니다.
   - ``Remove-AzureRmDataLakeStoreItemAcl``
   - ``Set-AzureRmDataLakeStoreItemAcl``
   - ``Set-AzureRmDataLakeStoreItemAclEntry``

```powershell
# Old
Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo

# New
Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
```

**Remove-AzureRmDataLakeStoreItemAcl(Remove-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAcl(Set-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAclEntry(Set-AdlStoreItemAclEntry)**
- 이러한 cmdlet은 ``-Acl`` 매개 변수에 대해 ``DataLakeStoreItemAce[]``를 수락합니다.
- ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``에서 ``DataLakeStoreItemAce[]``가 반환됩니다.

```powershell
# Old
$acl = Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo
Set-AdlStoreItemAcl -Account myadlsaccount -Path /foo -Acl $acl

# New
$aclEntries = Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
Set-AdlStoreItemAcl -Account myadlsaccount -Path /foo -Acl $aclEntries
```

## <a name="breaking-changes-to-apimanagement-cmdlets"></a>ApiManagement cmdlet의 주요 변경 내용

이 릴리스에는 다음과 같은 cmdlet이 적용됩니다([PR 2971](https://github.com/Azure/azure-powershell/pull/2971)).

**New-AzureRmApiManagementVirtualNetwork**
- 가상 네트워크를 참조하는 데 필요한 매개 변수가 필수 SubnetName 및 VnetId에서 ``/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ClassicNetwork/virtualNetworks/{virtualNetworkName}/subnets/{subnetName}`` 형식의 SubnetResourceId로 변경되었습니다.

```powershell
# Old
$virtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetName <String> -VnetId <Guid>

# New
$virtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetResourceId <String>

```

**Cmdlet Set-AzureRmApiManagementVirtualNetworks 사용 중지**
- ApiManagement 배포와 관련된 Virtual Network 설정 방법이 둘 이상 있으므로 Cmdlet이 더 이상 사용되지 않습니다.

```powershell
# Old
$networksList = @()
$networksList += New-AzureRmApiManagementVirtualNetwork -Location $vnetLocation -VnetId $vnetId -SubnetName $subnetName
Set-AzureRmApiManagementVirtualNetworks -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetworks $networksList

# New
$masterRegionVirtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetResourceId <String>
Update-AzureRmApiManagementDeployment -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetwork $masterRegionVirtualNetwork
```

## <a name="breaking-changes-to-network-cmdlets"></a>Network cmdlet의 주요 변경 내용

이 릴리스에는 다음과 같은 cmdlet이 적용됩니다([PR 2982](https://github.com/Azure/azure-powershell/pull/2982)).

**New-AzureRmVirtualNetworkGateway**
- 새로 생성된 가상 네트워크 게이트웨이에서 Active-Active 기능을 사용하기 위해 ``:- Bool parameter:-ActiveActive``가 제거되고 ``SwitchParameter:-EnableActiveActiveFeature``가 추가된 변경 내용에 대한 설명입니다.

```powershell
# Old 
# Sample of how the cmdlet was previously called
New-AzureRmVirtualNetworkGateway -ResourceGroupName $rgname -name $rname -Location $location -IpConfigurations $vnetIpConfig1,$vnetIpConfig2 -GatewayType Vpn -VpnType RouteBased -EnableBgp $false -GatewaySku HighPerformance -ActiveActive $true

# New
# Sample of how the cmdlet should now be called
New-AzureRmVirtualNetworkGateway -ResourceGroupName $rgname -name $rname -Location $location -IpConfigurations $vnetIpConfig1,$vnetIpConfig2 -GatewayType Vpn -VpnType RouteBased -EnableBgp $false -GatewaySku HighPerformance -EnableActiveActiveFeature
```

Set-AzureRmVirtualNetworkGateway
- 가상 네트워크 게이트웨이에서 Active-Active 기능을 사용 및 사용하지 않기 위해 ``:- Bool parameter:-ActiveActive``가 제거되고 두 ``SwitchParameters:-EnableActiveActiveFeature`` / ``DisableActiveActiveFeature``가 추가된 변경 내용에 대한 설명입니다.

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