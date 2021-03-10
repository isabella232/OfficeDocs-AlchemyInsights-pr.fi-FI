---
title: Nykyisen selainympäristön arviointi ja tavoitteiden määritteleminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693643"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a><span data-ttu-id="b2514-102">Nykyisen selainympäristön arviointi ja tavoitteiden määritteleminen</span><span class="sxs-lookup"><span data-stu-id="b2514-102">Evaluate your existing browser environment and define goals</span></span>

<span data-ttu-id="b2514-103">Nykyisen selaintilasi ja projektinäkösi ymmärtäminen vie aikaa varmistaa, että kaikki projektin sidosryhmät ovat linjassa ja että ne työskentelevät kohti samaa tavoitetta.</span><span class="sxs-lookup"><span data-stu-id="b2514-103">Taking time to understand your current browser state and project vision ensures all project stakeholders are aligned and are working toward the same goal.</span></span> <span data-ttu-id="b2514-104">Toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="b2514-104">Follow these steps:</span></span>

1. <span data-ttu-id="b2514-105">Määritä nykyinen tilasi.</span><span class="sxs-lookup"><span data-stu-id="b2514-105">Define your current state.</span></span> <span data-ttu-id="b2514-106">Ota seuraavat seikat huomioon:</span><span class="sxs-lookup"><span data-stu-id="b2514-106">Consider the following:</span></span>
- <span data-ttu-id="b2514-107">Mitkä selaimet ovat tällä hetkellä käytössä ympäristössäsi?</span><span class="sxs-lookup"><span data-stu-id="b2514-107">Which browsers are currently deployed in your environment?</span></span>
- <span data-ttu-id="b2514-108">Mikä selain on määritetty oletusselaimeksi?</span><span class="sxs-lookup"><span data-stu-id="b2514-108">Which browser is set as the default browser?</span></span>
- <span data-ttu-id="b2514-109">Onko sinun käytettävä Internet Exploreria joihinkin sovelluksiin?</span><span class="sxs-lookup"><span data-stu-id="b2514-109">Do you need to use Internet Explorer for some of your apps?</span></span>
- <span data-ttu-id="b2514-110">Käytätkö yritystilasivustoluetteloa Internet Explorerin määrittämiseen jo tänään?</span><span class="sxs-lookup"><span data-stu-id="b2514-110">Do you use an Enterprise Mode Site List to configure Internet Explorer today?</span></span>
- <span data-ttu-id="b2514-111">Mitä käyttöjärjestelmäympäristöjä, kuten Windows 10 ja macOS, tukeeko ympäristösi?</span><span class="sxs-lookup"><span data-stu-id="b2514-111">Which OS platforms, such as Windows 10 and macOS, does your environment support?</span></span>
- <span data-ttu-id="b2514-112">Mitä hallintatyökaluja käytät selaimen hallintaan?</span><span class="sxs-lookup"><span data-stu-id="b2514-112">Which management tools do you use for browser management?</span></span>
- <span data-ttu-id="b2514-113">Kuka vastaa selaimen määrityksestä ja hallinnasta?</span><span class="sxs-lookup"><span data-stu-id="b2514-113">Who's responsible for browser configuration and management?</span></span>
- <span data-ttu-id="b2514-114">Miten selainyhteensopivuus vahvistetaan?</span><span class="sxs-lookup"><span data-stu-id="b2514-114">What's the process for validating browser compatibility?</span></span>
2. <span data-ttu-id="b2514-115">Määritä käyttöönoton tavoitteet.</span><span class="sxs-lookup"><span data-stu-id="b2514-115">Define the goals for your deployment.</span></span> <span data-ttu-id="b2514-116">Pidä seuraavat asiat mielessä:</span><span class="sxs-lookup"><span data-stu-id="b2514-116">Keep the following things in mind:</span></span>
- <span data-ttu-id="b2514-117">Haluatko määrittää [Microsoft Edgen oletusselaimeksi?](https://docs.microsoft.com/DeployEdge/edge-default-browser)</span><span class="sxs-lookup"><span data-stu-id="b2514-117">Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span></span>
- <span data-ttu-id="b2514-118">Haluatko piilottaa Microsoft Edgen vanhan version vai jättää sen [käyttäjien saataville?](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)</span><span class="sxs-lookup"><span data-stu-id="b2514-118">Do you want to hide the legacy version of Microsoft Edge or do you want to [leave it available for users](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span></span>
- <span data-ttu-id="b2514-119">Miten [määrität Microsoft Edgen?](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)</span><span class="sxs-lookup"><span data-stu-id="b2514-119">How will you [configure Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span></span>
- <span data-ttu-id="b2514-120">Mitä ominaisuuksia on erittäin tärkeää määrittää osana ensimmäistä käyttöönottoa?</span><span class="sxs-lookup"><span data-stu-id="b2514-120">What features are critical to configure as part of your initial deployment?</span></span>
- <span data-ttu-id="b2514-121">Mikä on prosessi tunnistettuihin yhteensopivuus- tai määritysongelmiin?</span><span class="sxs-lookup"><span data-stu-id="b2514-121">What is the process for addressing any identified compatibility or configuration issues?</span></span>
3. <span data-ttu-id="b2514-122">Tietoja käyttöedellytysten ymmärtäminen esimerkiksi seuraavista ominaisuuksista:</span><span class="sxs-lookup"><span data-stu-id="b2514-122">Understand the prerequisites for features you might want to use, such as:</span></span>
- [<span data-ttu-id="b2514-123">Windows Defenderin sovellussuoja</span><span class="sxs-lookup"><span data-stu-id="b2514-123">Windows Defender Application Guard</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [<span data-ttu-id="b2514-124">Internet Explorer -tila</span><span class="sxs-lookup"><span data-stu-id="b2514-124">Internet Explorer mode</span></span>](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [<span data-ttu-id="b2514-125">Todennus ja synkronointi</span><span class="sxs-lookup"><span data-stu-id="b2514-125">Authentication and sync</span></span>](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

<span data-ttu-id="b2514-126">Kun olet suorittanut nämä vaiheet, voit aloittaa käyttöönottostrategian suunnittelun.</span><span class="sxs-lookup"><span data-stu-id="b2514-126">After you complete these steps, you're ready to start planning your deployment strategy.</span></span>
