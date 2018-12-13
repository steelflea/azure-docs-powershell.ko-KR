---
title: macOS 또는 Linux에 Azure PowerShell 설치
description: macOS 또는 Linux에 Azure PowerShell 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/05/2018
ms.openlocfilehash: f60ea1c608be4b1c8319d53303713ba039276abc
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/13/2018
ms.locfileid: "53216673"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>macOS 또는 Linux에 Azure PowerShell 설치

Windows 이외의 플랫폼에서도 PowerShell Core v6에서 Azure PowerShell을 실행할 수 있게 되었습니다. 본 버전의 PowerShell은 .NET Core를 지원하는 모든 플랫폼에서 사용할 수 있도록 빌드되었습니다. 이러한 플랫폼에서 작동하기 위해, Azure PowerShell의 .NET 표준 버전이 사용 가능합니다.

> [!NOTE]
> 이때 .NET Standard에 대한 Azure PowerShell은 아직 베타입니다.
> 문제가 있거나 버그를 발견한 경우 GitHub에서 문제를 제출하십시오.
>
> * [Azure PowerShell에 대한 문제](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a>PowerShell Core 설치

PowerShell Core를 위한 설치 지침은 macOS나 대부분의 Linux 배포와 다릅니다.
자세한 지침은 다음 문서에서 찾을 수 있습니다.

* [macOS에 PowerShell Core 설치](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [Linux에 PowerShell Core 설치](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-standard"></a>.NET 표준용 Azure PowerShell 설치

> [!IMPORTANT]
> 다른 아티클에서 설명된 `AzureRM` 모듈은 PowerShell Core와 작동하지 않습니다.
> PowerShell Core에서 Azure PowerShell 기능을 활용하려면 `Az` 모듈을 설치해야 합니다.

PowerShell Core는 PowerShellGet 모듈이 이미 설치되어 제공됩니다. 해당 명령을 사용하여 PowerShell을 시작합니다.

```bash
pwsh
```

Azure PowerShell을 설치하려면 다음 명령을 실행합니다:

```powershell-interactive
Install-Module Az
```

> [!NOTE]
> 모듈을 설치할 때 사용 권한 오류가 발생하면 모듈을 설치하기 위해 수퍼 사용자 모드로 PowerShell을 실행해야 할 수 있습니다.
>
> ```bash
> sudo pwsh
> ```

기본적으로 PowerShell 갤러리는 PowerShellGet에 대한 신뢰할 수 있는 리포지토리로 구성되지 않습니다. PSGallery를 처음 사용할 때는 다음과 같은 메시지가 표시됩니다.

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

설치를 계속하려면 `Yes` 또는 `Yes to All`로 답변합니다.

## <a name="enable-aliases"></a>별칭을 사용하도록 설정

기존 `AzureRM` 모듈과의 호환성을 위해, 새 `Az` 모듈은 `AzureRM` cmdlet에 대해 이전 버전과 호환되는 별칭을 만들 수 있습니다. 처음으로 모듈을 사용하기 전에 다음 명령 사용하여 이러한 별칭을 설정합니다.

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Enable AzureRM aliases for the user
Enable-AzureRmAlias -Scope CurrentUser
```

이 별칭은 현재 사용자에 대해서만 설정합니다. 별칭을 설정하려면 `-Scope`에 제공할 수 있는 다른 값에 대한 cmdlet 도움말을 확인하십시오.

> [!NOTE]
> 경로 위치에 대한 오류가 발생하면 로컬 시스템에 경로 위치가 있는지 확인하십시오. `CurrentUser` 범위에 대해, `bash`에서 다음 명령을 실행하여 이 오류를 해결할 수 있습니다.
>
> ```bash
> mkdir -p $HOME/.config/powershell
> ```

## <a name="sign-in"></a>로그인

Azure PowerShell을 사용하여 작업을 시작 하려면 [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet을 사용하여 PowerShell 세션에 `Az`을 로드한 후 Azure 자격 증명으로 로그인합니다. 모듈 가져오기는 상승된 권한이 필요하지 __않습니다__.

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

모든 새 PowerShell 세션에 대해 이러한 단계를 반복해야 합니다. `Az` 모듈을 자동으로 가져오려면 PowerShell 프로필을 설정해야 하며, 프로필 설정은 [프로필 정보](/powershell/module/microsoft.powershell.core/about/about_profiles)에서 알아볼 수 있습니다.
macOS 및 Linux에서, `$Profile` 환경 변수를 통해 프로필 작업을 해야 합니다. 세션 간에 Azure 로그인을 유지하는 방법을 보려면 [PowerShell 세션간에 사용자 자격 증명 유지](context-persistence.md)를 참조하세요.

## <a name="next-steps"></a>다음 단계

Azure PowerShell 사용에 대한 자세한 내용은 [Azure PowerShell 시작](get-started-azureps.md) 문서를 참조하세요.
