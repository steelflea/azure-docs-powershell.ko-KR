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
ms.sourcegitcommit: 6c38e86e16da99f65cd183c63e34f7176b121ab8
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/04/2018
ms.locfileid: "47425264"
---
# <a name="run-azure-powershell-in-a-docker-container"></a><span data-ttu-id="923cc-103">Docker 컨테이너에서 Azure PowerShell 실행</span><span class="sxs-lookup"><span data-stu-id="923cc-103">Run Azure PowerShell in a Docker container</span></span>

<span data-ttu-id="923cc-104">Microsoft는 Azure PowerShell이 미리 설치된 상태로 Docker 이미지를 게시합니다.</span><span class="sxs-lookup"><span data-stu-id="923cc-104">Microsoft publishes Docker images with Azure PowerShell pre-installed.</span></span> <span data-ttu-id="923cc-105">이러한 이미지는 Azure PowerShell 실험에 사용하거나 격리된 환경에서 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="923cc-105">These images allow for experimenting with Azure PowerShell or running it in an isolated environment.</span></span> <span data-ttu-id="923cc-106">PowerShell Core 및 PowerShell 5를 모두 실행하는 이미지는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="923cc-106">There are images running both PowerShell Core and PowerShell 5.</span></span> 

| <span data-ttu-id="923cc-107">Environment</span><span class="sxs-lookup"><span data-stu-id="923cc-107">Environment</span></span> | <span data-ttu-id="923cc-108">Docker 이미지</span><span class="sxs-lookup"><span data-stu-id="923cc-108">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="923cc-109">PowerShell(Windows)</span><span class="sxs-lookup"><span data-stu-id="923cc-109">PowerShell on Windows</span></span> | [<span data-ttu-id="923cc-110">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="923cc-110">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="923cc-111">PowerShell Core(Windows)</span><span class="sxs-lookup"><span data-stu-id="923cc-111">PowerShell Core on Windows</span></span> | [<span data-ttu-id="923cc-112">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="923cc-112">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="923cc-113">PowerShell Core(Linux)</span><span class="sxs-lookup"><span data-stu-id="923cc-113">PowerShell Core on Linux</span></span> | [<span data-ttu-id="923cc-114">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="923cc-114">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="923cc-115">이러한 컨테이너를 실행하려면 `docker run -it $ImageName`을 사용하여 대화형 터미널을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="923cc-115">To run any of these containers, use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="923cc-116">예들를 어 PowerShell Core에서 Linux 컨테이너를 실행하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="923cc-116">For example, to run a Linux container with PowerShell Core:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="923cc-117">Docker에서 Windows 컨테이너를 실행하려면 호스트 OS가 Windows여야 하며 Docker를 Windows 컨테이너를 실행하도록 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="923cc-117">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="923cc-118">Docker에서 Windows와 Linux 환경 사이에서 전환하는 방법에 대한 자세한 내용은, Docker 설명서 [Windows 및 Linux 컨테이너 간 전환](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers)을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="923cc-118">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>

## <a name="use-a-powershell-core-container"></a><span data-ttu-id="923cc-119">PowerShell Core 컨테이너 사용</span><span class="sxs-lookup"><span data-stu-id="923cc-119">Use a PowerShell Core container</span></span>

<span data-ttu-id="923cc-120">PowerShell Core 컨테이너에는 PowerShell Core v6가 제공되며 `AzureRM.NetCore` 모듈이 미리 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="923cc-120">The PowerShell Core containers come with PowerShell Core v6 and the `AzureRM.NetCore` module pre-installed.</span></span> <span data-ttu-id="923cc-121">[Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet을 실행한 후 Azure 계정으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="923cc-121">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a><span data-ttu-id="923cc-122">PowerShell이 포함된 Windows 컨테이너를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="923cc-122">Use the Windows container with PowerShell</span></span>

<span data-ttu-id="923cc-123">Windows 컨테이너에는 `AzureRM` 모듈이 미리 설치되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="923cc-123">The Windows container has the `AzureRM` module pre-installed.</span></span> <span data-ttu-id="923cc-124">[Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet을 실행한 후 Azure 계정으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="923cc-124">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```
