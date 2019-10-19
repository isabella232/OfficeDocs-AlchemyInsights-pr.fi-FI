---
title: Vaihda perinteinen pääsivusto modernilla sivustolla
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749257"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="9f848-102">Vaihda perinteinen pääsivusto modernilla sivustolla</span><span class="sxs-lookup"><span data-stu-id="9f848-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="9f848-103">Jos ympäristösi on määritetty ennen huhtikuun 2019, voit muuttaa pääsivuston nykyaikaiseen sivustoon Microsoft PowerShellin avulla:</span><span class="sxs-lookup"><span data-stu-id="9f848-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="9f848-104">Jos sinulla on eri sivusto, jota haluat käyttää pääsivustoosi, voit korvata [(swap) pääsivuston](https://docs.microsoft.com/sharepoint/modern-root-site) sen kanssa.</span><span class="sxs-lookup"><span data-stu-id="9f848-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="9f848-105">Käytä [Kutsu-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , jos haluat vaihtaa sivuston sijainnin toisen sivuston kanssa arkistoitaessa alkuperäistä sivustoa.</span><span class="sxs-lookup"><span data-stu-id="9f848-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="9f848-106">Käytettävissä sekä ryhmäsivustoon (ei yhdistetty ryhmään) että viestintä sivustoon.</span><span class="sxs-lookup"><span data-stu-id="9f848-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="9f848-107">Pian otetaan käyttöön lisä ominaisuuksia, joiden avulla voit jatkaa sivuston sisällön käyttämistä, mutta muuntaa olemassa olevan sivuston viestintä sivustoksi.</span><span class="sxs-lookup"><span data-stu-id="9f848-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="9f848-108">Nämä ominaisuudet otetaan käyttöön vähitellen.</span><span class="sxs-lookup"><span data-stu-id="9f848-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="9f848-109">Jatka Office 365-Message Center-päivitysten tarkistaminen.</span><span class="sxs-lookup"><span data-stu-id="9f848-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="9f848-110">Sivustojen vaihtamisen tunnetut ongelmat</span><span class="sxs-lookup"><span data-stu-id="9f848-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="9f848-111">Kohde sivusto saattaa palauttaa virheen "ei löytynyt" (HTTP 404), joka on lyhyt ajan jakso.</span><span class="sxs-lookup"><span data-stu-id="9f848-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="9f848-112">Sisältö on indeksoida uudelleen, jotta haku indeksi voidaan päivittää.</span><span class="sxs-lookup"><span data-stu-id="9f848-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="9f848-113">Manuaalista vaihetta ei tarvita-tämä tapahtuu automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="9f848-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="9f848-114">Kaikki, jotka ovat riippuvaisia "staattisista" linkeistä (kuten tiedostojen synkronointi ja OneNote-tiedostot), on korjattava manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="9f848-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="9f848-115">Jos lähdesivusto oli organisaation uutisivusto, Päivitä URL-osoite.</span><span class="sxs-lookup"><span data-stu-id="9f848-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="9f848-116">Hanki luettelo kaikista organisaation uutis sivustoista.</span><span class="sxs-lookup"><span data-stu-id="9f848-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="9f848-117">Project Server-sivustot on ehkä validoitava sen varmistamiseksi, että ne liittyvät edelleen oikein.</span><span class="sxs-lookup"><span data-stu-id="9f848-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





