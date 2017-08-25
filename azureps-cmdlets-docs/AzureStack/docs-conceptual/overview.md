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
# <a name="azure-stack-powershell"></a>Azure Stack PowerShell 

Azure Stack에는 다음 두 가지 PowerShell 모듈이 필요합니다.  

1. Azure Stack 호환 **AzureRM** 모듈 - **2017-03-09-profile** API 버전 프로필을 설치하여 사용할 수 있습니다. 이 프로필을 사용하여 설치한 cmdlet은 Azure Stack 클라우드 관리자와 테넌트가 사용할 수 있습니다. 이 프로필에서 사용할 수 있는 PowerShell cmdlet에 대한 자세한 내용은 [AzureRM 1.2.9 버전](https://docs.microsoft.com/en-us/powershell/azure/overview?view=azurermps-1.2.9) 모듈에 대한 PowerShell 참조 콘텐츠를 참조하세요.  

2. **AzureStack** 모듈 **1.2.9** 버전 - 이 모듈을 사용하여 설치한 cmdlet은 Azure Stack 클라우드 관리자만 사용할 수 있습니다. 관리자는 이 모듈에서 제공하는 PowerShell cmdlet을 사용하여 제안, 계획, 서비스, 할당량 등의 관리 작업을 수행할 수 있습니다. 이 모듈에서 사용할 수 있는 PowerShell cmdlet에 대한 자세한 내용은 [AzureStackAdmin](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.9#azurerm.azurestackadmin) 및 [AzureStackStorage](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.9#azurerm.azurestackstorage) 참조 콘텐츠를 참조하세요.

## <a name="next-steps"></a>다음 단계

* [Azure Stack용 PowerShell 설치](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [Azure Stack과 함께 사용하도록 PowerShell 구성](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)


