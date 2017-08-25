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
ms.openlocfilehash: 2a03697e0f3e80d63c48f2dc5615f6c99b9ef716
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/29/2017
---
# <a name="azure-stack-powershell"></a><span data-ttu-id="d69e8-103">Azure Stack PowerShell</span><span class="sxs-lookup"><span data-stu-id="d69e8-103">Azure Stack PowerShell</span></span> 

<span data-ttu-id="d69e8-104">Azure Stack에는 다음 두 가지 PowerShell 모듈이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="d69e8-104">Azure Stack requires the following two PowerShell modules:</span></span>  

1. <span data-ttu-id="d69e8-105">Azure Stack 호환 **AzureRM** 모듈 - **2017-03-09-profile** API 버전 프로필을 설치하여 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d69e8-105">The Azure Stack compatible **AzureRM** module which is available by installing the **2017-03-09-profile** API Version Profile.</span></span> <span data-ttu-id="d69e8-106">이 프로필을 사용하여 설치한 cmdlet은 Azure Stack 클라우드 관리자와 테넌트가 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d69e8-106">The cmdlets installed by using this profile can be used by the Azure Stack cloud administrators and the tenants.</span></span> <span data-ttu-id="d69e8-107">이 프로필에서 사용할 수 있는 PowerShell cmdlet에 대한 자세한 내용은 [AzureRM 1.2.9 버전](https://docs.microsoft.com/en-us/powershell/azure/overview?view=azurermps-1.2.9) 모듈에 대한 PowerShell 참조 콘텐츠를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d69e8-107">To learn about the PowerShell cmdlets that are available in this profile, see the PowerShell reference content for the [1.2.9 version of AzureRM](https://docs.microsoft.com/en-us/powershell/azure/overview?view=azurermps-1.2.9) module.</span></span>  

2. <span data-ttu-id="d69e8-108">**AzureStack** 모듈 **1.2.9** 버전 -</span><span class="sxs-lookup"><span data-stu-id="d69e8-108">The **1.2.9** version of the **AzureStack** module.</span></span> <span data-ttu-id="d69e8-109">이 모듈을 사용하여 설치한 cmdlet은 Azure Stack 클라우드 관리자만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d69e8-109">The cmdlets installed by using this module can be used by Azure Stack cloud administrators only.</span></span> <span data-ttu-id="d69e8-110">관리자는 이 모듈에서 제공하는 PowerShell cmdlet을 사용하여 제안, 계획, 서비스, 할당량 등의 관리 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d69e8-110">Administrator can perform operations such as manage offers, plans, services, quotas, etc. by using the PowerShell cmdlets provided by this module.</span></span> <span data-ttu-id="d69e8-111">이 모듈에서 사용할 수 있는 PowerShell cmdlet에 대한 자세한 내용은 [AzureStackAdmin](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.9#azurerm.azurestackadmin) 및 [AzureStackStorage](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.9#azurerm.azurestackstorage) 참조 콘텐츠를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d69e8-111">To learn about the PowerShell cmdlets available in this module, see the [AzureStackAdmin](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.9#azurerm.azurestackadmin) and [AzureStackStorage](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.9#azurerm.azurestackstorage) Reference content.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d69e8-112">다음 단계</span><span class="sxs-lookup"><span data-stu-id="d69e8-112">Next Steps</span></span>

* [<span data-ttu-id="d69e8-113">Azure Stack용 PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="d69e8-113">Install PowerShell for Azure Stack</span></span>](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [<span data-ttu-id="d69e8-114">Azure Stack과 함께 사용하도록 PowerShell 구성</span><span class="sxs-lookup"><span data-stu-id="d69e8-114">Configure PowerShell for use with Azure Stack</span></span>](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)


