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
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/15/2018
ms.locfileid: "51575929"
---
# <a name="log-in-with-azure-powershell"></a><span data-ttu-id="c0a42-103">Azure PowerShell을 사용하여 로그인</span><span class="sxs-lookup"><span data-stu-id="c0a42-103">Log in with Azure PowerShell</span></span>

<span data-ttu-id="c0a42-104">Azure PowerShell에서는 여러 로그인 방법을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-104">Azure PowerShell supports multiple login methods.</span></span> <span data-ttu-id="c0a42-105">가장 간단하게 시작하는 방법은 명령줄에서 대화형으로 로그인하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-105">The simplest way to get started is to log in interactively at the command line.</span></span>

## <a name="interactive-log-in"></a><span data-ttu-id="c0a42-106">대화형 로그인</span><span class="sxs-lookup"><span data-stu-id="c0a42-106">Interactive log in</span></span>

1. <span data-ttu-id="c0a42-107">`Login-AzureRmAccount`을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-107">Type `Login-AzureRmAccount`.</span></span> <span data-ttu-id="c0a42-108">Azure 자격 증명을 묻는 대화 상자가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-108">You will get dialog box asking for your Azure credentials.</span></span>

2. <span data-ttu-id="c0a42-109">계정과 연결된 메일 주소 및 암호를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-109">Type the email address and password associated with your account.</span></span> <span data-ttu-id="c0a42-110">Azure가 자격 증명 정보를 인증 및 저장한 후 창을 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-110">Azure authenticates and saves the credential information, and then closes the window.</span></span>

## <a name="log-in-with-a-service-principal"></a><span data-ttu-id="c0a42-111">서비스 주체를 사용하여 로그인</span><span class="sxs-lookup"><span data-stu-id="c0a42-111">Log in with a service principal</span></span>

<span data-ttu-id="c0a42-112">서비스 주체는 리소스를 조작하는 데 사용할 수 있는 비 대화형 계정을 만드는 방법을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-112">Service principals provide a way for you to create non-interactive accounts that you can use to manipulate resources.</span></span> <span data-ttu-id="c0a42-113">서비스 주체는 Azure Active Directory를 사용하여 규칙을 적용할 수 있는 사용자 계정과 비슷합니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-113">Service principals are like user accounts to which you can apply rules using Azure Active Directory.</span></span> <span data-ttu-id="c0a42-114">서비스 주체에게 필요한 최소 사용 권한만 부여하여 자동화 스크립트를 훨씬 안전하게 보호할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-114">By granting the minimum permissions needed to a service principal, you can ensure your automation scripts are even more secure.</span></span>

1. <span data-ttu-id="c0a42-115">아직 서비스 주체가 없는 경우 [하나 만듭니다](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="c0a42-115">If you don't already have a service principal, [create one](create-azure-service-principal-azureps.md).</span></span>

2. <span data-ttu-id="c0a42-116">서비스 주체를 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-116">Log in with the service principal.</span></span>

    ```powershell-interactive
    Login-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
    ```

    <span data-ttu-id="c0a42-117">TenantId를 가져오려면 대화형으로 로그인한다음 구독에서 TenantId를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-117">To get your TenantId, log in interactively and then get the TenantId from your subscription.</span></span>

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

### <a name="log-in-using-managed-identities-for-azure-resources"></a><span data-ttu-id="c0a42-118">Azure 리소스에 대한 관리 ID를 사용하여 로그인</span><span class="sxs-lookup"><span data-stu-id="c0a42-118">Log in using managed identities for Azure resources</span></span>

<span data-ttu-id="c0a42-119">Azure 리소스에 대한 관리 ID는 Azure Active Directory의 기능입니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-119">Managed identities for Azure resources is a feature of Azure Active Directory.</span></span> <span data-ttu-id="c0a42-120">로그인에 관리 ID 서비스 주체를 사용할 수 있으며, 다른 리소스에 액세스하려면 앱 전용 액세스 토큰이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-120">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span>

<span data-ttu-id="c0a42-121">Azure 리소스의 관리 ID에 대한 자세한 내용은 [Azure VM에서 Azure 리소스에 대한 관리 ID를 사용하여 액세스 토큰을 획득하는 방법](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c0a42-121">For more information about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="log-in-to-another-cloud"></a><span data-ttu-id="c0a42-122">다른 클라우드로 로그인</span><span class="sxs-lookup"><span data-stu-id="c0a42-122">Log in to another Cloud</span></span>

<span data-ttu-id="c0a42-123">Azure Cloud Services는 다양한 정부의 데이터 처리 규정에 부합되는 여러 다른 환경을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-123">Azure cloud services provide different environments that adhere to the data-handling regulations of various governments.</span></span> <span data-ttu-id="c0a42-124">Azure 계정에 있으면 하나는 정부 클라우드에 속할 경우 로그인 시 해당 환경을 지정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-124">If your Azure account is in one the government clouds, you need to specify the environment when you sign in.</span></span> <span data-ttu-id="c0a42-125">예를 들어 계정이 중국 클라우드에 있으면 다음 명령을 사용하여 로그온합니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-125">For example, if you account is in the China cloud you sign on using the following command:</span></span>

```powershell-interactive
Login-AzureRmAccount -EnvironmentName AzureChinaCloud
```

<span data-ttu-id="c0a42-126">사용 가능한 환경 목록을 가져오려면 다음 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="c0a42-126">Use the following command to get a list of available environments:</span></span>

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

## <a name="learn-more-about-managing-azure-role-based-access"></a><span data-ttu-id="c0a42-127">Azure 역할 기반 액세스를 관리하는 방법에 대해 알아보기</span><span class="sxs-lookup"><span data-stu-id="c0a42-127">Learn more about managing Azure role-based access</span></span>

<span data-ttu-id="c0a42-128">Azure에서 인증 및 구독 관리에 대한 자세한 내용은 [계정, 구독 및 관리 역할 관리](/azure/active-directory/role-based-access-control-configure)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c0a42-128">For more information about authentication and subscription management in Azure, see [Manage Accounts, Subscriptions, and Administrative Roles](/azure/active-directory/role-based-access-control-configure).</span></span>

<span data-ttu-id="c0a42-129">역할 관리를 위한 Azure PowerShell cmdlet</span><span class="sxs-lookup"><span data-stu-id="c0a42-129">Azure PowerShell cmdlets for role management</span></span>

* [<span data-ttu-id="c0a42-130">Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c0a42-130">Get-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [<span data-ttu-id="c0a42-131">Get-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0a42-131">Get-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [<span data-ttu-id="c0a42-132">New-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c0a42-132">New-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [<span data-ttu-id="c0a42-133">New-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0a42-133">New-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [<span data-ttu-id="c0a42-134">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c0a42-134">Remove-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [<span data-ttu-id="c0a42-135">Remove-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0a42-135">Remove-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [<span data-ttu-id="c0a42-136">Set-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0a42-136">Set-AzureRmRoleDefinition</span></span>](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)
