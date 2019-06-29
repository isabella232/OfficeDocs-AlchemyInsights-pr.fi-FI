---
title: Sisältö ei näy hakutuloksissa SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363800"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="6f804-102">Sisältö ei näy hakutuloksissa SharePoint</span><span class="sxs-lookup"><span data-stu-id="6f804-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="6f804-103">Suorita seuraavat vianmääritysvaiheet, kun odotettu sisältö ei näy etsinnän tuloksissa:</span><span class="sxs-lookup"><span data-stu-id="6f804-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="6f804-104">Tarkista, että odotettua sisältöä sisältävä **sivusto** on määritetty sallimaan sisällön näkyvän etsinnän tuloksissa.</span><span class="sxs-lookup"><span data-stu-id="6f804-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="6f804-105">Noudata [Näytä sisältöä sivuston hakutuloksissa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="6f804-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="6f804-106">Tarkista, että **luettelo** tai **kirjasto** , joka sisältää odotettu sisältö on sisällön näkyvän etsinnän tuloksissa.</span><span class="sxs-lookup"><span data-stu-id="6f804-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="6f804-107">Noudata [Näytä sisältöä luetteloiden tai kirjastojen hakutuloksissa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="6f804-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="6f804-108">Varmista, että sivun, tiedoston tai mukautetun sivun asettelu julkaistaan **pääversio.**</span><span class="sxs-lookup"><span data-stu-id="6f804-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="6f804-109">Vaiheen 3- [haku ei palauta kaikkia tuloksia SharePoint Onlinessa](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="6f804-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="6f804-110">Varmista, että käyttäjällä on **oikeudet** tarkastella sisältöä.</span><span class="sxs-lookup"><span data-stu-id="6f804-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="6f804-111">Ohjeiden [ymmärtäminen käyttöoikeustasoja SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="6f804-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="6f804-112">Jos haku rakennetta on muutettu lisäämällä uusi hallittu ominaisuus, hallitun ominaisuuden muokkaamalla tai poistamalla sitten pyytää hallitun ominaisuuden indeksointi ja indeksoida uudelleen vaaditaan.</span><span class="sxs-lookup"><span data-stu-id="6f804-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="6f804-113">**Indeksoi** sisältö [manuaalisesti pyytää Läpikäymiselle ja indeksoinnille uudelleen sivuston kirjasto tai luettelo](https://docs.microsoft.com/sharepoint/crawl-site-content)-ohjeiden mukaan.</span><span class="sxs-lookup"><span data-stu-id="6f804-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="6f804-114">Tämä saattaa kestää jonkin aikaa, odota 24 tuntia, ennen kuin tarkistat tulokset uudelleen.</span><span class="sxs-lookup"><span data-stu-id="6f804-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="6f804-115">Lisätietoja [voi etsiä tietoja sivuston sisällön käyttöön](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="6f804-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
