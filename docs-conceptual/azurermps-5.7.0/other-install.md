---
title: Azure PowerShell을 설치하는 다른 방법
description: MSI 패키지 또는 웹 플랫폼 설치 관리자를 사용하여 Azure PowerShell을 설치하는 방법입니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 0919583d9cb05a75fae3b812eed84109be8b28aa
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323274"
---
# <a name="other-installation-methods"></a>다른 설치 방법

이 문서에서는 MSI 또는 웹 플랫폼 설치 관리자 (WebPI)를 사용하여 Azure PowerShell을 설치 하는 방법에 대해 설명합니다. 또한 Docker 컨테이너 내부에서 Azure PowerShell을 실행할 수도 있습니다. 시스템에 필요한 경우에만 이러한 설치 방법을 사용합니다. Azure PowerShell을 설치하는 정식 방법은 PowerShellGet을 사용하는 방식입니다. PowerShellGet을 사용하여 Azure PowerShell을 설치하는 방법은 [PowerShellGet으로 Azure PowerShell 설치하기](install-azurerm-ps.md)를 참조합니다.

Linux 또는 macOS 환경에 설치하려면 [macOS 또는 Linux에 Azure PowerShell 설치](install-azurermps-maclinux.md)를 참조합니다.

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a>웹 플랫폼 설치 관리자를 사용하여 Windows에 설치 및 업데이트

WebPI에서 최신 Azure PowerShell을 설치하는 것은 이전 버전과 같습니다.
[Azure PowerShell WebPI 패키지](http://aka.ms/webpi-azps)를 다운로드하고 설치를 시작합니다.

> [!NOTE]
> 이전에 PowerShell 갤러리에서 Azure 모듈을 설치한 경우에는 설치 관리자가 해당 모듈을 자동으로 제거합니다. 한 가지 버전의 Azure PowerShell을 설치하여 사용자 환경을 단순화합니다. 그러나 여러 버전이 동시에 설치된 시나리오가 있습니다.
>
> PowerShell 갤러리 모듈은 `$env:ProgramFiles\WindowsPowerShell\Modules`에서 모듈을 설치합니다. 반면, WebPI 설치 관리자는 `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`에서 Azure 모듈을 설치합니다.
>
> 설치 중에 오류가 발생하는 경우 `$env:ProgramFiles\WindowsPowerShell\Modules` 폴더에서 `Azure*`폴더를 수동으로 제거한 다음 다시 설치하면 됩니다.

설치가 완료되면 `$env:PSModulePath` 설정에는 Azure PowerShell cmdlet이 들어 있는 디렉터리가 포함되어야 합니다. 다음 명령을 사용하여 Azure PowerShell이 제대로 설치되어 있는지 확인할 수 있습니다.

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> WebPI에서 설치할 때 발생할 수 있는 알려진 문제가 있습니다. 시스템 업데이트 또는 다른 설치로 인해 컴퓨터를 다시 시작해야 하는 경우 `$env:PSModulePath` 업데이트 과정에서 Azure PowerShell이 설치된 경로가 포함되지 않을 수 있습니다.

설치 후에 cmdlet을 로드하거나 실행하려고 할 때 다음과 같은 오류 메시지가 나타날 수 있습니다.

```
PS C:\> Connect-AzureRmAccount
Connect-AzureRmAccount : The term 'Connect-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Connect-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Connect-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

컴퓨터를 다시 시작하거나 정규화된 경로를 사용하는 모듈을 가져와서 이 오류를 해결할 수 있습니다.

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-or-update-on-windows-using-the-msi-package"></a>MSI 패키지를 사용하여 Windows에 설치 및 업데이트

Azure PowerShell은 [GitHub](https://aka.ms/azps-release)에서 사용할 수 있는 MSI 파일을 사용하여 설치할 수 있습니다. 이전 버전의 Azure 모듈이 설치된 경우 설치 관리자에서 자동으로 제거합니다. MSI 패키지는 `$env:ProgramFiles\WindowsPowerShell\Modules`에서 모듈을 설치하지만 특정 버전 폴더를 만들지는 않습니다.

## <a name="run-in-a-docker-container"></a>Docker 컨테이너에서 실행

Microsoft는 Azure PowerShell로 미리 구성된 Docker 이미지 집합을 유지합니다. 사용할 수 있는 두 가지 유형의 컨테이너: Windows에서 기존의 PowerShell을 실행 중인 컨테이너 및 Windows 또는 Linux에서 PowerShell Core를 실행 중인 컨테이너

| Environment | Docker 이미지 |
|-------------|--------------|
| PowerShell(Windows) | [azuresdk/azure-powershell](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| PowerShell Core(Windows) | [azuresdk/azure-powershell-core:nanoserver](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| PowerShell Core(Linux) | [azuresdk/azure-powershell-core:latest](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

이러한 컨테이너 중 하나를 실행하려면 `docker run -it $ImageName`을(를) 사용하여 대화형 터미널을 가져옵니다. 예를 들어 Linux 컨테이너에서 PowerShell Core를 실행하려면 다음을 사용 합니다.

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> Docker에서 Windows 컨테이너를 실행하려면 호스트 OS가 Windows여야 하며 Docker를 Windows 컨테이너를 실행하도록 설정해야 합니다. Docker에서 Windows와 Linux 환경 사이에서 전환하는 방법에 대한 자세한 내용은, Docker 설명서 [Windows 및 Linux 컨테이너 간 전환](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers)을 참조합니다.