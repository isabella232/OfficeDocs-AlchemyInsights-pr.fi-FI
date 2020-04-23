---
title: SharePoint Onlinen rajoittaminen perinteiseen tilaan
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742466"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="c2041-102">SharePoint Onlinen rajoittaminen perinteiseen tilaan</span><span class="sxs-lookup"><span data-stu-id="c2041-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="c2041-103">Jotkin organisaatiot tarvitsevat edelleen Classic-tilan.</span><span class="sxs-lookup"><span data-stu-id="c2041-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="c2041-104">Vaikka ei ole suunnitelmia poistaa perinteistä tilaa rakeisen tasolla, koko organisaatiota (vuokraajaa) ei voi enää rajoittaa perinteiseen tilaan luetteloita ja kirjastoja varten.</span><span class="sxs-lookup"><span data-stu-id="c2041-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="c2041-105">Admin on seuraavat vaihtoehdot hallita yksittäisiä luetteloita ja kirjastoja klassisessa tilassa käyttämällä rakeinen opt-out kytkimet, että tarjoamme seuraavilla tasoilla:</span><span class="sxs-lookup"><span data-stu-id="c2041-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="c2041-106">sivuston kokoelma</span><span class="sxs-lookup"><span data-stu-id="c2041-106">site collection</span></span>
- <span data-ttu-id="c2041-107">Sivuston</span><span class="sxs-lookup"><span data-stu-id="c2041-107">site</span></span>
- <span data-ttu-id="c2041-108">Luettelo</span><span class="sxs-lookup"><span data-stu-id="c2041-108">list</span></span>
- <span data-ttu-id="c2041-109">Kirjasto</span><span class="sxs-lookup"><span data-stu-id="c2041-109">library</span></span>

<span data-ttu-id="c2041-110">Lisäksi luettelot, jotka käyttävät tiettyjä ominaisuuksia ja mukautuksia, joita moderni ei tue, siirtyvät edelleen automaattisesti perinteiseen tilaan.</span><span class="sxs-lookup"><span data-stu-id="c2041-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="c2041-111">1.4.2019 alkaen prosessi, jossa vuokraajan taso poistetaan käytöstä, ja kirjastot alkavat ja jatkuvat 31.5.2019 asti.</span><span class="sxs-lookup"><span data-stu-id="c2041-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="c2041-112">Luettelot ja kirjastot, jotka ovat perinteisessä tilassa vuokraajan kieltäytymisen seurauksena, siirretään automaattisesti moderniin.</span><span class="sxs-lookup"><span data-stu-id="c2041-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="c2041-113">Jos tarvitset klassista tilaa, katso lisätietoja [täältä](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ja PnP Powershell [-ohje,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) joka kuvaa vaihtoehtoja ja työkaluja, joita voit käyttää tänään perinteisen tilan käyttökokemuksen käyttämiseen.</span><span class="sxs-lookup"><span data-stu-id="c2041-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
