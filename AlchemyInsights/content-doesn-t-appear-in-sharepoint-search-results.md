---
title: Sisältö ei näy SharePoint-hakutuloksissa
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705658"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="688ef-102">Sisältö ei näy SharePoint-hakutuloksissa</span><span class="sxs-lookup"><span data-stu-id="688ef-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="688ef-103">Noudata seuraavia vianmääritysohjeita, kun odotettua sisältöä ei näy hakutuloksissa:</span><span class="sxs-lookup"><span data-stu-id="688ef-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="688ef-104">Tarkista, että **sivuston,** joka sisältää odotetun sisällön, on määritetty sallimaan sisällön näkyminen hakutuloksissa.</span><span class="sxs-lookup"><span data-stu-id="688ef-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="688ef-105">Noudata kohdan [Näytä sivuston sisältö hakutuloksissa olevia](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)ohjeita.</span><span class="sxs-lookup"><span data-stu-id="688ef-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="688ef-106">Tarkista, että odotetun sisällön sisältävä **luettelo** tai **kirjasto** on määritetty sallimaan sisällön näkyminen hakutuloksissa.</span><span class="sxs-lookup"><span data-stu-id="688ef-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="688ef-107">Noudata kohdan [Näytä luetteloiden tai kirjastojen sisältö hakutuloksissa olevia](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)ohjeita.</span><span class="sxs-lookup"><span data-stu-id="688ef-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="688ef-108">Varmista, että sivu, asiakirja tai mukautettu sivun asettelu on julkaistu **pääversiona.**</span><span class="sxs-lookup"><span data-stu-id="688ef-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="688ef-109">Seuraa hakua kohdan Haku vaihetta 3 [ei palauteta kaikkia Tuloksia SharePoint Onlinessa](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="688ef-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="688ef-110">Varmista, että käyttäjällä on **sisällön tarkasteluoikeudet.**</span><span class="sxs-lookup"><span data-stu-id="688ef-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="688ef-111">Noudata tietoja [SharePointin käyttöoikeustasoista](https://docs.microsoft.com/sharepoint/understanding-permission-levels).follow the steps sharePoint .</span><span class="sxs-lookup"><span data-stu-id="688ef-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="688ef-112">Jos hakurakennetta on muutettu lisäämällä uusi hallittu ominaisuus, muokkaamalla hallittua ominaisuutta tai poistamalla hallittu ominaisuus, tarvitaan indeksointia ja uudelleenindeksointia.</span><span class="sxs-lookup"><span data-stu-id="688ef-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="688ef-113">**Indeksoi** sisältö uudelleen noudattamalla kohdan [Sivuston, kirjaston tai luettelon selaamisen ja uudelleenindeksoinnin manuaalinen pyytäminen ohjeita.](https://docs.microsoft.com/sharepoint/crawl-site-content)</span><span class="sxs-lookup"><span data-stu-id="688ef-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="688ef-114">Tämä voi kestää jonkin aikaa, odota 24 tuntia ennen tulosten tarkistamista uudelleen.</span><span class="sxs-lookup"><span data-stu-id="688ef-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="688ef-115">Lisätietoja on [ohjeaiheessa Sivuston sisällön ottaminen käyttöön hakukelpoisina](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="688ef-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
