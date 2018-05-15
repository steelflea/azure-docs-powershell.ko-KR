---
title: Azure PowerShell 변경 로그 | Microsoft Docs
description: Azure PowerShell에 대한 최신 릴리스의 변경 내용입니다.
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: 5fe7591855577e083aad5923aed37b18d0b2a40c
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/08/2018
---
# <a name="release-notes"></a><span data-ttu-id="64d40-103">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="64d40-103">Release notes</span></span>

<span data-ttu-id="64d40-104">Azure PowerShell에 대한 릴리스의 변경 내용 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="64d40-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-129"></a><span data-ttu-id="64d40-105">1.2.9 버전</span><span class="sxs-lookup"><span data-stu-id="64d40-105">Version 1.2.9</span></span>

<span data-ttu-id="64d40-106">이 릴리스의 변경 내용</span><span class="sxs-lookup"><span data-stu-id="64d40-106">Changes This Release</span></span>

* <span data-ttu-id="64d40-107">AzureRm.AzureStackAdmin 모듈</span><span class="sxs-lookup"><span data-stu-id="64d40-107">AzureRm.AzureStackAdmin Module</span></span>
    + <span data-ttu-id="64d40-108">Admin Azure 리소스 관리자 및 tenant azure 리소스 관리자 분할 지원에 대한 Add-AzureRmResourceProviderRegistration cmdlet 변경.</span><span class="sxs-lookup"><span data-stu-id="64d40-108">Changes in the Add-AzureRmResourceProviderRegistration cmdlet for the support of Admin Azure resource manager and tenant azure resource manager split.</span></span> <span data-ttu-id="64d40-109">새로운 -ResourceManagerType 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="64d40-109">A new parameter -ResourceManagerType has been added.</span></span>
    + <span data-ttu-id="64d40-110">각 cmdlet에서 -AdminUri, -ApiVersion, -SubscriptionId 및 -Token 매개 변수 제거.</span><span class="sxs-lookup"><span data-stu-id="64d40-110">Removal of the parameters -AdminUri, -ApiVersion, -SubscriptionId and -Token from each cmdlets.</span></span> <span data-ttu-id="64d40-111">이 매개 변수는 더 이상 사용되지 않을 것이며 지금은 제거되었다는 경고를 제공하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="64d40-111">We have been printing warnings that these parameters will be deprecated and now they got removed.</span></span>
* <span data-ttu-id="64d40-112">AzureStackStorage 모듈</span><span class="sxs-lookup"><span data-stu-id="64d40-112">AzureStackStorage module</span></span>
    + <span data-ttu-id="64d40-113">컨테이너 마이그레이션 시나리오를 지원하는 새 cmdlet 추가.</span><span class="sxs-lookup"><span data-stu-id="64d40-113">Added new cmdlets to support container migration scenarios.</span></span>
    + <span data-ttu-id="64d40-114">내부 구성 요소 및 기본 기능을 참조하는 cmdlet 제거.</span><span class="sxs-lookup"><span data-stu-id="64d40-114">Removed cmdlets referring to internal components and underlying features.</span></span>
* <span data-ttu-id="64d40-115">AzureRM.BootStrapper</span><span class="sxs-lookup"><span data-stu-id="64d40-115">AzureRM.BootStrapper</span></span>
    + <span data-ttu-id="64d40-116">버전 프로필을 사용하여 Azure PowerShell cmdlet 버전을 관리하는 새 모듈 생성</span><span class="sxs-lookup"><span data-stu-id="64d40-116">Created new module to manage versions of Azure PowerShell cmdlets through the use of version profiles</span></span>