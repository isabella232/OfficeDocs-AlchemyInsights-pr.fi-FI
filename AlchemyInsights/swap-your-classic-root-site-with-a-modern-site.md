---
title: Perinteisen pääsivuston vaihtaminen modernilla sivustolla
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691176"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="184f4-102">Perinteisen pääsivuston vaihtaminen modernilla sivustolla</span><span class="sxs-lookup"><span data-stu-id="184f4-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="184f4-103">Jos ympäristösi on määritetty ennen huhtikuun 2019, voit vaihtaa pääsivuston moderniin sivustoon Microsoft PowerShellin avulla:</span><span class="sxs-lookup"><span data-stu-id="184f4-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="184f4-104">Jos sinulla on jokin muu sivusto, jota haluat käyttää pääsivustona, voit vaihtaa [pääsivustoa](https://docs.microsoft.com/sharepoint/modern-root-site) sen kanssa.</span><span class="sxs-lookup"><span data-stu-id="184f4-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="184f4-105">Käytä [Invoke-SPOSiteSwap-](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) vaihto pistettä, jos haluat vaihtaa sivuston sijainnin toiseen sivustoon arkistoitaessa alkuperäistä sivustoa.</span><span class="sxs-lookup"><span data-stu-id="184f4-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="184f4-106">Saatavilla sekä Ryhmäsivustolle (ei yhdistetty ryhmään) että Viestintäsivustoon.</span><span class="sxs-lookup"><span data-stu-id="184f4-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="184f4-107">Saat pian käyttöön lisä ominaisuuksia, joiden avulla voit jatkaa sivuston sisällön käyttöä, mutta muuntaa aiemmin luodun sivuston viestintä sivustoksi.</span><span class="sxs-lookup"><span data-stu-id="184f4-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="184f4-108">Nämä ominaisuudet otetaan käyttöön asteittain.</span><span class="sxs-lookup"><span data-stu-id="184f4-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="184f4-109">Jatka Tarkista viesti keskus päivitysten varalta.</span><span class="sxs-lookup"><span data-stu-id="184f4-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="184f4-110">Sivuston vaihtamisen tunnetut ongelmat</span><span class="sxs-lookup"><span data-stu-id="184f4-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="184f4-111">Kohdesivusto voi palauttaa lyhyen ajan "not found" (HTTP 404)-virheen.</span><span class="sxs-lookup"><span data-stu-id="184f4-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="184f4-112">Sisältö on määritettävä uudelleen, jotta haku indeksiä voi päivittää.</span><span class="sxs-lookup"><span data-stu-id="184f4-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="184f4-113">Manuaalista vaihetta ei tarvita-tämä tapahtuu automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="184f4-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="184f4-114">Kaikki staattisista linkeistä riippuvat (kuten tiedostojen synkronointi ja OneNote-tiedostot) on korjattava manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="184f4-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="184f4-115">Jos lähdesivusto oli organisaation uutissivusto, Päivitä URL-osoite.</span><span class="sxs-lookup"><span data-stu-id="184f4-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="184f4-116">Saat luettelon kaikista organisaation uutis sivuista.</span><span class="sxs-lookup"><span data-stu-id="184f4-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="184f4-117">Project Server-sivustot on ehkä vahvistettava sen varmistamiseksi, että ne liitetään edelleen oikein.</span><span class="sxs-lookup"><span data-stu-id="184f4-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
