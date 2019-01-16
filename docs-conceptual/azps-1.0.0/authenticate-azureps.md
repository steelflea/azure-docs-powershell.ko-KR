---
title: Azure PowerShell로 로그인
description: Azure PowerShell 사용자나 서비스 주체로 로그인 또는 Azure 리소스에 대한 관리 ID로 로그인하는 방법.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: 80c59a10666c6e3a01e6c33716fce40094fb14be
ms.sourcegitcommit: b5635e291cdc324e66c936aa16c5772507fc78e8
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/04/2019
ms.locfileid: "54055679"
---
# <a name="sign-in-with-azure-powershell"></a>Azure PowerShell로 로그인

Azure PowerShell에서는 여러 인증 방법을 지원합니다. 시작하는 가장 쉬운 방법은 [Azure Cloud Shell](/azure/cloud-shell/overview)을 사용하는 것으로서, 자동으로 로그인합니다. 로컬 설치에서는, 브라우저를 통해 대화형으로 로그인할 수 있습니다. 자동화 스크립트를 작성할 때 권장되는 방법은 필요한 권한이 있는 [서비스 주체](create-azure-service-principal-azureps.md)를 사용하는 것입니다. 사용 사례에 대해 로그인 권한을 가능한 한 많이 제한하면 Azure 리소스를 안전하게 유지할 수 있습니다.

로그인한 후 명령은 기본 구독에 대해 실행됩니다. 세션에 대한 활성 구독을 변경하려면 [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet을 사용합니다. Azure PowerShell로 로그인할 때 사용되는 기본 구독을 변경하려면 [Set-AzDefault](/powershell/module/az.accounts/set-azdefault)를 사용합니다.

> [!IMPORTANT]
>
> 로그인한 상태를 유지하는 한, 여러 PowerShell 세션에서 자격 증명을 공유할 수 있습니다.
> 자세한 내용은 [영구 자격 증명](context-persistence.md)에 대한 아티클을 참조합니다.

## <a name="sign-in-interactively"></a>대화형으로 로그인

대화형으로 로그인하려면 [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet을 사용합니다.

```azurepowershell-interactive
Connect-AzAccount
```

실행되면 이 cmdlet은 토큰 문자열을 제공합니다. 로그인 하려면 이 문자열을 복사하여 브라우저에서 https://microsoft.com/devicelogin에 붙여 넣습니다. 그러면 PowerShell 세션이 인증되어 Azure에 연결됩니다.

## <a name="sign-in-with-credentials"></a>자격 증명으로 로그인

Azure에 연결할 권한이 있는 `PSCredential` 개체로 로그인할 수도 있습니다.
자격 증명 개체를 가져오는 가장 쉬운 방법은 [Get-credential](/powershell/module/Microsoft.PowerShell.Security/Get-Credential) cmdlet입니다. 이 cmdlet을 실행하면 사용자 이름/암호 자격 증명 쌍을 묻는 메시지가 표시됩니다.

> [!Note]
> 이 접근 방식은 Microsoft 계정 또는 2단계 인증을 사용하는 계정에서는 작동하지 않습니다.

```azurepowershell-interactive
$creds = Get-Credential
Connect-AzAccount -Credential $creds
```

## <a name="sign-in-with-a-service-principal"></a>서비스 주체를 사용하여 로그인

서비스 주체는 비대화형 Azure 계정입니다. 다른 사용자 계정과 마찬가지로 해당 권한은 Azure Active Directory를 사용하여 관리됩니다. 서비스 주체에 필요한 권한만 부여하여 자동화 스크립트 보안을 유지할 수 있습니다.

Azure PowerShell에 사용할 서비스 주체를 생성하는 방법을 보려면 [Azure PowerShell을 사용하여 Azure 서비스 주체 만들기](create-azure-service-principal-azureps.md)를 참조하세요.

서비스 주체로 로그인하려면 `Connect-AzAccount` cmdlet `-ServicePrincipal`인수를 사용합니다. 또한 서비스 주체의 애플리케이션 ID, 로그인 자격 증명 및 서비스 주체와 연결된 테넌트 ID가 필요합니다. 서비스 주체의 자격 증명을 적절한 개체로 가져오려면 [Get-credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet을 사용합니다. 이 cmdlet은 서비스 주체 사용자 ID와 암호에 대한 메시지를 표시합니다.

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-a-managed-identity"></a>관리 ID를 사용하여 로그인 

관리 ID는 Azure Active Directory의 기능입니다. 관리 ID는 Azure에서 실행되는 리소스에 할당된 서비스 주체입니다. 로그인에 관리 ID 서비스 주체를 사용할 수 있으며, 다른 리소스에 액세스하려면 앱 전용 액세스 토큰이 필요합니다. 관리 ID는 Azure 클라우드에서 실행되는 리소스에서만 사용할 수 있습니다.

Azure 리소스의 관리 ID에 대한 자세한 내용은 [Azure VM에서 Azure 리소스에 대한 관리 ID를 사용하여 액세스 토큰을 획득하는 방법](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token)을 참조하세요.

## <a name="sign-in-with-a-non-default-tenant-or-as-a-cloud-solution-provider-csp"></a>기본이 아닌 테넌트를 사용하여 로그인하거나 클라우드 솔루션 공급자(CSP)로 로그인

계정이 둘 이상의 테넌트와 연결되어 있는 경우 로그인은 연결 시 `-TenantId` 매개 변수를 사용해야 합니다. 이 매개 변수는 다른 로그인 메서드를 사용하여 작동 합니다. 로그인할 때 이 매개 변수 값은 테넌트의 Azure 개체 ID(테넌트 ID) 또는 테넌트의 정규화된 도메인 이름이 될 수 있습니다.

[클라우드 솔루션 공급자(CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/)의 경우 `-TenantId` 값은 **반드시** 테넌트 ID여야 합니다.

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a>다른 클라우드로 로그인

Azure 클라우드 서비스는 지역 데이터 처리법을 준수하는 환경을 제공합니다.
지역별 클라우드의 계정에 대해 로그인할 때 `-Environment` 인수를 사용해서 환경을 설정합니다.
예를 들어 계정이 중국 클라우드에 있는 경우:

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

다음 명령은 사용 가능한 환경 목록을 가져옵니다.

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```