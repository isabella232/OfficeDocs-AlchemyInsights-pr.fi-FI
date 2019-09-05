---
title: Rajoita SharePoint Onlinea Classic-tilaan
ms.author: pebaum
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752065"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="cf9ce-102">Rajoita SharePoint Onlinea Classic-tilaan</span><span class="sxs-lookup"><span data-stu-id="cf9ce-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="cf9ce-103">Jotkin organisaatiot vaativat silti perinteisen tilan käyttö kokemuksen.</span><span class="sxs-lookup"><span data-stu-id="cf9ce-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="cf9ce-104">Vaikka perinteisen tilan poistamista ei ole suunnitelmia rakeisen tason avulla, koko organisaatiota (vuokraajaa) ei voi enää rajoittaa luetteloiden ja kirjastojen klassiseen tilaan.</span><span class="sxs-lookup"><span data-stu-id="cf9ce-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="cf9ce-105">Järjestelmänvalvojalle on seuraavat vaihto ehdot hallita yksittäisiä luetteloita ja kirjastoja klassisessa tilassa käyttämällä rakeisia opt-out-kytkimiä, joita tarjoamme seuraavilla tasoilla:</span><span class="sxs-lookup"><span data-stu-id="cf9ce-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="cf9ce-106">sivustokokoelman</span><span class="sxs-lookup"><span data-stu-id="cf9ce-106">site collection</span></span>
- <span data-ttu-id="cf9ce-107">Sivuston</span><span class="sxs-lookup"><span data-stu-id="cf9ce-107">site</span></span>
- <span data-ttu-id="cf9ce-108">Luettelo</span><span class="sxs-lookup"><span data-stu-id="cf9ce-108">list</span></span>
- <span data-ttu-id="cf9ce-109">Kirjasto</span><span class="sxs-lookup"><span data-stu-id="cf9ce-109">library</span></span>

<span data-ttu-id="cf9ce-110">Lisäksi luettelot, jotka käyttävät tiettyjä ominaisuuksia ja mukautuksia, joita Modern ei tue, ovat edelleen automaattisesti klassisessa tilassa.</span><span class="sxs-lookup"><span data-stu-id="cf9ce-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="cf9ce-111">Huhtikuun alussa 1, 2019, prosessi poistaa vuokralaisen tason opt pois modernin luettelon ja kirjastot käynnistyy ja jatkuu läpi toukokuun 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="cf9ce-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="cf9ce-112">Luettelot ja kirjastot, jotka ovat klassisessa tilassa vuokralaisen opt-out-järjestelyn seura uksena, siirtyvät automaattisesti moderniin.</span><span class="sxs-lookup"><span data-stu-id="cf9ce-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="cf9ce-113">Jos tarvitset klassista tilaa, Katso lisä tietoja [tästä](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ja PnP PowerShell-ohjeet [täältä](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , jossa kerrotaan vaihto ehdoista ja työkaluista, joita voit käyttää tänään klassisen tilan käyttö kokemuksen käyttämistä varten.</span><span class="sxs-lookup"><span data-stu-id="cf9ce-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
