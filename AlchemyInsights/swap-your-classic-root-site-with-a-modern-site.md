---
title: Vaihda Classic juuri sivuston modernin sivuston
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741541"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="b2a36-102">Vaihda Classic juuri sivuston modernin sivuston</span><span class="sxs-lookup"><span data-stu-id="b2a36-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="b2a36-103">Jos ympäristöon määritetty ennen huhtikuuta 2019, voit muuttaa pääsivuston moderniksi sivustoksi Microsoft PowerShellin avulla:</span><span class="sxs-lookup"><span data-stu-id="b2a36-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="b2a36-104">Jos sinulla on eri sivusto, jota haluat käyttää pääsivustona, voit korvata [(vaihtaa) juurisivuston](https://docs.microsoft.com/sharepoint/modern-root-site) sillä.</span><span class="sxs-lookup"><span data-stu-id="b2a36-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="b2a36-105">[Käytä Invoke-SPOSiteSwapia](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) sivuston sijainnin vaihtamiseen toisen sivuston kanssa alkuperäisen sivuston arkistoimisen aikana.</span><span class="sxs-lookup"><span data-stu-id="b2a36-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="b2a36-106">Käytettävissä sekä ryhmäsivustossa (ei yhdistettynä ryhmään) että viestintäsivustossa.</span><span class="sxs-lookup"><span data-stu-id="b2a36-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="b2a36-107">Pian otetaan käyttöön lisäominaisuuksia, joiden avulla voit jatkaa sivuston sisällön käyttämistä, mutta muuntaa aiemmin luodun sivuston viestintäsivustoksi.</span><span class="sxs-lookup"><span data-stu-id="b2a36-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="b2a36-108">Nämä ominaisuudet otetaan käyttöön vähitellen.</span><span class="sxs-lookup"><span data-stu-id="b2a36-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="b2a36-109">Jatka päivitysten tarkistamista Viestikeskuksesta.</span><span class="sxs-lookup"><span data-stu-id="b2a36-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="b2a36-110">Sivustojen vaihtamisen tunnetut ongelmat</span><span class="sxs-lookup"><span data-stu-id="b2a36-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="b2a36-111">Kohdesivusto saattaa palauttaa http 404 (ei löydy) -virheen lyhyeksi ajaksi.</span><span class="sxs-lookup"><span data-stu-id="b2a36-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="b2a36-112">Hakuindeksin päivittäminen edellyttää sisällön indeksointia uudelleen.</span><span class="sxs-lookup"><span data-stu-id="b2a36-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="b2a36-113">Manuaalista vaihetta ei tarvita - tämä tehdään automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="b2a36-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="b2a36-114">Kaikki staattisesta linkistä riippuvaiset linkit (kuten Tiedostojen synkronointi ja OneNote-tiedostot) on korjattava manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="b2a36-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="b2a36-115">Jos lähdesivusto oli organisaation uutissivusto, päivitä URL-osoite.</span><span class="sxs-lookup"><span data-stu-id="b2a36-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="b2a36-116">Saat luettelon kaikista organisaation uutissivustoista.</span><span class="sxs-lookup"><span data-stu-id="b2a36-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="b2a36-117">Project Server -sivustot on ehkä vahvistettava, jotta ne voidaan edelleen liittää oikein.</span><span class="sxs-lookup"><span data-stu-id="b2a36-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
