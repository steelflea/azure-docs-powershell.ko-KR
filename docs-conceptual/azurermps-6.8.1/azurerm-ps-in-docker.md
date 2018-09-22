---
title: Docker 컨테이너에서 Azure PowerShell 실행
description: Docker 컨테이너에서 Azure PowerShell 실행 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.openlocfilehash: 0ed8f50abbcb2aa00192196f19004446dc696b5d
ms.sourcegitcommit: bc88e64c494337821274d6a66c1edad656c119c5
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/20/2018
ms.locfileid: "46304015"
---
# <a name="run-azure-powershell-in-a-docker-container"></a>Docker 컨테이너에서 Azure PowerShell 실행

Microsoft는 Azure PowerShell이 미리 설치된 상태로 Docker 이미지를 게시합니다. 이러한 이미지는 Azure PowerShell 실험에 사용하거나 격리된 환경에서 실행할 수 있습니다. PowerShell Core 및 PowerShell 5를 모두 실행하는 이미지는 다음과 같습니다. 

| Environment | Docker 이미지 |
|-------------|--------------|
| PowerShell(Windows) | [azuresdk/azure-powershell](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| PowerShell Core(Windows) | [azuresdk/azure-powershell-core:nanoserver](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| PowerShell Core(Linux) | [azuresdk/azure-powershell-core:nanoserver](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

이러한 컨테이너를 실행하려면 `docker run -it $ImageName`을 사용하여 대화형 터미널을 가져옵니다. 예들를 어 PowerShell Core에서 Linux 컨테이너를 실행하려면 다음을 수행합니다.

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> Docker에서 Windows 컨테이너를 실행하려면 호스트 OS가 Windows여야 하며 Docker를 Windows 컨테이너를 실행하도록 설정해야 합니다. Docker에서 Windows와 Linux 환경 사이에서 전환하는 방법에 대한 자세한 내용은, Docker 설명서 [Windows 및 Linux 컨테이너 간 전환](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers)을 참조합니다.

## <a name="use-a-powershell-core-container"></a>PowerShell Core 컨테이너 사용

PowerShell Core 컨테이너에는 PowerShell Core v6가 제공되며 `AzureRM.NetCore` 모듈이 미리 설치됩니다. [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet을 실행한 후 Azure 계정으로 로그인합니다.

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a>PowerShell이 포함된 Windows 컨테이너를 사용합니다.

Windows 컨테이너에는 `AzureRM` 모듈이 미리 설치되어 있습니다. [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet을 실행한 후 Azure 계정으로 로그인합니다.

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```
