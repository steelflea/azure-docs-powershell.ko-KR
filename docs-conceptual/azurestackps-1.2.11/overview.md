---
title: "Azure Stack PowerShell 개요 | Microsoft Docs"
description: "Azure Stack PowerShell 설치 및 구성에 대해 간략히 설명합니다."
author: SnehaGunda
manager: Byronr
ms.product: azure-stack
ms.service: powershell
ms.devlang: powershell
ms.topic: reference
ms.author: sngun
ms.manager: byronr
ms.openlocfilehash: f895992b4200f260189b3dbc541452e73a377b00
ms.sourcegitcommit: 8446ae373ac6928871ec8f10d3a4918b4601d5b2
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/27/2018
---
# <a name="azure-stack-powershell"></a><span data-ttu-id="e6ca6-103">Azure Stack PowerShell</span><span class="sxs-lookup"><span data-stu-id="e6ca6-103">Azure Stack PowerShell</span></span>

<span data-ttu-id="e6ca6-104">Azure Stack에는 다음 두 가지 PowerShell 모듈이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="e6ca6-104">Azure Stack requires the following two PowerShell modules:</span></span>  

1. <span data-ttu-id="e6ca6-105">Azure Stack 호환 **AzureRM** 모듈 - **2017-03-09-profile** API 버전 프로필을 설치하여 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e6ca6-105">The Azure Stack compatible **AzureRM** module which is available by installing the **2017-03-09-profile** API Version Profile.</span></span> <span data-ttu-id="e6ca6-106">이 프로필을 사용하여 설치한 cmdlet은 Azure Stack 연산자 및 사용자가 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e6ca6-106">The cmdlets installed by using this profile can be used by Azure Stack operators and users.</span></span>

2. <span data-ttu-id="e6ca6-107">현재 버전은 **AzureStack** 모듈의 **1.2.11** 설치입니다.</span><span class="sxs-lookup"><span data-stu-id="e6ca6-107">The most current version is the **1.2.11** install of the **AzureStack** module.</span></span> <span data-ttu-id="e6ca6-108">이 모듈을 사용하여 설치한 cmdlet은 Azure Stack 연산자만이 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e6ca6-108">The cmdlets installed by using this module can be used by Azure Stack operators only.</span></span> <span data-ttu-id="e6ca6-109">연산자는 이 모듈에서 제공하는 PowerShell cmdlet을 사용하여 제안, 계획, 서비스, 할당량 등의 관리 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e6ca6-109">Operators can perform operations such as manage offers, plans, services, quotas, etc. by using the PowerShell cmdlets provided by this module.</span></span> <span data-ttu-id="e6ca6-110">이 모듈에서 사용할 수 있는 PowerShell cmdlet에 대한 자세한 내용은 [AzureStackAdmin](https://docs.microsoft.com/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.11#azurerm.azurestackadmin) 및 [AzureStackStorage](https://docs.microsoft.com/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.11#azurerm.azurestackstorage) 참조 콘텐츠를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e6ca6-110">To learn about the PowerShell cmdlets available in this module, see the [AzureStackAdmin](https://docs.microsoft.com/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.11#azurerm.azurestackadmin) and [AzureStackStorage](https://docs.microsoft.com/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.11#azurerm.azurestackstorage) Reference content.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e6ca6-111">다음 단계</span><span class="sxs-lookup"><span data-stu-id="e6ca6-111">Next Steps</span></span>

* [<span data-ttu-id="e6ca6-112">Azure Stack용 PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="e6ca6-112">Install PowerShell for Azure Stack</span></span>](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [<span data-ttu-id="e6ca6-113">Azure Stack과 함께 사용하도록 PowerShell 구성</span><span class="sxs-lookup"><span data-stu-id="e6ca6-113">Configure PowerShell for use with Azure Stack</span></span>](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
