---
title: macOS 또는 Linux에 Azure PowerShell 설치
description: macOS 또는 Linux에 Azure PowerShell 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 17912c155255b6fdfd3cfb9242163b67d405dc03
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323172"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>macOS 또는 Linux에 Azure PowerShell 설치

Windows 이외의 플랫폼에서도 PowerShell Core v6 위에 Azure PowerShell을 실행할 수 있게 되었습니다. Windows용 .NET Framework 기반 표준 Azure PowerShell 대신, 본 제품은 .NET Core용 기반으로서 .Net Core 런타임을 지원하는 모든 플랫폼에서 실행할 수 있습니다.

> [!NOTE]
> 이때 PowerShell Core v6과 .NET Core용 Azure PowerShell은 아직 베타 버전입니다.
> 이러한 제품에 대한 지원은 제한됩니다. 문제가 있거나 버그를 발견한 경우 GitHub에서 문제를 제출하십시오.
>
> * [PowerShell Core v6에 대한 문제](https://github.com/PowerShell/PowerShell/issues)
> * [Azure PowerShell에 대한 문제](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core-v6"></a>PowerShell Core v6 설치

Linux 또는 macOS에 PowerShell Core v6을 설치하는 것은 Linux 배포 및 OS 버전에 따라 달라집니다.
자세한 지침은 다음 문서에서 찾을 수 있습니다.

- [macOS에 PowerShell Core 설치](/powershell/scripting/setup/installing-powershell-core-on-macos)
- [Linux에 PowerShell Core 설치](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a>.NET Core용 Azure PowerShell 설치

PowerShell Core v6은 PowerShellGet 모듈이 이미 설치되어 제공됩니다. 따라서 PowerShell 갤러리에 게시된 어떤 모듈도 쉽게 설치할 수 있습니다. Azure PowerShell을 설치하려면 새 PowerShell 세션을 열고 다음 명령을 실행합니다.

```powershell
Install-Module AzureRM.NetCore
```

## <a name="load-the-azurermnetcore-module"></a>AzureRM.Netcore 모듈 로드

모듈이 설치되면 PowerShell 세션에 모듈을 로드해야 합니다. 모듈은 다음과 같이 `Import-Module` cmdlet을 사용하여 로드됩니다.

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

가져오기가 완료되면 다음 명령을 사용하여 Azure에 로그인을 시도하여 새로 설치한 모듈을 테스트할 수 있습니다.

```powershell
Connect-AzureRmAccount
```

위의 명령을 실행하면 `https://aka.ms/devicelogin`으로 이동하여 제공된 코드를 입력하라는 메시지가 나타납니다.

## <a name="available-cmdlets"></a>사용할 수 있는 cmdlet

.NET 표준용 Azure PowerShell 모듈은 아직 개발 중입니다. 이러한 모듈은 모듈의 Windows 버전에 대해 사용할 수 있는 cmdlet의 집합을 모두 제공하지 않습니다. 다음 함수는 AzureRM.Netcore 모듈에서 구현됩니다.

* 계정 관리
  - Microsoft 계정, 조직 계정 또는 Azure Active Directory를 통해 서비스 사용자로 로그인
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
