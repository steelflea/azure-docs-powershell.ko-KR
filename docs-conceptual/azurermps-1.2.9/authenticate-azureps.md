---
title: Azure PowerShell을 사용하여 로그인
description: Azure PowerShell을 사용하여 로그인
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: edbf17141cac4ea6e41282c8e1dd07c5b738351c
ms.sourcegitcommit: ac4b53bb42a25aae013a9d8cd9ae98ada9397274
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/08/2018
ms.locfileid: "51274707"
---
# <a name="log-in-with-azure-powershell"></a>Azure PowerShell을 사용하여 로그인

Azure PowerShell에서는 여러 로그인 방법을 지원합니다. 가장 간단하게 시작하는 방법은 명령줄에서 대화형으로 로그인하는 것입니다.

## <a name="interactive-log-in"></a>대화형 로그인

1. `Login-AzureRmAccount`을 입력합니다. Azure 자격 증명을 묻는 대화 상자가 표시됩니다.

2. 계정과 연결된 메일 주소 및 암호를 입력합니다. Azure가 자격 증명 정보를 인증 및 저장한 후 창을 닫습니다.

## <a name="log-in-with-a-service-principal"></a>서비스 주체를 사용하여 로그인

서비스 주체는 리소스를 조작하는 데 사용할 수 있는 비 대화형 계정을 만드는 방법을 제공합니다. 서비스 주체는 Azure Active Directory를 사용하여 규칙을 적용할 수 있는 사용자 계정과 비슷합니다. 서비스 주체에게 필요한 최소 사용 권한만 부여하여 자동화 스크립트를 훨씬 안전하게 보호할 수 있습니다.

1. 아직 서비스 주체가 없는 경우 [하나 만듭니다](create-azure-service-principal-azureps.md).

2. 서비스 주체를 사용하여 로그인합니다.

    ```powershell-interactive
    Login-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
    ```

    TenantId를 가져오려면 대화형으로 로그인한다음 구독에서 TenantId를 가져옵니다.

    ```powershell-interactive
    Get-AzureRmSubscription
    ```

    ```output
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Production Subscription
    CurrentStorageAccount :
    ```

### <a name="log-in-using-managed-identities-for-azure-resources"></a>Azure 리소스에 대한 관리 ID를 사용하여 로그인

Azure 리소스에 대한 관리 ID는 Azure Active Directory의 기능입니다. 로그인에 관리 ID 서비스 주체를 사용할 수 있으며, 다른 리소스에 액세스하려면 앱 전용 액세스 토큰이 필요합니다.

Azure 리소스의 관리 ID에 대한 자세한 내용은 [Azure VM에서 Azure 리소스에 대한 관리 ID를 사용하여 액세스 토큰을 획득하는 방법](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token)을 참조하세요.

## <a name="log-in-to-another-cloud"></a>다른 클라우드로 로그인

Azure Cloud Services는 다양한 정부의 데이터 처리 규정에 부합되는 여러 다른 환경을 제공합니다. Azure 계정에 있으면 하나는 정부 클라우드에 속할 경우 로그인 시 해당 환경을 지정해야 합니다. 예를 들어 계정이 중국 클라우드에 있으면 다음 명령을 사용하여 로그온합니다.

```powershell-interactive
Login-AzureRmAccount -EnvironmentName AzureChinaCloud
```

사용 가능한 환경 목록을 가져오려면 다음 명령을 사용합니다.

```powershell-interactive
Get-AzureRmEnvironment | Select-Object Name
```

```output
Name
----
AzureCloud
AzureChinaCloud
AzureUSGovernment
AzureGermanCloud
```

## <a name="learn-more-about-managing-azure-role-based-access"></a>Azure 역할 기반 액세스를 관리하는 방법에 대해 알아보기

Azure에서 인증 및 구독 관리에 대한 자세한 내용은 [계정, 구독 및 관리 역할 관리](/azure/active-directory/role-based-access-control-configure)를 참조하세요.

역할 관리를 위한 Azure PowerShell cmdlet

* [Get-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [Get-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [New-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [New-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [Remove-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [Remove-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [Set-AzureRmRoleDefinition](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)
