---
title: Sisältö ei näy SharePoint-haku tuloksissa
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713127"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="10d89-102">Sisältö ei näy SharePoint-haku tuloksissa</span><span class="sxs-lookup"><span data-stu-id="10d89-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="10d89-103">Noudata näitä vian määritys vaiheita, kun oletettua sisältöä ei näy haku tuloksissa:</span><span class="sxs-lookup"><span data-stu-id="10d89-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="10d89-104">Tarkista, että **sivuston** , joka sisältää oletetun sisällön, asetuksena on sallia sisällön näkyvän haku tuloksissa.</span><span class="sxs-lookup"><span data-stu-id="10d89-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="10d89-105">Noudata artikkelissa [sivuston sisällön näyttäminen haku tuloksissa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)annettuja ohjeita.</span><span class="sxs-lookup"><span data-stu-id="10d89-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="10d89-106">Tarkista, että oletetun sisällön sisältävä **luettelo** tai **Kirjasto** on valittu sallimaan sisällön näkymisen haku tuloksissa.</span><span class="sxs-lookup"><span data-stu-id="10d89-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="10d89-107">Noudata ohjeita kohdassa [sisällön näyttäminen luetteloista tai kirjastoista haku tuloksissa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="10d89-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="10d89-108">Varmista, että sivun, asia kirjan tai mukautetun sivun asettelu on julkaistu **pääversiona.**</span><span class="sxs-lookup"><span data-stu-id="10d89-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="10d89-109">Seuraa vaihetta 3 [haku ei palauta kaikkia tuloksia SharePoint Onlinessa](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="10d89-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="10d89-110">Varmista, että käyttäjällä on **oikeus** tarkastella sisältöä.</span><span class="sxs-lookup"><span data-stu-id="10d89-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="10d89-111">Noudata artikkelissa [SharePointin käyttö oikeus tasojen ymmärtäminen](https://docs.microsoft.com/sharepoint/understanding-permission-levels)annettuja ohjeita.</span><span class="sxs-lookup"><span data-stu-id="10d89-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="10d89-112">Jos haku rakennetta on muutettu lisäämällä uusi hallittu ominaisuus muokkaamalla hallittua ominaisuutta tai poistamalla hallittu ominaisuus, sinun on pyydettävä indeksointia ja uudelleenindeksiä.</span><span class="sxs-lookup"><span data-stu-id="10d89-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="10d89-113">**Indeksoi sisältö uudelleen** noudattamalla ohjeita, jotka koskevat [sivuston, kirjaston tai luettelon indeksoimisen manuaalista selaamista ja uudelleenindeksointia](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="10d89-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="10d89-114">Tämä voi kestää hetken, odota 24 tuntia, ennen kuin tarkistat tulokset uudelleen.</span><span class="sxs-lookup"><span data-stu-id="10d89-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="10d89-115">Lisä tietoja on kohdassa [sivuston sisällön ottaminen käyttöön haettavaksi](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="10d89-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
