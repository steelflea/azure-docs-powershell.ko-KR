---
title: AzureRM에서 Az로 Azure PowerShell 스크립트 마이그레이션
description: AzureRM 모듈에서 새 Az 모듈로 스크립트를 마이그레이션하는 단계와 도구에 대해 알아보세요.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/07/2018
ms.openlocfilehash: 720387ec1b23f10ddf2b153cf0705b2b6d1b7b82
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/13/2018
ms.locfileid: "53216197"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a>AzureRM에서 Azure PowerShell Az로 마이그레이션

Az 모듈은 AzureRM과 기능 패리티를 가지고 있지만 더 짧고 일관된 cmdlet 이름을 사용합니다.
AzureRM cmdlet용으로 작성된 스크립트는 새 모듈과 자동으로 작동하지 않습니다. 쉽게 전환하기 위해 Az는 AzureRM을 사용하여 기존 스크립트를 실행할 수 있는 도구를 제공합니다. 새 명령 집합으로 마이그레이션은 편리하지 않지만 이 문서는 새로운 모듈로 전환을 시작하는 데 도움이 됩니다.

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a>기존 스크립트가 최신 AzureRM 릴리스와 함께 작동하는지 확인하세요

가장 중요한 단계입니다! 기존 스크립트를 실행하고 AzureRM(__6.13.0__)의 _최신_ 릴리스와 함께 작동하는지 확인하세요. 스크립트가 작동하지 않으면 [AzureRM 마이그레이션 가이드](migration-guide.6.0.0.md)를 읽으세요.

## <a name="install-the-azure-powershell-az-module"></a>Azure PowerShell Az 모듈 설치

첫 번째 단계는 플랫폼에 Az 모듈을 설치하는 것입니다. Az를 설치하려면 AzureRM을 제거해야 합니다.
다음 단계에서는 기존 스크립트를 계속 실행하고 이전 cmdlet 이름과의 호환성을 유지하는 방법을 알아보겠습니다.

Azure PowerShell Az 모듈을 설치하려면 다음 단계를 수행하십시오.

* [AzureRM 모듈을 제거합니다](uninstall-azurerm-ps.md). 가장 최신 버전뿐만 아니라 설치된 _모든_ AzureRM 버전을 제거해야 합니다.
* [Az 모듈 설치](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-alias-mode"></a><a name="aliases"/>AzureRM 별칭 모드 사용

AzureRM을 제거하고 최신 AzureRM 버전과 함께 스크립트가 작동하면 이제 Az 모듈에 대한 호환 모드를 사용할 때입니다. 호환성은 다음 명령으로 사용됩니다.

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

별칭을 사용하면 `Az` 모듈이 설치된 이전 cmdlet 이름을 사용할 수 있습니다. 이러한 별칭은 선택한 범위에 대한 사용자 프로필에 기록됩니다. 사용자 프로필이 없으면 프로일 하나가 만들어집니다.

> [!WARNING]
>
> 이 명령에 대해 다른 `-Scope`를 사용할 수 있지만 권장되지는 않습니다! 별칭은 선택된 범위에 대한 사용자 프로필에 기록되므로 가능한 한 범위를 제한적으로 유지합니다. 별칭을 시스템 전체에서 사용하도록 설정하면 `AzureRM`을 로컬 범위에 설치한 다른 사용자에게 문제가 발생할 수 있습니다.

별칭 모드가 활성화되면 스크립트를 다시 실행하여 스크립트가 여전히 예상대로 작동하는지 확인합니다. 

## <a name="change-module-imports-and-cmdlet-names"></a>모듈 가져오기 및 cmdlet 이름 변경

일반적으로 모듈 이름은 `AzureRM` 및 `Azure`가 `Az`가 되도록 변경되었으며 cmdlet에도 동일하게 적용됩니다.
예를 들어, `AzureRM.Compute` 모듈의 이름이 `Az.Compute`로 변경되었습니다. `New-AzureRmVM`은 `New-AzVM`이 되고 `Get-AzureStorageBlob`은 이제 `Get-AzStorageBlob`입니다.

이 이름 변경에는 예외가 있으며 이름을 바꾸기 전에 알아야 할 사항이 있습니다.

| AzureRM 모듈 | Az 모듈 |
|----------------|-----------|
| AzureRM.DataFactories | Az.DataFactory |
| AzureRM.DataFactoryV2 | Az.DataFactory |
| AzureRM.RecoveryServices.Backup | Az.RecoveryServices |
| AzureRM.RecoveryServices.SiteRecovery | Az.RecoveryServices |

## <a name="summary"></a>요약

이 단계를 따르면 기존 스크립트를 모두 업데이트하여 새 모듈을 사용할 수 있습니다. 마이그레이션을 어렵게 하는 이들 단계에 대해 질문이나 문제가 있는 경우 지침을 개선할 수 있도록 이 문서에 의견을 남겨주세요.
