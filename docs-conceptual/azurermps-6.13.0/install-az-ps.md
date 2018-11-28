---
title: PowerShellGet으로 Azure PowerShell 'Az' 설치
description: PowerShellGet으로 Azure PowerShell을 Windows, macOS, Linux에 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/16/2018
ms.openlocfilehash: 32e96c6459c9db0c4b9eda0cc170c85ba99a22ca
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/22/2018
ms.locfileid: "52259797"
---
# <a name="install-the-azure-powershell-az-module"></a>Azure PowerShell ‘Az’ 모듈 설치

이 문서에서는 PowerShellGet을 사용하여 Azure PowerShell 모듈을 설치하는 방법을 설명합니다. 이러한 지침은 Windows, macOS 및 Linux 플랫폼에서 작동합니다. Az의 미리보기 릴리스에서는 다른 설치 방법이 지원되지 않습니다. 

## <a name="requirements"></a>요구 사항

Azure PowerShell은 Windows의 PowerShell 5.x 또는 모든 플랫폼의 PowerShell 6.x에서 작동합니다. 시스템의 PowerShell 버전을 확인하려면 다음 명령을 실행합니다.

```powershell-interactive
$PSVersionTable.PSVersion
```

오래된 버전이 있거나 PowerShell을 설치해야 하는 경우 [다양한 버전의 PowerShell 설치](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6)를 참조하세요. 플랫폼에 대한 설치 정보는 해당 페이지에 링크되어 있습니다.

## <a name="install-the-azure-powershell-module"></a>Azure PowerShell 모듈 설치

> [!IMPORTANT]
>
> 한 시스템에 `AzureRM` 및 `Az` 모듈을 동시에 설치하지 않아야 합니다. `Az` 모듈을 설치하려면 `AzureRM`을 제거해야 합니다. 이를 수행하는 방법에 대한 지침은 [Azure PowerShell 모듈(AzureRM) 제거](uninstall-azurerm-ps.md)를 참조하세요.

모듈을 전역 범위에 설치하려면 상승된 권한으로 PowerShell 갤러리에서 모듈을 설치해야 합니다. Azure PowerShell을 설치하려면 상승된 세션에서 다음 명령을 실행합니다(Windows에서는 "관리자 권한으로 실행", macOS 또는 Linux에서는 슈퍼 사용자 권한으로 실행).

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

관리자 권한에 대한 액세스 권한이 없으면 `-Scope` 인수를 추가하여 현재 사용자를 위해 설치할 수 있습니다.

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

기본적으로 PowerShell 갤러리는 PowerShellGet에 대한 신뢰할 수 있는 리포지토리로 구성되지 않습니다. PSGallery를 처음 사용할 때는 다음과 같은 메시지가 표시됩니다.

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

설치를 계속하려면 `Yes` 또는 `Yes to All`로 답변합니다.

`Az` 모듈은 Azure PowerShell cmdlet의 롤업 모듈입니다. 설치하면 사용 가능한 모든 Azure Resource Manager 모듈이 다운로드되고 cmdlet을 사용할 수 있게 됩니다.

## <a name="sign-in"></a>로그인

Azure PowerShell을 사용하여 작업을 시작하려면 Azure 자격 증명으로 로그인합니다.

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> 모듈 자동 로딩을 비활성화한 경우 `Import-Module Az`을 사용하여 모듈을 수동으로 가져와야 합니다. 모듈 구조화 방식으로 인해 몇 초 정도 걸릴 수 있습니다.

모든 새 PowerShell 세션에 대해 이러한 단계를 반복해야 합니다. PowerShell 세션 간에 Azure 로그인을 유지하는 방법을 보려면 [PowerShell 세션간에 사용자 자격 증명 유지](context-persistence.md)를 참조하세요.

## <a name="update-the-azure-powershell-module"></a>Azure PowerShell 모듈 업데이트

[Update-Module](/powershell/module/powershellget/update-module)을 실행하여 Azure PowerShell 설치를 업데이트할 수 있습니다. 이 명령은 이전 버전을 제거하지 __않습니다__.

```powershell-interactive
Update-Module -Name Az
```

Azure PowerShell의 이전 버전을 시스템에서 제거하려면, [Azure PowerShell 모듈 제거](uninstall-azurerm-ps.md)를 참조합니다.

## <a name="use-multiple-versions-of-azure-powershell"></a>여러 버전의 Azure PowerShell 사용

Azure PowerShell은 버전을 2개 이상 설치할 수 없습니다. 여러 버전의 Azure PowerShell이 설치되어 있는지 확인하려면 다음 명령을 사용합니다.

```powershell-interactive
Get-Module -Name Az -List | select Name,Version
```

Azure PowerShell의 버전을 제거하려면 [Azure PowerShell 모듈 제거](uninstall-azurerm-ps.md)를 참조합니다.

`Install-Module` 및 `Import-Module`과 함께 `-RequiredVersion` 인수를 사용하여 `Az` 모듈의 특정 버전을 로드할 수 있습니다.

```powershell-interactive
Install-Module -Name Az -RequiredVersion 0.4.0
Import-Module -Name Az -RequiredVersion 0.4.0
```

두 개 이상의 모듈 버전이 설치되어 있는 경우,기본적으로 최신 버전이 로드됩니다.

## <a name="provide-feedback"></a>피드백 제공

Azure Powershell 사용 중 버그 발생 시, [ GitHub에서 문제를 제출](https://github.com/Azure/azure-powershell/issues)하세요.
명령줄에서 피드백을 제공하려면 [Send-Feedback](/powershell/module/az.profile/send-feedback) cmdlet을 사용해 보세요.

## <a name="next-steps"></a>다음 단계

Azure PowerShell 사용을 시작하려면, [Azure PowerShell 시작](get-started-azureps.md)을 참조하여 모듈 및 모듈의 기능에 대해 자세히 알아보세요.
