---
title: SharePoint Onlinen rajoittaminen perinteiseen tilaan
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751419"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="841df-102">SharePoint Onlinen rajoittaminen perinteiseen tilaan</span><span class="sxs-lookup"><span data-stu-id="841df-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="841df-103">Jotkin organisaatiot vaativat edelleen perinteisen tilan käyttö kokemusta.</span><span class="sxs-lookup"><span data-stu-id="841df-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="841df-104">Vaikka perinteistä tilaa ei ole tarkoitus poistaa rakeisella tasolla, koko organisaatiota (vuokraaja) ei voi enää rajoittaa luetteloiden ja kirjastojen perinteiseen tilaan.</span><span class="sxs-lookup"><span data-stu-id="841df-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="841df-105">Järjestelmänvalvojalla on seuraavat asetukset, joilla hallitaan yksittäisiä luetteloita ja kirjastoja perinteisessä tilassa käyttämällä rakeisia kieltäytymis valitsimia, jotka tarjoamme seuraavilla tasoilla:</span><span class="sxs-lookup"><span data-stu-id="841df-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="841df-106">sivustokokoelma</span><span class="sxs-lookup"><span data-stu-id="841df-106">site collection</span></span>
- <span data-ttu-id="841df-107">sivuston</span><span class="sxs-lookup"><span data-stu-id="841df-107">site</span></span>
- <span data-ttu-id="841df-108">luettelo</span><span class="sxs-lookup"><span data-stu-id="841df-108">list</span></span>
- <span data-ttu-id="841df-109">kirjaston</span><span class="sxs-lookup"><span data-stu-id="841df-109">library</span></span>

<span data-ttu-id="841df-110">Lisäksi luettelot, jotka käyttävät tiettyjä ominaisuuksia ja mukautuksia, joita moderni ei tue, kytketään automaattisesti perinteiseen tilaan.</span><span class="sxs-lookup"><span data-stu-id="841df-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="841df-111">1. huhtikuuta 2019 lähtien prosessi, joka poistaa vuokra ajan tason jättäytymisen pois modernista luettelosta ja kirjastot alkavat ja jatkuvat 31. toukokuuta 2019.</span><span class="sxs-lookup"><span data-stu-id="841df-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="841df-112">Luettelot ja kirjastot, jotka ovat perinteisessä tilassa vuokra ajan käytöstä poisjäämisen seura uksena, siirtyvät automaattisesti moderniin.</span><span class="sxs-lookup"><span data-stu-id="841df-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="841df-113">Jos tarvitset perinteistä tilaa, Katso lisä tietoja [täältä](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ja PnP-PowerShell [-Ohje,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) jossa kerrotaan vaihto ehdoista ja työkaluista, joilla voit käyttää perinteistä tila kokemusta.</span><span class="sxs-lookup"><span data-stu-id="841df-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
