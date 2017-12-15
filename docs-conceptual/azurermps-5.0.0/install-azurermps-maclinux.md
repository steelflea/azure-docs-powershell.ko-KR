---
title: "macOS 및 Linux에서 Azure PowerShell 설치 및 구성 | Microsoft Docs"
description: "macOS 및 Linux에서 Azure PowerShell을 처음으로 설치하고 구성하는 방법입니다."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/06/2017
ms.openlocfilehash: 94b39c18acaca7a4b17b5207feed025442665acc
ms.sourcegitcommit: c42c7176276ec4e1cc3360a93e6b15d32083bf9f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/14/2017
---
# <a name="install-and-configure-azure-powershell-on-macos-and-linux"></a>macOS 및 Linux에서 Azure PowerShell 설치 및 구성

이제 Windows 이외의 플랫폼에서도 PowerShell 6(베타) 및 Azure PowerShell을 설치할 수 있게 되었습니다.
macOS 및 Linux에 Azure PowerShell 설치 프로세스는 Windows와 다르지 않지만, PowerShell 6(베타)을 먼저 설치해야 합니다.

> [!NOTE]

> 이때 PowerShell 6(베타)과 .NET Core용 Azure PowerShell은 아직 베타 버전입니다.
> 이러한 제품에 대한 지원은 제한됩니다. 문제가 있거나 버그를 발견한 경우 GitHub에서 문제를 제출하십시오.
>
> * [PowerShell 6(베타)에 대한 문제](https://github.com/PowerShell/PowerShell/issues)
> * [Azure PowerShell에 대한 문제](https://github.com/azure/azure-docs-powershell/issues)

## <a name="step-1-install-powershell-6-beta"></a>1단계: PowerShell 6(베타) 설치

PowerShell 6(베타) 설치 프로세스는 대상 운영 체제에 따라 달라집니다.
Windows에 PowerShell 6(베타)를 설치할 수 있지만 이 문서에서는 macOS 및 Linux에 설치하는 것에 초점을 둡니다. Windows에서 Azure PowerShell을 사용하려는 경우 Windows용 [설치](./install-azurerm-ps.md) 문서를 참조하세요.

Linux 또는 macOS에 **PowerShell 6**(베타)를 설치하려면 경우 다음을 수행해야 합니다.

1. [GitHub](https://github.com/powershell/powershell#get-powershell)에서 특정 운영 체제 및 버전용 PowerShell을 가져옵니다.
2. 설치 지침을 따릅니다.
   - [Linux](https://github.com/PowerShell/PowerShell/blob/master/docs/installation/linux.md)
   - [macOS](https://github.com/PowerShell/PowerShell/blob/master/docs/installation/linux.md#macos-1012)

## <a name="step-2-install-azure-powershell-for-net-core"></a>2단계: .NET Core용 Azure PowerShell 설치

PowerShell 6(베타)은 PowerShellGet 모듈이 이미 설치되어 제공됩니다. 따라서 PowerShell 갤러리에 게시된 어떤 모듈도 쉽게 설치할 수 있습니다. Azure PowerShell을 설치하려면 새 PowerShell 세션을 열고 다음 명령을 실행합니다.

```powershell
Install-Module AzureRM.NetCore
```

## <a name="step-3-load-the-azurermnetcore-module"></a>3단계: AzureRM.Netcore 모듈 로드

모듈이 설치되면 PowerShell 세션에 모듈을 로드해야 합니다. 모듈은 다음과 같이 `Import-Module` cmdlet을 사용하여 로드됩니다.

```powershell
Import-Module AzureRM.Netcore
```

가져오기가 완료되면 다음 명령을 사용하여 Azure에 로그인을 시도하여 새로 설치한 모듈을 테스트할 수 있습니다.

```powershell
Login-AzureRMAccount
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
  - 가상 컴퓨터
  - App Service(웹 사이트)
  - SQL Database
  - Storage
  - 네트워크

## <a name="next-steps"></a>다음 단계

Azure PowerShell 사용에 대한 자세한 내용은 [Azure PowerShell 시작](get-started-azureps.md) 문서를 참조하세요.
