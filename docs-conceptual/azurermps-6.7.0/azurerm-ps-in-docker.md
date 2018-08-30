---
title: Docker 컨테이너에서 Azure PowerShell 실행
description: Docker 컨테이너에서 Azure PowerShell 실행 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 27ac176d8bd0b142b7740b2ba6793edb500a8af3
ms.sourcegitcommit: f648ac92fafb16cc0e9ca6bc85d00fa327baf396
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/28/2018
ms.locfileid: "43018947"
---
# <a name="run-azure-powershell-in-a-docker-container"></a><span data-ttu-id="3d68f-103">Docker 컨테이너에서 Azure PowerShell 실행</span><span class="sxs-lookup"><span data-stu-id="3d68f-103">Run Azure PowerShell in a Docker container</span></span>

<span data-ttu-id="3d68f-104">Azure PowerShell을 쉽게 이동 가능한 환경에서 실행되도록 하기 위해, Microsoft는 미리 설치된 Azure PowerShell을 사용하여 Docker 이미지를 게시합니다.</span><span class="sxs-lookup"><span data-stu-id="3d68f-104">To make running Azure PowerShell in portable environments easy, Microsoft publishes Docker images with Azure PowerShell pre-installed.</span></span> <span data-ttu-id="3d68f-105">이러한 이미지는 PowerShell Core를 실행하는 Linux 게스트 또는 PowerShell Core 또는 PowerShell 5를 사용하는 Windows 게스트를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="3d68f-105">These images offer a Linux guest running PowerShell Core, or a Windows guest with either PowerShell Core or PowerShell 5.</span></span>

| <span data-ttu-id="3d68f-106">Environment</span><span class="sxs-lookup"><span data-stu-id="3d68f-106">Environment</span></span> | <span data-ttu-id="3d68f-107">Docker 이미지</span><span class="sxs-lookup"><span data-stu-id="3d68f-107">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="3d68f-108">PowerShell(Windows)</span><span class="sxs-lookup"><span data-stu-id="3d68f-108">PowerShell on Windows</span></span> | [<span data-ttu-id="3d68f-109">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="3d68f-109">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="3d68f-110">PowerShell Core(Windows)</span><span class="sxs-lookup"><span data-stu-id="3d68f-110">PowerShell Core on Windows</span></span> | [<span data-ttu-id="3d68f-111">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="3d68f-111">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="3d68f-112">PowerShell Core(Linux)</span><span class="sxs-lookup"><span data-stu-id="3d68f-112">PowerShell Core on Linux</span></span> | [<span data-ttu-id="3d68f-113">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="3d68f-113">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="3d68f-114">이러한 컨테이너 중 하나를 실행하려면 `docker run -it $ImageName`을(를) 사용하여 대화형 터미널을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="3d68f-114">To run any of these containers, you use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="3d68f-115">예를 들어 Linux 컨테이너에서 PowerShell Core를 실행하려면 다음을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="3d68f-115">For example, to run the PowerShell Core on Linux container, use:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="3d68f-116">Docker에서 Windows 컨테이너를 실행하려면 호스트 OS가 Windows여야 하며 Docker를 Windows 컨테이너를 실행하도록 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3d68f-116">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="3d68f-117">Docker에서 Windows와 Linux 환경 사이에서 전환하는 방법에 대한 자세한 내용은, Docker 설명서 [Windows 및 Linux 컨테이너 간 전환](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers)을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="3d68f-117">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>

## <a name="use-a-powershell-core-container"></a><span data-ttu-id="3d68f-118">PowerShell Core 컨테이너 사용</span><span class="sxs-lookup"><span data-stu-id="3d68f-118">Use a PowerShell Core container</span></span>

<span data-ttu-id="3d68f-119">PowerShell Core 컨테이너에는 PowerShell Core v6가 제공되며 `AzureRM.NetCore` 모듈이 미리 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="3d68f-119">The PowerShell Core containers come with PowerShell Core v6 and the `AzureRM.NetCore` module pre-installed.</span></span> <span data-ttu-id="3d68f-120">[Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet을 실행한 후 Azure 계정으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="3d68f-120">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a><span data-ttu-id="3d68f-121">PowerShell이 포함된 Windows 컨테이너를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="3d68f-121">Use the Windows container with PowerShell</span></span>

<span data-ttu-id="3d68f-122">Windows 컨테이너에는 `AzureRM` 모듈이 미리 설치되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3d68f-122">The Windows container has the `AzureRM` module pre-installed.</span></span> <span data-ttu-id="3d68f-123">[Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet을 실행한 후 Azure 계정으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="3d68f-123">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```
