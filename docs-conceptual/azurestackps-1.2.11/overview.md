---
title: Azure Stack PowerShell 개요 | Microsoft Docs
description: Azure Stack PowerShell 설치 및 구성에 대해 간략히 설명합니다.
author: SnehaGunda
manager: Byronr
ms.product: azure-stack
ms.devlang: powershell
ms.topic: reference
ms.author: sngun
ms.manager: byronr
ms.openlocfilehash: 3f55ff613004f0726e20255126b29bf7f64662b8
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/06/2018
ms.locfileid: "34820204"
---
# <a name="azure-stack-powershell"></a>Azure Stack PowerShell

Azure Stack에는 다음 두 가지 PowerShell 모듈이 필요합니다.  

1. Azure Stack 호환 **AzureRM** 모듈 - **2017-03-09-profile** API 버전 프로필을 설치하여 사용할 수 있습니다. 이 프로필을 사용하여 설치한 cmdlet은 Azure Stack 연산자 및 사용자가 사용할 수 있습니다.

2. 현재 버전은 **AzureStack** 모듈의 **1.2.11** 설치입니다. 이 모듈을 사용하여 설치한 cmdlet은 Azure Stack 연산자만이 사용할 수 있습니다. 연산자는 이 모듈에서 제공하는 PowerShell cmdlet을 사용하여 제안, 계획, 서비스, 할당량 등의 관리 작업을 수행할 수 있습니다. 이 모듈에서 사용할 수 있는 PowerShell cmdlet에 대한 자세한 내용은 [AzureStackAdmin](https://docs.microsoft.com/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.11#azurerm.azurestackadmin) 및 [AzureStackStorage](https://docs.microsoft.com/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.11#azurerm.azurestackstorage) 참조 콘텐츠를 참조하세요.

## <a name="next-steps"></a>다음 단계

* [Azure Stack용 PowerShell 설치](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [Azure Stack과 함께 사용하도록 PowerShell 구성](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
