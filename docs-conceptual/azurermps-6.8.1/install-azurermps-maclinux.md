---
title: macOS 또는 Linux에 Azure PowerShell 설치
description: macOS 또는 Linux에 Azure PowerShell 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: f014d62e898da195a38052db6b7e37a2cd96dfdd
ms.sourcegitcommit: 3a02e0c85c83de873981dd392500bc82c1cf9286
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/24/2018
ms.locfileid: "46560119"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>macOS 또는 Linux에 Azure PowerShell 설치

Windows 이외의 플랫폼에서도 PowerShell Core v6에서 Azure PowerShell을 실행할 수 있게 되었습니다. 본 버전의 PowerShell은 .NET Core를 지원하는 모든 플랫폼에서 사용할 수 있도록 빌드되었습니다. 이러한 플랫폼에서 작동하기 위해, Azure PowerShell의 .NET 표준 버전이 사용 가능합니다.

> [!NOTE]
> 이때 PowerShell Core v6과 .NET Core용 Azure PowerShell은 아직 베타 버전입니다.
> 이러한 제품에 대한 지원은 제한됩니다. 문제가 있거나 버그를 발견한 경우 GitHub에서 문제를 제출하십시오.
>
> * [PowerShell Core v6에 대한 문제](https://github.com/PowerShell/PowerShell/issues)
> * [Azure PowerShell에 대한 문제](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a>PowerShell Core 설치

PowerShell Core를 위한 설치 지침은 macOS나 대부분의 Linux 배포와 다릅니다.
자세한 지침은 다음 문서에서 찾을 수 있습니다.

* [macOS에 PowerShell Core 설치](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [Linux에 PowerShell Core 설치](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a>.NET Core용 Azure PowerShell 설치

PowerShell Core는 PowerShellGet 모듈이 이미 설치되어 제공됩니다. PowerShell에서 모듈을 설치하려면 상승된 권한이 필요하므로 세션을 슈퍼 사용자로 시작해야 합니다:

```bash
sudo pwsh
```

Azure PowerShell을 설치하려면 다음 명령을 실행합니다:

```powershell
Install-Module Az
```

> [!IMPORTANT]
> 다른 아티클에서 설명된 `AzureRM` 모듈은 .NET Core용으로 빌드된 것이 아니며 PowerShell Core와 작동하지 않습니다. `Az` 모듈에는 모든 `AzureRM` cmdlet에 대한 명령 별칭이 포함되어 있으므로 `AzureRM`의 모든 설명서가 적용됩니다.

기본적으로 PowerShell 갤러리는 PowerShellGet에 대한 신뢰할 수 있는 리포지토리로 구성되지 않습니다. PSGallery를 처음 사용할 때는 다음과 같은 메시지가 표시됩니다.

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

설치를 계속하려면 `Yes` 또는 `Yes to All`로 답변합니다.

## <a name="sign-in"></a>로그인

Azure PowerShell을 사용하여 작업을 시작 하려면 [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet을 사용하여 PowerShell 세션에 `Az`을 로드한 후 Azure 자격 증명으로 로그인합니다. 모듈 가져오기는 상승된 권한이 필요하지 __않습니다__.

```powershell
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

모든 새 PowerShell 세션에 대해 이러한 단계를 반복해야 합니다. `Az` 모듈을 자동으로 가져오려면 PowerShell 프로필을 설정해야 하며, 프로필 설정은 [프로필 정보](/powershell/module/microsoft.powershell.core/about/about_profiles)에서 알아볼 수 있습니다.
macOS 및 Linux에서, `$Profile` 환경 변수를 통해 프로필 작업을 해야 합니다. 세션 간에 Azure 로그인을 유지하는 방법을 보려면 [PowerShell 세션간에 사용자 자격 증명 유지](context-persistence.md)를 참조하세요.

## <a name="next-steps"></a>다음 단계

Azure PowerShell 사용에 대한 자세한 내용은 [Azure PowerShell 시작](get-started-azureps.md) 문서를 참조하세요.
