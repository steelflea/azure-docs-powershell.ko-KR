---
title: AzureRM에서 Az로 Azure PowerShell 스크립트 마이그레이션
description: AzureRM 모듈에서 새 Az 모듈로 스크립트를 마이그레이션하는 단계와 도구에 대해 알아보세요.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/07/2018
ms.openlocfilehash: 0c73e7ac1d47a2a97b6136fa481d0adce8de33db
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/22/2018
ms.locfileid: "52259641"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a><span data-ttu-id="4db5f-103">AzureRM에서 Azure PowerShell Az로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="4db5f-103">Migrate from AzureRM to Azure PowerShell Az</span></span>

<span data-ttu-id="4db5f-104">Az 모듈은 AzureRM과 기능 패리티를 가지고 있지만 더 짧고 일관된 cmdlet 이름을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-104">The Az module has feature parity with AzureRM, but uses shorter and more consistent cmdlet names.</span></span>
<span data-ttu-id="4db5f-105">AzureRM cmdlet용으로 작성된 스크립트는 새 모듈과 자동으로 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-105">Scripts written for the AzureRM cmdlets won't automatically work with the new module.</span></span> <span data-ttu-id="4db5f-106">쉽게 전환하기 위해 Az는 AzureRM을 사용하여 기존 스크립트를 실행할 수 있는 도구를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-106">To make the transition easier, Az offers tools to allow you to run your existing scripts using AzureRM.</span></span> <span data-ttu-id="4db5f-107">새 명령 집합으로 마이그레이션은 편리하지 않지만 이 문서는 새로운 모듈로 전환을 시작하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-107">No migration to a new command set is ever convenient, but this article will help you get started on transitioning to the new module.</span></span>

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a><span data-ttu-id="4db5f-108">기존 스크립트가 최신 AzureRM 릴리스와 함께 작동하는지 확인하세요</span><span class="sxs-lookup"><span data-stu-id="4db5f-108">Ensure your existing scripts work with the latest AzureRM release</span></span>

<span data-ttu-id="4db5f-109">가장 중요한 단계입니다!</span><span class="sxs-lookup"><span data-stu-id="4db5f-109">This is the most important step!</span></span> <span data-ttu-id="4db5f-110">기존 스크립트를 실행하고 AzureRM(__6.12.0__)의 _최신_ 릴리스와 함께 작동하는지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="4db5f-110">Run your existing scripts, and make sure that they work with the _latest_ release of AzureRM (__6.12.0__).</span></span> <span data-ttu-id="4db5f-111">스크립트가 작동하지 않으면 [AzureRM 마이그레이션 가이드](migration-guide.6.0.0.md)를 읽으세요.</span><span class="sxs-lookup"><span data-stu-id="4db5f-111">If your scripts don't work, make sure to read the [AzureRM migration guide](migration-guide.6.0.0.md).</span></span>

## <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="4db5f-112">Azure PowerShell Az 모듈 설치</span><span class="sxs-lookup"><span data-stu-id="4db5f-112">Install the Azure PowerShell Az module</span></span>

<span data-ttu-id="4db5f-113">첫 번째 단계는 플랫폼에 Az 모듈을 설치하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-113">The first step is to install the Az module on your platform.</span></span> <span data-ttu-id="4db5f-114">Az를 설치하려면 AzureRM을 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-114">To install Az, you need to uninstall AzureRM.</span></span>
<span data-ttu-id="4db5f-115">다음 단계에서는 기존 스크립트를 계속 실행하고 이전 cmdlet 이름과의 호환성을 유지하는 방법을 알아보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-115">In the following steps, you'll learn how to keep running your existing scripts and enable compatibility for old cmdlet names.</span></span>

<span data-ttu-id="4db5f-116">Azure PowerShell Az 모듈을 설치하려면 다음 단계를 수행하십시오.</span><span class="sxs-lookup"><span data-stu-id="4db5f-116">To install the Azure PowerShell Az module, follow these steps:</span></span>

* <span data-ttu-id="4db5f-117">[AzureRM 모듈을 제거합니다](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="4db5f-117">[Uninstall the AzureRM module](uninstall-azurerm-ps.md).</span></span> <span data-ttu-id="4db5f-118">가장 최신 버전뿐만 아니라 설치된 _모든_ AzureRM 버전을 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-118">Make sure that you remove _all_ installed versions of AzureRM, not just the most recent version.</span></span>
* [<span data-ttu-id="4db5f-119">Az 모듈 설치</span><span class="sxs-lookup"><span data-stu-id="4db5f-119">Install the Az module</span></span>](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-alias-mode"></a><span data-ttu-id="4db5f-120"><a name="aliases"/>AzureRM 별칭 모드 사용</span><span class="sxs-lookup"><span data-stu-id="4db5f-120"><a name="aliases"/>Enable AzureRM alias mode</span></span>

<span data-ttu-id="4db5f-121">AzureRM을 제거하고 최신 AzureRM 버전과 함께 스크립트가 작동하면 이제 Az 모듈에 대한 호환 모드를 사용할 때입니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-121">With AzureRM uninstalled and your scripts working with the latest AzureRM version, now is the time to enable the compatibility mode for the Az module.</span></span> <span data-ttu-id="4db5f-122">호환성은 다음 명령으로 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-122">Compatibility is enabled with the command:</span></span>

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="4db5f-123">별칭을 사용하면 `Az` 모듈이 설치된 이전 cmdlet 이름을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-123">Aliases enable the ability to use old cmdlet names with the `Az` module installed.</span></span> <span data-ttu-id="4db5f-124">이러한 별칭은 선택한 범위에 대한 사용자 프로필에 기록됩니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-124">These aliases are written to the user profile for the selected scope.</span></span> <span data-ttu-id="4db5f-125">사용자 프로필이 없으면 프로일 하나가 만들어집니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-125">If no user profile exists, one is created.</span></span>

> [!WARNING]
>
> <span data-ttu-id="4db5f-126">이 명령에 대해 다른 `-Scope`를 사용할 수 있지만 권장되지는 않습니다!</span><span class="sxs-lookup"><span data-stu-id="4db5f-126">You can use a different `-Scope` for this command, but it's not recommended!</span></span> <span data-ttu-id="4db5f-127">별칭은 선택된 범위에 대한 사용자 프로필에 기록되므로 가능한 한 범위를 제한적으로 유지합니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-127">Aliases are written to the user profile for the selected scope, so keep enabling them to as limited a scope as possible.</span></span> <span data-ttu-id="4db5f-128">별칭을 시스템 전체에서 사용하도록 설정하면 `AzureRM`을 로컬 범위에 설치한 다른 사용자에게 문제가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-128">Enabling aliases system-wide could also cause issues for other users which have `AzureRM` installed in their local scope.</span></span>

<span data-ttu-id="4db5f-129">별칭 모드가 활성화되면 스크립트를 다시 실행하여 스크립트가 여전히 예상대로 작동하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-129">Once the alias mode is enabled, run your scripts again to confirm that they still function as expected.</span></span> 

## <a name="change-module-imports-and-cmdlet-names"></a><span data-ttu-id="4db5f-130">모듈 가져오기 및 cmdlet 이름 변경</span><span class="sxs-lookup"><span data-stu-id="4db5f-130">Change module imports and cmdlet names</span></span>

<span data-ttu-id="4db5f-131">일반적으로 모듈 이름은 `AzureRM` 및 `Azure`가 `Az`가 되도록 변경되었으며 cmdlet에도 동일하게 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-131">In general, the module names have been changed so that `AzureRM` and `Azure` become `Az`, and the same for cmdlets.</span></span>
<span data-ttu-id="4db5f-132">예를 들어, `AzureRM.Compute` 모듈의 이름이 `Az.Compute`로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-132">For example, the `AzureRM.Compute` module has been renamed to `Az.Compute`.</span></span> <span data-ttu-id="4db5f-133">`New-AzureRmVM`은 `New-AzVM`이 되고 `Get-AzureStorageBlob`은 이제 `Get-AzStorageBlob`입니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-133">`New-AzureRmVM` has become `New-AzVM`, and `Get-AzureStorageBlob` is now `Get-AzStorageBlob`.</span></span>

<span data-ttu-id="4db5f-134">이 이름 변경에는 예외가 있으며 이름을 바꾸기 전에 알아야 할 사항이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-134">There are exceptions to this naming change that you should be aware of before doing any renaming:</span></span>

| <span data-ttu-id="4db5f-135">AzureRM 모듈</span><span class="sxs-lookup"><span data-stu-id="4db5f-135">AzureRM module</span></span> | <span data-ttu-id="4db5f-136">Az 모듈</span><span class="sxs-lookup"><span data-stu-id="4db5f-136">Az module</span></span> |
|----------------|-----------|
| <span data-ttu-id="4db5f-137">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="4db5f-137">AzureRM.DataFactories</span></span> | <span data-ttu-id="4db5f-138">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="4db5f-138">Az.DataFactory</span></span> |
| <span data-ttu-id="4db5f-139">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="4db5f-139">AzureRM.DataFactoryV2</span></span> | <span data-ttu-id="4db5f-140">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="4db5f-140">Az.DataFactory</span></span> |
| <span data-ttu-id="4db5f-141">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="4db5f-141">AzureRM.RecoveryServices.Backup</span></span> | <span data-ttu-id="4db5f-142">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4db5f-142">Az.RecoveryServices</span></span> |
| <span data-ttu-id="4db5f-143">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="4db5f-143">AzureRM.RecoveryServices.SiteRecovery</span></span> | <span data-ttu-id="4db5f-144">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4db5f-144">Az.RecoveryServices</span></span> |

## <a name="summary"></a><span data-ttu-id="4db5f-145">요약</span><span class="sxs-lookup"><span data-stu-id="4db5f-145">Summary</span></span>

<span data-ttu-id="4db5f-146">이 단계를 따르면 기존 스크립트를 모두 업데이트하여 새 모듈을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4db5f-146">By following these steps, you can update all of your existing scripts to use the new module.</span></span> <span data-ttu-id="4db5f-147">마이그레이션을 어렵게 하는 이들 단계에 대해 질문이나 문제가 있는 경우 지침을 개선할 수 있도록 이 문서에 의견을 남겨주세요.</span><span class="sxs-lookup"><span data-stu-id="4db5f-147">If you have any questions or problems with these steps that made your migration difficult, please comment on this article so that we can improve the instructions.</span></span>