---
title: Azure PowerShell Az 모듈 소개
description: AzureRM 모듈을 대체하는 새로운 Azure PowerShell 모듈 Az을 소개합니다.
ms.date: 11/07/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: b0f31341d4344bdac5b4d657a1f66acfd9984dda
ms.sourcegitcommit: 558436c824d9b59731aa9b963cdc8df4dea932e7
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/29/2018
ms.locfileid: "52587315"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a><span data-ttu-id="ae695-103">새로운 Azure PowerShell Az 모듈 소개</span><span class="sxs-lookup"><span data-stu-id="ae695-103">Introducing the new Azure PowerShell Az module</span></span>

<span data-ttu-id="ae695-104">2018년 11월부터 Azure PowerShell `Az` 모듈을 전체 공개 미리보기로 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-104">Starting in November 2018, the Azure PowerShell `Az` module is available for full public preview.</span></span>
<span data-ttu-id="ae695-105">Az은 짧아진 명령과 향상된 안정성을 제공하며, Windows, macOS 및 Linux를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-105">Az offers shorter commands, improved stability, and supports Windows, macOS, and Linux.</span></span> <span data-ttu-id="ae695-106">Az은 또한 AzureRM에서 기능 패리티와 쉬운 마이그레이션 경로를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-106">Az also offers feature parity and an easy migration path from AzureRM.</span></span>

<span data-ttu-id="ae695-107">Az는 .NET 표준 라이브러리를 사용합니다. 즉, PowerShell 5.x 및 PowerShell 6.x에서 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-107">Az uses the .NET Standard library, which means it runs on PowerShell 5.x and PowerShell 6.x.</span></span>
<span data-ttu-id="ae695-108">PowerShell 6.x는 Linux, macOS 및 Windows에서 실행할 수 있으므로, Az는 모든 플랫폼에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-108">Since PowerShell 6.x can run on Linux, macOS, and Windows, that means Az is available for all platforms.</span></span>
<span data-ttu-id="ae695-109">.NET 표준을 사용하면 사용자에게 미치는 영향을 최소화하면서 Azure PowerShell의 코드 기반을 통합할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-109">Using .NET Standard allows us to unify the code base of Azure PowerShell with minimal impact on users.</span></span>

<span data-ttu-id="ae695-110">Az는 새로운 모듈이므로 버전이 다시 설정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-110">Az is a new module, so the version has been reset.</span></span> <span data-ttu-id="ae695-111">첫 번째 안정적인 릴리스는 1.0이지만, 모듈은 2018년 11월 현재 AzureRm과 기능 패리티를 유지합니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-111">The first stable release will be 1.0, but the module has feature parity with AzureRm as of November 2018.</span></span>

## <a name="upgrade-to-az"></a><span data-ttu-id="ae695-112">Az로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="ae695-112">Upgrade to Az</span></span>

<span data-ttu-id="ae695-113">사용자가 새로운 `Az` 모듈로 업그레이드하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-113">It's recommended that users upgrade to the new `Az` module.</span></span> <span data-ttu-id="ae695-114">이렇게 하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-114">To do so:</span></span>

* [<span data-ttu-id="ae695-115">Azure PowerShell AzureRM 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="ae695-115">Uninstall the Azure PowerShell AzureRM module</span></span>](/powershell/azure/uninstall-azurerm-ps)
* [<span data-ttu-id="ae695-116">Azure PowerShell Az 모듈 설치</span><span class="sxs-lookup"><span data-stu-id="ae695-116">Install the Azure PowerShell Az module</span></span>](/powershell/azure/install-az-ps)
* <span data-ttu-id="ae695-117">새 명령 집합에 익숙해지면서 `Enable-AzureRMAlias`로 AzureRM의 호환 모드를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-117">Enable compatibility mode for AzureRM with `Enable-AzureRMAlias` while you become familiar with the new command set.</span></span>

## <a name="migrate-existing-scripts-to-az"></a><span data-ttu-id="ae695-118">기존 스크립트를 Az로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="ae695-118">Migrate existing scripts to Az</span></span>

<span data-ttu-id="ae695-119">주요 업데이트가 불편할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-119">Major updates can be inconvenient.</span></span> <span data-ttu-id="ae695-120">그러나 `Az` 모듈에는 새로운 구문에 대한 업데이트 작업을 하는 동안 기존 스크립트를 사용할 수 있도록 해주는 호환 모드가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-120">However, the `Az` module has a compatibility mode to help you use existing scripts while you work on updates to the new syntax.</span></span> <span data-ttu-id="ae695-121">`Enable-AzureRmAlias` cmdlet을 사용하여 `AzureRM` 호환 모드를 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-121">Use the `Enable-AzureRmAlias` cmdlet to enable the `AzureRM` compatibility mode.</span></span> <span data-ttu-id="ae695-122">이 cmdlet은 `AzureRM` cmdlet 이름을 새 `Az` cmdlet 이름의 별칭으로 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-122">This cmdlet defines `AzureRM` cmdlet names as aliases for the new `Az` cmdlet names.</span></span>

<span data-ttu-id="ae695-123">새로운 cmdlet 이름은 쉽게 익힐 수 있도록 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-123">The new cmdlet names have been designed to be easy to learn.</span></span> <span data-ttu-id="ae695-124">cmdlet 이름에 `AzureRm` 또는 `Azure`를 사용하는 대신 `Az`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-124">Instead of using `AzureRm` or `Azure` in cmdlet names, use `Az`.</span></span> <span data-ttu-id="ae695-125">예를 들어, 이전 명령 `New-AzureRmVm`은 `New-AzVm`이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-125">For example, the old command `New-AzureRmVm` has become `New-AzVm`.</span></span>

<span data-ttu-id="ae695-126">마이그레이션 프로세스에 대한 전체 설명은 [AzureRM에서 Az로 마이그레이션](migrate-from-azurerm-to-az.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ae695-126">For a full description of the migration process, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

## <a name="the-future-of-support-for-azurerm"></a><span data-ttu-id="ae695-127">AzureRM에 대한 향후 지원</span><span class="sxs-lookup"><span data-stu-id="ae695-127">The future of support for AzureRM</span></span>

<span data-ttu-id="ae695-128">2018년 12월에 `Az` 버전 1.0이 릴리스되면 기존 `AzureRM` 모듈은 더 이상 새로운 cmdlet 또는 기능을 받지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-128">The existing `AzureRM` module will no longer receive new cmdlets or features when `Az` version 1.0 is released in December 2018.</span></span> <span data-ttu-id="ae695-129">그러나 `AzureRM`은 공식적으로 유지되며 버그 수정도 이루어집니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-129">However, `AzureRM` is still officially maintained and will get bug fixes.</span></span> <span data-ttu-id="ae695-130">최신 Azure 서비스 및 기능을 유지하기 위해서는 `Az` 모듈로 전환해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ae695-130">To keep up with the latest Azure services and features, you should switch to the `Az` module.</span></span>