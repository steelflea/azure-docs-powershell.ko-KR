---
title: Azure PowerShell 개요 | Microsoft Docs
description: 설치 및 구성에 대한 링크를 포함한 Azure PowerShell 개요입니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 09/11/2018
ms.openlocfilehash: bdd8e69a2ea9df8b4fff100e1f3cc4c82d2d9d9d
ms.sourcegitcommit: 558436c824d9b59731aa9b963cdc8df4dea932e7
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/29/2018
ms.locfileid: "52588097"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="6954e-103">Azure PowerShell 개요</span><span class="sxs-lookup"><span data-stu-id="6954e-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="6954e-104">Azure PowerShell은 Azure 리소스를 관리하기 위해 [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) 모델을 사용하는 cmdlet 집합을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="6954e-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="6954e-105">[Azure Cloud Shell](/azure/cloud-shell/overview)과 함께 브라우저에서 사용하거나 로컬 컴퓨터에 설치하여 PowerShell 세션에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6954e-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can install it on your local machine and use it in any PowerShell session.</span></span>

<span data-ttu-id="6954e-106">[Cloud Shell](/azure/cloud-shell/overview)을 사용하여 브라우저에서 Azure PowerShell을 실행하거나 자신의 컴퓨터에 [설치](install-azurerm-ps.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="6954e-106">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the Azure PowerShell in your browser, or [install](install-azurerm-ps.md) it on own computer.</span></span> <span data-ttu-id="6954e-107">그런 다음 [시작](get-started-azureps.md) 문서를 읽고 사용을 시작해 보세요.</span><span class="sxs-lookup"><span data-stu-id="6954e-107">Then read the [Get Started](get-started-azureps.md) article to begin using it.</span></span> <span data-ttu-id="6954e-108">최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azureps.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6954e-108">For information about the latest release, see the [release notes](release-notes-azureps.md).</span></span>

<span data-ttu-id="6954e-109">다음 샘플을 통해 Azure PowerShell로 일반 시나리오를 수행하는 방법을 배울 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6954e-109">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="6954e-110">Linux Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="6954e-110">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="6954e-111">Windows Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="6954e-111">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="6954e-112">Web Apps</span><span class="sxs-lookup"><span data-stu-id="6954e-112">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="6954e-113">SQL Databases</span><span class="sxs-lookup"><span data-stu-id="6954e-113">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

[!INCLUDE[az-replacing-azurerm](../includes/az-replacing-azurerm.md)]

## <a name="learn-powershell-basics"></a><span data-ttu-id="6954e-114">PowerShell 기본 사항 알아보기</span><span class="sxs-lookup"><span data-stu-id="6954e-114">Learn PowerShell basics</span></span>

<span data-ttu-id="6954e-115">PowerShell에 대해 익숙하지 않으면 PowerShell 소개가 도움이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6954e-115">If you're unfamiliar with PowerShell, an introduction to PowerShell may be helpful.</span></span>

* [<span data-ttu-id="6954e-116">PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="6954e-116">Installing PowerShell</span></span>](/powershell/scripting/setup/installing-windows-powershell)
* [<span data-ttu-id="6954e-117">PowerShell 스크립팅</span><span class="sxs-lookup"><span data-stu-id="6954e-117">Scripting with PowerShell</span></span>](/powershell/scripting/powershell-scripting)

<span data-ttu-id="6954e-118">[PowerShell 기본 사항: (1부) PowerShell 시작](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1) 비디오를 시청할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6954e-118">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

<span data-ttu-id="6954e-119">또는 Microsoft Virtual Academy의 [PowerShell 시작](https://mva.microsoft.com/liveevents/powershell-jumpstart)에 참석합니다.</span><span class="sxs-lookup"><span data-stu-id="6954e-119">Or attend the Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart).</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="6954e-120">Microsoft Learn을 통해 기술 쌓기</span><span class="sxs-lookup"><span data-stu-id="6954e-120">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="6954e-121">PowerShell을 사용하여 스크립트로 Azure 작업 자동화</span><span class="sxs-lookup"><span data-stu-id="6954e-121">Automate Azure tasks using scripts with PowerShell</span></span>](/learn/modules/automate-azure-tasks-with-powershell/)
- [<span data-ttu-id="6954e-122">더 많은 대화형 학습 보기...</span><span class="sxs-lookup"><span data-stu-id="6954e-122">More interactive learning...</span></span>](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="6954e-123">다른 Azure PowerShell 모듈</span><span class="sxs-lookup"><span data-stu-id="6954e-123">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="6954e-124">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="6954e-124">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="6954e-125">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6954e-125">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="6954e-126">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6954e-126">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="6954e-127">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="6954e-127">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
