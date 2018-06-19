---
title: PowerShellGet으로 Azure PowerShell 설치
description: PowerShellGet으로 Azure PowerShell을 설치 하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/31/2018
ms.openlocfilehash: 9b7046157e32a5c8473210e9840f9ae1b2f45902
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323104"
---
# <a name="install-azure-powershell-with-powershellget"></a>PowerShellGet으로 Azure PowerShell 설치

이 문서에서는 Windows 환경에서 PowerShellGet을 사용하여 Azure PowerShell 모듈을 설치하는 단계를 설명합니다.  이는 Azure PowerShell을 설치하는 더 좋은 방법이지만 대신 웹 플랫폼 설치 관리자 또는 MSI 패키지로 설치하려는 경우 [다른 설치 방법](other-install.md)을 참조합니다.

macOS 또는 Linux에서 Azure PowerShell을 사용하려는 경우 다음 문서: [macOS 및 Linux에서 Azure PowerShell 설치 및 구성](install-azurermps-maclinux.md)을 참조하세요.

## <a name="system-requirements"></a>시스템 요구 사항

Azure PowerShell 버전 6.1.0에는 PowerShell 버전 5.0 이상이 필요합니다. PowerShell 5.0에 업그레이드에 대한 자세한 내용은 [기존 Windows PowerShell 업그레이드](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell)를 참조합니다.

PowerShellGet은 자동으로 PowerShell 5.0의 일부로 포함됩니다.

## <a name="install-or-update-the-azure-powershell-module"></a>Azure PowerShell 모듈 설치 및 업그레이드

PowerShell 갤러리에서 Azure PowerShell을 설치하려면 상승된 권한이 필요합니다. 상승된 PowerShell 세션에서 다음 명령을 실행합니다.

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

> [!IMPORTANT]
> 이 명령은 시스템에서 기존 Azure PowerShell 설치를 업데이트합니다. 둘 이상의 버전을 설치해야 할 경우 [여러 버전의 Azure PowerShell을 설치할 수 있습니까?](#multiple-versions)에 대한 FAQ 응답을 참조하십시오.

기본적으로 PowerShell 갤러리는 PowerShellGet에 대한 신뢰할 수 있는 리포지토리로 구성되지 않습니다. PSGallery를 처음 사용할 때는 다음과 같은 메시지가 표시됩니다.

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

설치를 계속하려면 'Yes' 또는 'Yes to All'로 답변합니다.

> [!NOTE]
> NuGet 2.8.5.201 이전 버전을 사용하는 경우 최신 버전의 NuGet을 다운로드하여 설치하라는 메시지가 표시됩니다.

AzureRM 모듈은 Azure Resource Manager cmdlet의 롤업 모듈입니다. AzureRM 모듈을 설치하는 경우 이전에 설치되지 않은 Azure PowerShell 모듈이 PowerShell 갤러리에서 다운로드됩니다.

## <a name="load-the-azure-powershell-module"></a>Azure PowerShell 모듈 로드

모듈이 설치되면 PowerShell 세션에 모듈을 로드해야 합니다. 이 작업은 일반(권한이 상승되지 않은) PowerShell 세션에서 수행해야 합니다. 모듈은 다음과 같이 `Import-Module` cmdlet을 사용하여 로드됩니다.

```powershell
Import-Module -Name AzureRM
```

## <a name="reporting-issues-and-feedback"></a>문제 보고 및 피드백

이 도구를 사용하여 버그가 발생하는 경우 [GitHub에서 문제를 제출](https://github.com/Azure/azure-powershell/issues)합니다. 명령줄에서 피드백을 제공하려면 `Send-Feedback` cmdlet을 사용해 보세요.

## <a name="next-steps"></a>다음 단계

Azure PowerShell을 사용하는 방법에 대한 자세한 내용은 다음 문서를 참조하세요.

* [Azure PowerShell 시작](get-started-azureps.md)

## <a name="frequently-asked-questions"></a>질문과 대답

### <a id="helpmechoose"></a>Azure PowerShell 버전은 어떻게 확인할 수 있습니까?

가능한 한 빨리 최신 버전으로 업그레이드하는 것이 좋지만 여러 버전의 Azure PowerShell이 지원됩니다. 설치한 Azure PowerShell의 버전을 확인하려면 명령줄에서 `Get-Module AzureRM`을 실행합니다.

```powershell
Get-Module AzureRM -ListAvailable | Select-Object -Property Name,Version,Path
```

### <a name="can-i-use-azure-powershell-for-azure-classic-deployments"></a>Azure 클래식 배포에 Azure PowerShell을 사용할 수 있습니까?

클래식 배포 모델을 사용하는 배포가 있는 경우 Azure PowerShell의 Service Management 버전을 설치할 수 있습니다. 자세한 내용은 [Azure PowerShell Service Management 모듈 설치](/powershell/azure/servicemanagement/install-azure-ps)를 참조하세요. Azure 모듈과 AzureRM 모듈은 공통 종속성을 공유합니다. Azure와 AzureRM 모듈을 둘 다 사용하는 경우 각 패키지의 동일한 버전을 설치해야 합니다.

### <a name="a-namemultiple-versionscan-i-install-multiple-versions-of-azure-powershell"></a><a name="multiple-versions"/>여러 버전의 Azure PowerShell을 설치할 수 있습니까?

PowerShellGet은 여러 버전을 지원하는 유일한 설치 방법입니다. 여러 버전을 설치하려면 `-RequiredVersion` 매개 변수를 `Install-Module` cmdlet에 추가할 수 있습니다. 예를 들어, 6.1.0 및 1.2.9 두 버전을 설치 하려면:

```powershell
Install-Module -Name AzureRM -RequiredVersion 6.1.0
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

PowerShell 세션에서 한 버전의 모듈만 로드할 수 있습니다. 새 PowerShell 창을 열고 `Import-Module`을 사용하여 특정 버전의 Azure PowerShell 모듈을 가져와야 합니다.

```powershell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

> [!NOTE]
> 2.1.0 버전 및 1.2.6 버전은 나란히 설치하여 사용하도록 설계된 첫 번째 모듈 버전입니다. 이전 버전의 Azure PowerShell을 로드하는 경우는 호환되지 않는 **AzureRM.Profile** 모듈 버전이 로드됩니다. 그 결과 cmdlet을 실행할 때마다 로그인하라는 메시지가 표시됩니다.
