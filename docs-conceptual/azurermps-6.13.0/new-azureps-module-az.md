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
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/13/2018
ms.locfileid: "53217544"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a>새로운 Azure PowerShell Az 모듈 소개

2018년 11월부터 Azure PowerShell `Az` 모듈을 전체 공개 미리보기로 제공됩니다.
Az은 짧아진 명령과 향상된 안정성을 제공하며, Windows, macOS 및 Linux를 지원합니다. Az은 또한 AzureRM에서 기능 패리티와 쉬운 마이그레이션 경로를 제공합니다.

Az는 .NET 표준 라이브러리를 사용합니다. 즉, PowerShell 5.x 및 PowerShell 6.x에서 실행됩니다.
PowerShell 6.x는 Linux, macOS 및 Windows에서 실행할 수 있으므로, Az는 모든 플랫폼에서 사용할 수 있습니다.
.NET 표준을 사용하면 사용자에게 미치는 영향을 최소화하면서 Azure PowerShell의 코드 기반을 통합할 수 있습니다.

Az는 새로운 모듈이므로 버전이 다시 설정되었습니다. 첫 번째 안정적인 릴리스는 1.0이지만, 모듈은 2018년 11월 현재 AzureRm과 기능 패리티를 유지합니다.

## <a name="upgrade-to-az"></a>Az로 업그레이드

새로운 `Az` 모듈로 업그레이드하는 것이 권장되며 업그레이드 절차는 다음과 같습니다. 이렇게 하려면 다음을 수행합니다.

* [Azure PowerShell AzureRM 모듈 제거](/powershell/azure/uninstall-azurerm-ps)
* [Azure PowerShell Az 모듈 설치](/powershell/azure/install-az-ps)
* 새 명령 집합에 익숙해지면서 `Enable-AzureRMAlias`로 AzureRM의 호환 모드를 사용합니다.

## <a name="migrate-existing-scripts-to-az"></a>기존 스크립트를 Az로 마이그레이션

주요 업데이트가 불편할 수 있습니다. 그러나 `Az` 모듈에는 새로운 구문에 대한 업데이트 작업을 하는 동안 기존 스크립트를 사용할 수 있도록 해주는 호환 모드가 있습니다. `Enable-AzureRmAlias` cmdlet을 사용하여 `AzureRM` 호환 모드를 활성화합니다. 이 cmdlet은 `AzureRM` cmdlet 이름을 새 `Az` cmdlet 이름의 별칭으로 정의합니다.

새로운 cmdlet 이름은 쉽게 익힐 수 있도록 되었습니다. cmdlet 이름에 `AzureRm` 또는 `Azure`를 사용하는 대신 `Az`를 사용합니다. 예를 들어, 이전 명령 `New-AzureRmVm`은 `New-AzVm`이 됩니다.

마이그레이션 프로세스에 대한 전체 설명은 [AzureRM에서 Az로 마이그레이션](migrate-from-azurerm-to-az.md)을 참조하세요.

## <a name="the-future-of-support-for-azurerm"></a>AzureRM에 대한 향후 지원

2018년 12월에 `Az` 버전 1.0이 릴리스되면 기존 `AzureRM` 모듈은 더 이상 새로운 cmdlet 또는 기능을 받지 않습니다. 그러나 `AzureRM`은 공식적으로 유지되며 버그 수정도 이루어집니다. 최신 Azure 서비스 및 기능을 유지하기 위해서는 `Az` 모듈로 전환해야 합니다.