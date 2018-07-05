---
title: Docker 컨테이너에서 Azure PowerShell 실행
description: Docker 컨테이너에서 Azure PowerShell 실행 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: b224beb95809d0e48c6f1dd5985de45b3b4df816
ms.sourcegitcommit: 4c775721461210431bd913f28d1f1e6f1976880a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/28/2018
ms.locfileid: "37091629"
---
## <a name="run-azure-powershell-in-a-docker-container"></a>Docker 컨테이너에서 Azure PowerShell 실행

Azure PowerShell로 미리 구성된 Docker 이미지 집합이 있습니다. 사용할 수 있는 두 가지 유형의 컨테이너: Windows에서 기존의 PowerShell을 실행 중인 컨테이너 및 Windows 또는 Linux에서 PowerShell Core를 실행 중인 컨테이너

| Environment | Docker 이미지 |
|-------------|--------------|
| PowerShell(Windows) | [azuresdk/azure-powershell](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| PowerShell Core(Windows) | [azuresdk/azure-powershell-core:nanoserver](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| PowerShell Core(Linux) | [azuresdk/azure-powershell-core:nanoserver](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

이러한 컨테이너 중 하나를 실행하려면 `docker run -it $ImageName`을(를) 사용하여 대화형 터미널을 가져옵니다. 예를 들어 Linux 컨테이너에서 PowerShell Core를 실행하려면 다음을 사용 합니다.

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