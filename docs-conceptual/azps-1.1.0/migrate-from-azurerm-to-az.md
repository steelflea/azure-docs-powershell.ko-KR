---
title: AzureRM에서 Az로 Azure PowerShell 스크립트 마이그레이션
description: AzureRM 모듈에서 새 Az 모듈로 스크립트를 마이그레이션하는 단계와 도구에 대해 알아보세요.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 28122ca953d62b405f19effbbc680f2dc6202cca
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/16/2019
ms.locfileid: "54341989"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a>AzureRM에서 Azure PowerShell Az로 마이그레이션

Az 모듈은 AzureRM과 기능 패리티를 가지고 있지만 더 짧고 일관된 cmdlet 이름을 사용합니다.
AzureRM cmdlet용으로 작성된 스크립트는 새 모듈과 자동으로 작동하지 않습니다. 쉽게 전환하기 위해 Az는 AzureRM을 사용하여 기존 스크립트를 실행할 수 있는 도구를 제공합니다. 새 명령 집합으로 마이그레이션은 편리하지 않지만 이 문서는 새로운 모듈로 전환을 시작하는 데 도움이 됩니다.

AzureRM과 Az 간의 호환성이 손상되는 전체 변경 목록을 보려면 [Az 1.0.0 마이그레이션 가이드](migrate-az-1.0.0.md)를 참조하세요.

## <a name="check-for-installed-versions-of-azurerm"></a>설치된 AzureRM 버전 확인

Az 모듈은 AzureRM 모듈과 나란히 설치할 수 있지만 권장하지는 않습니다. 모든 마이그레이션 단계를 수행하기 전에 시스템에 설치된 AzureRM의 버전을 확인합니다. 이렇게 하면 스크립트가 최신 릴리스에서 이미 실행되고 있는지 확인하고 AzureRM을 제거하지 않고 명령 별칭을 사용할 수 있는지 여부를 알려줍니다.

설치한 AzureRM의 버전을 확인하려면 다음 명령을 입력합니다.

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a>기존 스크립트가 최신 AzureRM 릴리스와 함께 작동하는지 확인하세요

가장 중요한 단계입니다! 기존 스크립트를 실행하고 AzureRM(__6.13.1__)의 _최신_ 릴리스와 함께 작동하는지 확인하세요. 스크립트가 작동하지 않으면 [AzureRM 마이그레이션 가이드](/powershell/azure/azurerm/migration-guide.6.0.0)를 읽으세요.

## <a name="install-the-azure-powershell-az-module"></a>Azure PowerShell Az 모듈 설치

첫 번째 단계는 플랫폼에 Az 모듈을 설치하는 것입니다. Az를 설치할 때는 AzureRM을 제거하는 것이 좋습니다. 다음 단계에서는 기존 스크립트를 계속 실행하고 이전 cmdlet 이름과의 호환성을 유지하는 방법을 알아보겠습니다.

Azure PowerShell Az 모듈을 설치하려면 다음 단계를 수행하십시오.

* __권장__: [AzureRM 모듈을 제거합니다](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module).
  가장 최신 버전뿐만 아니라 설치된 _모든_ AzureRM 버전을 제거해야 합니다.
* [Az 모듈 설치](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-compatibility-aliases"></a><a name="aliases"/>AzureRM 호환성 별칭을 사용하도록 설정 

> [!IMPORTANT]
>
> _모든_ 버전의 AzureRM을 제거한 경우에만 호환성 모드를 활성화하세요. AzureRM cmdlet과의 호환 모드를 계속 사용하도록 설정하면 예기치 않은 동작이 발생할 수 있습니다. AzureRM을 설치하기로 결정한 경우 이 단계를 건너뛰세요. 그러나 AzureRM cmdlet은 이전 모듈을 사용하고 Az cmdlet은 호출하지 않습니다.

AzureRM을 제거하고 최신 AzureRM 버전과 함께 스크립트가 작동하면 이제 Az 모듈에 대한 호환 모드를 사용할 때입니다. 호환성은 다음 명령으로 사용됩니다.

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

별칭을 사용하면 Az 모듈이 설치된 이전 cmdlet 이름을 사용할 수 있습니다. 이러한 별칭은 선택한 범위에 대한 사용자 프로필에 기록됩니다. 사용자 프로필이 없으면 프로일 하나가 만들어집니다.

> [!WARNING]
>
> 이 명령에 대해 다른 `-Scope`를 사용할 수 있지만 권장되지는 않습니다. 별칭은 선택된 범위에 대한 사용자 프로필에 기록되므로 가능한 한 범위를 제한적으로 유지합니다. 별칭을 시스템 전체에서 사용하도록 설정하면 AzureRM을 로컬 범위에 설치한 다른 사용자에게 문제가 발생할 수 있습니다.

별칭 모드가 활성화되면 스크립트를 다시 실행하여 스크립트가 여전히 예상대로 작동하는지 확인합니다. 

## <a name="change-module-imports-and-cmdlet-names"></a>모듈 가져오기 및 cmdlet 이름 변경

일반적으로 모듈 이름은 `AzureRM` 및 `Azure`가 `Az`가 되도록 변경되었으며 cmdlet에도 동일하게 적용됩니다.
예를 들어, `AzureRM.Compute` 모듈의 이름이 `Az.Compute`로 변경되었습니다. `New-AzureRMVM`은 `New-AzVM`이 되고 `Get-AzureStorageBlob`은 이제 `Get-AzStorageBlob`입니다.

이 이름 변경에는 알아야 할 예외 사항이 있습니다. `AzureRM` 또는 `Azure`를 `Az`로 변경하는 것 이외에 일부 cmdlet의 접미사에 영향을 주지 않고 일부 모듈의 이름을 바꾸거나 기존 모듈에 병합했습니다. 또는 전체 cmdlet 접미사가 새로운 모듈 이름을 반영하도록 변경되었습니다.

| AzureRM 모듈 | Az 모듈 | Cmdlet 접미사가 변경되었습니까? |
|----------------|-----------|------------------------|
| AzureRM.Profile | Az.Accounts | 예 |
| AzureRM.Insights | Az.Monitor | 예 |
| AzureRM.DataFactories | Az.DataFactory | 예 |
| AzureRM.DataFactoryV2 | Az.DataFactory | 예 |
| AzureRM.RecoveryServices.Backup | Az.RecoveryServices | 아니요 |
| AzureRM.RecoveryServices.SiteRecovery | Az.RecoveryServices | 아니요 |
| AzureRM.Tags | Az.Resources | 아니요 |
| AzureRM.MachineLearningCompute | Az.MachineLearning | 아니요 |
| AzureRM.UsageAggregates | Az.Billing | 아니요 |
| AzureRM.Consumption | Az.Billing | 아니요 |

## <a name="summary"></a>요약

이 단계를 따르면 기존 스크립트를 모두 업데이트하여 새 모듈을 사용할 수 있습니다. 마이그레이션을 어렵게 하는 이들 단계에 대해 질문이나 문제가 있는 경우 지침을 개선할 수 있도록 이 문서에 의견을 남겨주세요.
