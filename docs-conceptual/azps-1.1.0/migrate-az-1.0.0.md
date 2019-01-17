---
title: Microsoft Azure PowerShell Az 1.0.0의 호환성이 손상되는 변경
description: 이 마이그레이션 가이드에는 Azure PowerShell Az 버전 1 릴리스의 호환성이 손상되는 변경에 대한 목록이 포함되어 있습니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/14/2018
ms.openlocfilehash: be3e19dc4b689adbc63b933dd9f3454122d5344a
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342208"
---
# <a name="migration-guide-for-az-100"></a>Az 1.0.0에 대한 마이그레이션 가이드

이 문서에서는 AzureRM 6.x 버전과 Az 1.0.0 버전 간의 변경 내용을 설명합니다.

## <a name="table-of-contents"></a>목차
- [일반적인 주요 변경 내용](#general-breaking-changes)
  - [Cmdlet 명사 접두사 변경](#cmdlet-noun-prefix-changes)
  - [모듈 이름 변경](#module-name-changes)
  - [제거된 모듈](#removed-modules)
  - [Windows PowerShell 5.1 및 .NET 4.7.2](#windows-powershell-51-and-net-472)
  - [PSCredential을 사용하여 사용자 로그인 임시 제거](#temporary-removal-of-user-login-using-pscredential)
  - [웹 브라우저 프롬프트 대신 기본 디바이스 코드 로그인](#temporary-default-device-code-login-instead-of-web-browser-prompt)
- [모듈의 호환성이 손상되는 변경](#module-breaking-changes)
  - [Az.ApiManagement(이전에는 AzureRM.ApiManagement)](#azapimanagement-previously-azurermapimanagement)
  - [Az.Billing(이전에는 AzureRM.Billing, AzureRM.Consumption, 및 AzureRM.UsageAggregates)](#azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates)
  - [Az.CognitiveServices(이전에는 AzureRM.CognitiveServices)](#azcognitiveservices-previously-azurermcognitiveservices)
  - [Az.Compute(이전에는 AzureRM.Compute)](#azcompute-previously-azurermcompute)
  - [Az.DataFactory(이전에는 AzureRM.DataFactories 및 AzureRM.DataFactoryV2)](#azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2)
  - [Az.DataLakeAnalytics(이전에는 AzureRM.DataLakeAnalytics)](#azdatalakeanalytics-previously-azurermdatalakeanalytics)
  - [Az.DataLakeStore(이전에는 AzureRM.DataLakeStore)](#azdatalakestore-previously-azurermdatalakestore)
  - [Az.KeyVault(이전에는 AzureRM.KeyVault)](#azkeyvault-previously-azurermkeyvault)
  - [Az.Media(이전에는 AzureRM.Media)](#azmedia-previously-azurermmedia)
  - [Az.Monitor(이전에는 AzureRM.Insights)](#azmonitor-previously-azurerminsights)
  - [Az.Network(이전에는 AzureRM.Network)](#aznetwork-previously-azurermnetwork)
  - [Az.OperationalInsights(이전에는 AzureRM.OperationalInsights)](#azoperationalinsights-previously-azurermoperationalinsights)
  - [Az.RecoveryServices(이전에는 AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, 및 AzureRM.RecoveryServices.SiteRecovery)](#azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery)
  - [Az.Resources(이전에는 AzureRM.Resources)](#azresources-previously-azurermresources)
  - [Az.ServiceFabric(이전에는 AzureRM.ServiceFabric)](#azservicefabric-previously-azurermservicefabric)
  - [Az.Sql(이전에는 AzureRM.Sql)](#azsql-previously-azurermsql)
  - [Az.Storage(이전에는 Azure.Storage 및 AzureRM.Storage)](#azstorage-previously-azurestorage-and-azurermstorage)
  - [Az.Websites(이전에는 AzureRM.Websites)](#azwebsites-previously-azurermwebsites)

## <a name="general-breaking-changes"></a>일반적인 주요 변경 내용
### <a name="cmdlet-noun-prefix-changes"></a>Cmdlet 명사 접두사 변경
AzureRM에서는 cmdlet 명사 접두사로 'AzureRM' 또는 'Azure'를 사용합니다.  Az는 cmndlet 이름을 단순화하고 정규화하여 모든 cmdlet이 'Az'를 cmdlet 명사 접두사로 사용합니다. 예: 
```powershell
Get-AzureRMVM
Get-AzureKeyVaultSecret
```

다음으로 변경되었습니다.
```powershell
Get-AzVM
Get-AzKeyVaultSecret
```

이러한 새 cmdlet 이름으로의 전환을 보다 간단하게 만들기 위해 Az는 두 가지 새로운 cmdlet인 ```Enable-AzureRmAlias```와 ```Disable-AzureRmAlias```를 도입했습니다.  ```Enable-AzureRmAlias```는 AzureRM의 이전 cmdlet 이름에서 최신 Az cmdlet 이름의 별칭을 만듭니다.  cmdlet을 사용하면 사용자 또는 컴퓨터 프로필을 변경하여 현재 세션에서 또는 모든 세션에서 별칭을 만들 수 있습니다. 

예를 들어, AzureRM의 다음 스크립트가 있습니다.
```powershell
#Requires -Modules AzureRM.Storage
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

```Enable-AzureRmAlias```를 사용하여 최소한의 변경으로 실행할 수 있습니다.
```powershell
#Requires -Modules Az.Storage
Enable-AzureRmAlias
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

```Enable-AzureRmAlias -Scope CurrentUser```를 실행하면 열려 있는 모든 powershell 세션의 별칭이 활성화되므로 이 cmdlet을 실행한 후 이와 같은 스크립트를 변경할 필요가 없습니다.
```powershell
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

별칭 cmdlet 사용에 대한 자세한 내용은 powershell 프롬프트에서 ```Get-Help -Online Enable-AzureRmAlias```를 실행합니다.

```Disable-AzureRmAlias```는 ```Enable-AzureRmAlias```로 만든 AzureRM cmdlet 별칭을 제거합니다.  자세한 내용은 powershell 프롬프트에서 ```Get-Help -Online Disable-AzureRmAlias```를 실행합니다.

### <a name="module-name-changes"></a>모듈 이름 변경
- 다음 모듈을 제외하고 모듈 이름이 `AzureRM.*`에서 `Az.*`로 변경되었습니다.
```
AzureRM.Profile                       -> Az.Accounts
Azure.AnalysisServices                -> Az.AnalysisServices
AzureRM.Consumption                   -> Az.Billing
AzureRM.UsageAggregates               -> Az.Billing
AzureRM.DataFactories                 -> Az.DataFactory
AzureRM.DataFactoryV2                 -> Az.DataFactory
AzureRM.MachineLearningCompute        -> Az.MachineLearning
AzureRM.Insights                      -> Az.Monitor
AzureRM.RecoveryServices.Backup       -> Az.RecoveryServices
AzureRM.RecoveryServices.SiteRecovery -> Az.RecoveryServices
AzureRM.Tags                          -> Az.Resources
Azure.Storage                         -> Az.Storage
```

모듈 이름이 변경되면 ```#Requires``` 또는 ```Import-Module```을 사용하여 특정 모듈을 로드하는 스크립트는 대신 새 모듈을 사용하도록 변경되어야 합니다.

#### <a name="migrating-requires-statements"></a>#Requires 문 마이그레이션
#Requires를 사용하여 AzureRM 모듈에 대한 의존성을 선언하는 스크립트는 새 모듈 이름을 사용하도록 업데이트해야 합니다.
```powershell
#Requires -Module AzureRM.Compute
```

다음과 같이 변경되어야 합니다.
```powershell
#Requires -Module Az.Compute
```

#### <a name="migrating-import-module-statements"></a>모듈 가져오기 문 마이그레이션
```Import-Module```을 사용하여 AzureRM 모듈을 로드하는 스크립트는 새 모듈 이름을 반영하도록 업데이트해야 합니다.
```powershell
Import-Module -Name AzureRM.Compute
```

다음과 같이 변경되어야 합니다.
```powershell
Import-Module -Name Az.Compute
```

### <a name="migrating-fully-qualified-cmdlet-invocations"></a>Cmdlet 정규화 호출 마이그레이션
다음과 같이 모듈 규정 cmdlet 호출을 사용하는 스크립트
```powershell
AzureRM.Compute\Get-AzureRmVM
```

새 모듈 및 cmdlet 이름을 사용하도록 변경되어야 합니다.
```powershell
Az.Compute\Get-AzVM
```

### <a name="migrating-module-manifest-dependencies"></a>모듈 매니페스트 종속성 마이그레이션
모듈 매니페스트(.psd1) 파일을 통해 AzureRM 모듈에 대한 종속성을 나타내는 모듈은 'RequiredModules'섹션에서 모듈 이름을 업데이트해야 합니다

```powershell
RequiredModules = @(@{ModuleName="AzureRM.Profile"; ModuleVersion="5.8.2"})
```

다음과 같이 변경되어야 합니다.

```powershell
RequiredModules = @(@{ModuleName="Az.Profile"; ModuleVersion="1.0.0"})
```

### <a name="removed-modules"></a>제거된 모듈
- `AzureRM.Backup`
- `AzureRM.Compute.ManagedService`
- `AzureRM.Scheduler`

이러한 서비스에 대한 도구는 더 이상 지원되지 않습니다.  편리한 대체 서비스로 이동하는 것이 좋습니다.

### <a name="windows-powershell-51-and-net-472"></a>Windows PowerShell 5.1 및 .NET 4.7.2
- Az를 사용 하 여 Windows PowerShell 5.1을 사용하려면 .NET 4.7.2를 설치해야 합니다. PowerShell Core를 사용하여 Az를 사용하려면 .NET 4.7.2가 필요하지 않습니다. 

### <a name="temporary-removal-of-user-login-using-pscredential"></a>PSCredential을 사용하여 사용자 로그인 임시 제거
- .NET 표준의 인증 흐름이 변경되어 PSCredential을 통한 사용자 로그인이 일시적으로 제거됩니다. 이 기능은 Windows PowerShell 5.1용 2019년 1월 15일 릴리스에서 다시 도입됩니다. [이 문제](https://github.com/Azure/azure-powershell/issues/7430)는 자세히 다루고 있습니다.

### <a name="default-device-code-login-instead-of-web-browser-prompt"></a>웹 브라우저 프롬프트 대신 기본 디바이스 코드 로그인
- .NET 표준의 인증 흐름이 변경되어 대화식 로그인 중에 기본 로그인 흐름으로 디바이스 로그인을 사용합니다. 웹 브라우저 기반 로그인은 Windows PowerShell 5.1에서 2019년 1월 15일 릴리스의 기본값으로 다시 도입됩니다. 이때 사용자는 스위치 매개 변수를 사용하여 디바이스 로그인을 선택할 수 있습니다.

## <a name="module-breaking-changes"></a>모듈의 호환성이 손상되는 변경

### <a name="azapimanagement-previously-azurermapimanagement"></a>Az.ApiManagement(이전에는 AzureRM.ApiManagement)
- 다음 cmdlet이 제거됩니다.
  - New-AzureRmApiManagementHostnameConfiguration
  - Set-AzureRmApiManagementHostnames
  - Update-AzureRmApiManagementDeployment
  - Import-AzureRmApiManagementHostnameCertificate
  - 이러한 속성 설정을 위해 **Set-AzApiManagement**를 사용합니다.
- 다음과 같은 속성이 제거되었습니다.
  - `PsApiManagementContext`에서 `PsApiManagementHostnameConfiguration` 형식의 `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration`, `ScmHostnameConfiguration` 속성을 제거했습니다. 대신 `PsApiManagementCustomHostNameConfiguration` 형식의 `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration`, `ScmCustomHostnameConfiguration`을 사용합니다.
  - PsApiManagementContext에서 `StaticIPs`속성을 제거했습니다. 해당 속성은 `PublicIPAddresses`, `PrivateIPAddresses`로 분할되었습니다.
  - 필수 속성 `Location`을 New-AzureApiManagementVirtualNetwork cmdlet에서 제거했습니다.

### <a name="azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates"></a>Az.Billing(이전에는 AzureRM.Billing, AzureRM.Consumption, 및 AzureRM.UsageAggregates)
- `InvoiceName` 매개 변수가 `Get-AzConsumptionUsageDetail` cmdlet에서 제거되었습니다.  스크립트는 청구서에 대한 다른 ID 매개 변수를 사용해야 합니다.

### <a name="azcognitiveservices-previously-azurermcognitiveservices"></a>Az.CognitiveServices(이전에는 AzureRM.CognitiveServices)
- `Get-AzCognitiveServicesAccountSkus` cmdlet에서 `GetSkusWithAccountParamSetName` 매개 변수 집합을 제거했습니다.  ResourceGroupName 및 계정 이름을 사용하는 대신 계정 형식 및 위치별로 SKU를 가져와야 합니다.

### <a name="azcompute-previously-azurermcompute"></a>Az.Compute(이전에는 AzureRM.Compute)
- `PSVirtualMachine` 및 `PSVirtualMachineScaleSet` 객체의 `Identity` 속성에서 `IdentityIds`가 제거되었습니다. 스크립트는 더 이상 이 필드의 값을 사용하여 처리 결정을 내려서는 안됩니다.
- `PSVirtualMachineScaleSetVM` 개체의 `InstanceView` 속성의 형식이 `VirtualMachineInstanceView`에서 `VirtualMachineScaleSetVMInstanceView`로 변경되었습니다.
- `UpgradePolicy` 속성에서 `AutoOSUpgradePolicy` 및 `AutomaticOSUpgrade` 속성이 제거되었습니다.
- `PSSnapshotUpdate` 개체의 `Sku` 속성의 형식이 `DiskSku`에서 `SnapshotSku`로 변경되었습니다.
- `VmScaleSetVMParameterSet`이 `Add-AzVMDataDisk` cmdlet에서 제거되면 더 이상 ScaleSet VM에 개별적으로 데이터 디스크를 추가할 수 없습니다.

### <a name="azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2"></a>Az.DataFactory(이전에는 AzureRM.DataFactories 및 AzureRM.DataFactoryV2)
- `GatewayName` 매개 변수가 `New-AzDataFactoryEncryptValue` cmdlet에서 필수 항목이 되었습니다.
- `New-AzDataFactoryGatewayKey` cmdlet이 제거됨
- `Get-AzDataFactoryV2ActivityRun` cmdlet에서 `LinkedServiceName` 매개 변수가 제거되었습니다. 스크립트는 더 이상 이 필드의 값을 사용하여 처리 결정을 내려서는 안됩니다.

### <a name="azdatalakeanalytics-previously-azurermdatalakeanalytics"></a>Az.DataLakeAnalytics(이전에는 AzureRM.DataLakeAnalytics)
- 사용되지 않는 cmdlet 제거: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret`, `Set-AzDataLakeAnalyticsCatalogSecret`

### <a name="azdatalakestore-previously-azurermdatalakestore"></a>Az.DataLakeStore(이전에는 AzureRM.DataLakeStore)
- 다음 cmdlet의 `Encoding` 매개 변수는 `FileSystemCmdletProviderEncoding` 형식에서 `System.Text.Encoding` 형식으로 변경되었습니다. 이 변경은 인코딩 값 `String` 및 `Oem`을 제거합니다. 다른 모든 이전 인코딩 값은 유지됩니다.
  - New-AzureRmDataLakeStoreItem
  - Add-AzureRmDataLakeStoreItemContent
  - Get-AzureRmDataLakeStoreItemContent
- 사용되지 않는 `Tags` 속성 별칭을 `New-AzDataLakeStoreAccount` 및 `Set-AzDataLakeStoreAccount` cmdlet에서 제거함

  다음을 사용하는 스크립트
  ```powershell
  New-AzureRMDataLakeStoreAccount -Tags @{TagName="TagValue"}
  ```

  다음과 같이 변경되어야 합니다.
  ```powershell
  New-AzDataLakeStoreAccount -Tag @{TagName="TagValue"}
  ```

- ```PSDataLakeStoreAccountBasic``` 개체에서 사용되지 않는 속성 ```Identity```, ```EncryptionState```, ```EncrypotionProvisioningState```, ```EncryptionConfig```, ```FirewallState```, ```FirewallRules```, ```VirtualNetworkRules```, ```TrustedIdProviderState```, ```TrustedIdProviders```, ```DefaultGroup```, ```NewTier```, ```CurrentTier```, ```FirewallAllowAzureIps```을 제거했습니다.  ```Get-AzDataLakeStoreAccount```에서 반환된 ```PSDatalakeStoreAccount```를 사용하는 모든 스크립트는 이러한 속성을 참조하지 않아야 합니다.

### <a name="azkeyvault-previously-azurermkeyvault"></a>Az.KeyVault(이전에는 AzureRM.KeyVault)
- `PurgeDisabled` 속성이 `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem` 및 `PSKeyVaultSecretAttributes` 개체에서 제거되었습니다. 스크립트는 더 이상 처리 결정을 내리기 위해 ```PurgeDisabled``` 속성을 참조하지 않습니다.

### <a name="azmedia-previously-azurermmedia"></a>Az.Media(이전에는 AzureRM.Media)
- 다음을 사용하여 `New-AzMediaService` cmdlet에서 사용되지 않는 `Tags` 속성 별칭을 제거합니다.
  ```powershell
  New-AzureRMMediaService -Tags @{TagName="TagValue"}
  ```

  다음과 같이 변경되어야 합니다.
  ```powershell
  New-AzMMediaService -Tag @{TagName="TagValue"}
  ```
### <a name="azmonitor-previously-azurerminsights"></a>Az.Monitor(이전에는 AzureRM.Insights)
- `Set-AzDiagnosticSetting` cmdlet 스크립트에서 다음을 사용하여 단일 매개 변수 이름을 위해 복수 이름 `Categories` 및 `Timegrains` 매개 변수를 제거했습니다.
  ```powershell
  Set-AzureRmDiagnosticSetting -Timegrains PT1M -Categories Category1, Category2
  ```

  다음과 같이 변경되어야 합니다.
  ```powershell
  Set-AzDiagnosticSetting -Timegrain PT1M -Category Category1, Category2
  ```
### <a name="aznetwork-previously-azurermnetwork"></a>Az.Network(이전에는 AzureRM.Network)
- 사용되지 않는 매개 변수 `ResourceId`를 `Get-AzServiceEndpointPolicyDefinition` cmdlet에서 제거
- `PSVirtualNetwork` 개체에서 사용되지 않는 속성 `EnableVmProtection`을 제거했습니다.
- 사용되지 않는 cmdlet 제거: `Set-AzVirtualNetworkGatewayVpnClientConfig`
  
스크립트는 더 이상이 필드의 값을 기반으로 처리 결정을 내려서는 안됩니다.

### <a name="azoperationalinsights-previously-azurermoperationalinsights"></a>Az.OperationalInsights(이전에는 AzureRM.OperationalInsights)
- `Get-AzOperationalInsightsDataSource`에 설정된 기본 매개 변수가 제거되고 `ByWorkspaceNameByKind`가 기본 매개 변수 집합이 되었습니다.

  다음을 사용하여 데이터 원본을 나열하는 스크립트
  ```powershell
  Get-AzureRmOperationalInsightsDataSource
  ```

  종류를 지정하도록 변경되어야 합니다.
  ```powershell
  Get-AzOperationalInsightsDataSource -Kind AzureActivityLog
  ```

### <a name="azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery"></a>Az.RecoveryServices(이전에는 AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, 및 AzureRM.RecoveryServices.SiteRecovery)
- `New/Set-AzRecoveryServicesAsrPolicy` cmdlet에서 `Encryption` 매개 변수를 제거했습니다.
- `TargetStorageAccountName` 매개 변수는 이제 `Restore-AzRecoveryServicesBackupItem` cmdlet의 관리 디스크 복원에 필수 항목입니다.
- `Restore-AzRecoveryServicesBackupItem` cmdlet에서 `StorageAccountName`, `StorageAccountResourceGroupName` 매개 변수 제거
- `Get-AzRecoveryServicesBackupContainer` cmdlet에서 `Name` 매개 변수 제거

### <a name="azresources-previously-azurermresources"></a>Az.Resources(이전에는 AzureRM.Resources)
- `New/Set-AzPolicyAssignment` cmdlet에서 `Sku` 매개 변수를 제거했습니다.
- `New-AzADServicePrincipal` 및 `New-AzADSpCredential` cmdlet에서 `Password` 매개 변수를 제거했습니다. 암호는 자동으로 생성되며 암호를 제공하는 스크립트는 다음과 같습니다.
  ```powershell
  New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476 -Password $secPassword
  ```

  출력에서 암호를 검색하도록 변경해야 합니다.
  ```powershell
  $credential = New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476
  $secPassword = $credential.Secret
  ```

### <a name="azservicefabric-previously-azurermservicefabric"></a>Az.ServiceFabric(이전에는 AzureRM.ServiceFabric)
- 다음 cmdlet 반환 형식이 변경되었습니다.
  - `ApplicationHealthPolicy` 형식의 속성 `SerivceTypeHealthPolicies`가 제거되었습니다.
  - `ClusterUpgradeDeltaHealthPolicy` 형식의 속성 `ApplicationHealthPolicies`가 제거되었습니다.
  - `ClusterUpgradePolicy` 형식의 속성 `OverrideUserUpgradePolicy`가 제거되었습니다.
  - 이러한 변경 내용은 다음 cmdlet에 영향을 줍니다.
    - Add-AzServiceFabricClientCertificate
    - Add-AzServiceFabricClusterCertificate
    - Add-AzServiceFabricNode
    - Add-AzServiceFabricNodeType
    - Get-AzServiceFabricCluster
    - Remove-AzServiceFabricClientCertificate
    - Remove-AzServiceFabricClusterCertificate
    - Remove-AzServiceFabricNode
    - Remove-AzServiceFabricNodeType
    - Remove-AzServiceFabricSetting
    - Set-AzServiceFabricSetting
    - Set-AzServiceFabricUpgradeType
    - Update-AzServiceFabricDurability
    - Update-AzServiceFabricReliability

### <a name="azsql-previously-azurermsql"></a>Az.Sql(이전에는 AzureRM.Sql)
- `Set-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet에서 `State`, `ResourceId` 매개 변수 제거
- 사용되지 않는 cmdlet 제거: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing`, `Remove-AzSqlServerAuditing`
- 사용되지 않는 매개 변수 `Current`를 `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet에서 제거
- 사용되지 않는 매개 변수 `DatabaseName`을 `Get-AzSqlServerServiceObjective` cmdlet에서 제거
- 사용되지 않는 매개 변수 `PrivilegedLogin`을 `Set-AzSqlDatabaseDataMaskingPolicy` cmdlet에서 제거

### <a name="azstorage-previously-azurestorage-and-azurermstorage"></a>Az.Storage(이전에는 Azure.Storage 및 AzureRM.Storage)
- 스토리지 계정 이름만 사용하여 Oauth 스토리지 컨텍스트를 만들 수 있도록 기본 매개 변수 집합이 `OAuthParameterSet`으로 변경되었습니다.
  - 예제: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`
- `Location` 매개 변수가 `Get-AzStorageUsage` cmdlet에서 필수 항목이 되었습니다.
- 이제 Storage API 메서드는 동기 API 호출 대신 작업 기반 비동기 패턴(TAP)을 사용합니다.
#### <a name="1-blob-snapshot"></a>1. BLOB 스냅숏
##### <a name="before"></a>이전:
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$b.ICloudBlob.Snapshot()
```

##### <a name="after"></a>이후:
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$task = $b.ICloudBlob.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="2-share-snapshot"></a>2. 스냅숏 공유
##### <a name="before"></a>이전:
```powershell
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$snapshot = $Share.Snapshot()
```
#####  <a name="after"></a>이후:
```powershell

$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$task = $Share.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="3-undelete-a-soft-delete-blob"></a>3. 일시 삭제 BLOB 삭제 취소
##### <a name="before"></a>이전:
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$b.ICloudBlob.Undelete()
```
##### <a name="after"></a>이후:
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$task = $b.ICloudBlob.UndeleteAsync()
$task.Wait()
```

#### <a name="4-set-blob-tier"></a>4. BLOB 계층 설정
##### <a name="before"></a>이전:
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$blockBlob.ICloudBlob.SetStandardBlobTier("hot")

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$pageBlob.ICloudBlob.SetPremiumBlobTier("P4")
```

##### <a name="after"></a>이후:
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$task = $blockBlob.ICloudBlob.SetStandardBlobTierAsync("hot")
$task.Wait()

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$task = $pageBlob.ICloudBlob.SetPremiumBlobTierAsync("P4")
$task.Wait()
```

### <a name="azwebsites-previously-azurermwebsites"></a>Az.Websites(이전에는 AzureRM.Websites)
- 사용되지 않는 속성을 `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo`, `PSSite` 개체에서 제거했습니다.