---
title: macOS 또는 Linux에 Azure PowerShell 설치
description: macOS 또는 Linux에 Azure PowerShell 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: a54af4b28642fe7b8623550fb05dff33e5c4a7f6
ms.sourcegitcommit: de0e60800df1add9f3400166faacca202ef567d9
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2018
ms.locfileid: "37406498"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>macOS 또는 Linux에 Azure PowerShell 설치

Windows 이외의 플랫폼에서도 PowerShell Core v6에서 Azure PowerShell을 실행할 수 있게 되었습니다. 본 버전의 PowerShell은 .NET Core를 지원하는 모든 플랫폼에서 사용할 수 있도록 빌드되었습니다. 이러한 플랫폼에서 작동하기 위해, Azure PowerShell의 특별 .NET Core 버전이 사용 가능합니다.

> [!NOTE]
> 이때 PowerShell Core v6과 .NET Core용 Azure PowerShell은 아직 베타 버전입니다.
> 이러한 제품에 대한 지원은 제한됩니다. 문제가 있거나 버그를 발견한 경우 GitHub에서 문제를 제출하십시오.
>
> * [PowerShell Core v6에 대한 문제](https://github.com/PowerShell/PowerShell/issues)
> * [Azure PowerShell에 대한 문제](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a>PowerShell Core 설치

PowerShell Core를 위한 설치 지침은 macOS나 대부분의 Linux 배포와 다릅니다.
자세한 지침은 다음 문서에서 찾을 수 있습니다.

- [macOS에 PowerShell Core 설치](/powershell/scripting/setup/installing-powershell-core-on-macos)
- [Linux에 PowerShell Core 설치](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a>.NET Core용 Azure PowerShell 설치

PowerShell Core는 PowerShellGet 모듈이 이미 설치되어 제공됩니다. PowerShell에서 모듈을 설치하려면 상승된 권한이 필요하므로 세션을 슈퍼 사용자로 시작해야 합니다:

```bash
sudo pwsh
```

Azure PowerShell을 설치하려면 다음 명령을 실행합니다:

```powershell
Install-Module AzureRM.NetCore
```

> [!IMPORTANT]
> 다른 아티클에서 설명된 `AzureRM` 모듈은 .NET Core용으로 빌드된 것이 아니며 PowerShell Core와 작동하지 않습니다. `AzureRM`, `AzureRM.NetCore` 둘 다 동일한 cmdlet 이름을 사용하므로 롤업 모듈의 이름과 빌드되는 .NET 버전에 따라 달라집니다.

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

Azure PowerShell을 사용하여 작업을 시작 하려면 [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet을 사용하여 PowerShell 세션에 `AzureRM.Netcore`을 로드한 후 Azure 자격 증명으로 로그인합니다. 모듈 가져오기는 상승된 권한이 필요하지 __않습니다__.

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM.Netcore
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

모든 새 PowerShell 세션에 대해 이러한 단계를 반복해야 합니다. `AzureRM` 모듈을 자동으로 가져오려면 PowerShell 프로필을 설정해야 하며, 프로필 설정은 [프로필 정보](/powershell/module/microsoft.powershell.core/about/about_profiles)에서 알아볼 수 있습니다.
macOS 및 Linux에서, `$Profile` 환경 변수를 통해 프로필 작업을 해야 합니다. Azure 로그인을 세션 간에 유지하는 방법을 알아보려면 [PowerShell 세션 간에 사용자 자격 증명 유지](context-persistence.md)를 참조합니다.

## <a name="available-cmdlets"></a>사용할 수 있는 cmdlet

.NET Core용 Azure PowerShell 모듈은 아직 개발 중입니다. 이러한 모듈은 모듈의 Windows 버전에 대해 사용할 수 있는 cmdlet의 집합을 모두 제공하지 않습니다. 다음 함수는 AzureRM.Netcore 모듈에서 구현됩니다.

* 계정 관리
  - Microsoft 계정, 조직 계정 또는 Microsoft Azure Active Directory를 통해 서비스 사용자로 로그인
  - Save-AzureRmContext로 자격 증명을 디스크에 저장하고 Import-AzureRmContext를 사용하여 저장된 자격 증명 로드
* Environment
  - 다른 기본 Microsoft Azure 환경 가져오기
  - 사용자 지정 환경 추가/설정/제거(예: Azure Stack 또는 Windows Azure 팩 환경)
* 리소스 관리자 및 서비스 관리 인터페이스를 사용하여 Azure 서비스용 평면 cmdlet 관리
  - Virtual Machine
  - App Service(웹 사이트)
  - SQL Database
  - Storage
  - 네트워크

## <a name="next-steps"></a>다음 단계

Azure PowerShell 사용에 대한 자세한 내용은 [Azure PowerShell 시작](get-started-azureps.md) 문서를 참조하세요.
