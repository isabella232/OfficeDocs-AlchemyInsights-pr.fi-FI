---
title: Etsi SharePoint Onlinessa
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044040"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="77648-102">Sisällön indeksointi ja indeksointi SharePoint Onlinessa</span><span class="sxs-lookup"><span data-stu-id="77648-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="77648-103">Sisältö on indeksoida ja lisättävä haku indeksiin, jotta käyttäjät löytävät etsimäsi SharePoint Onlinessa.</span><span class="sxs-lookup"><span data-stu-id="77648-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="77648-104">Sisältö indeksoi automaattisesti ennalta määritetyn indeksointi aikataulun perusteella (indeksointi aikataulua ei voi muuttaa).</span><span class="sxs-lookup"><span data-stu-id="77648-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="77648-105">Indeksoija poimii sisällön, joka on muuttunut viimeisimmän indeksoinnin jälkeen, ja päivittää indeksin.</span><span class="sxs-lookup"><span data-stu-id="77648-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="77648-106">Jos haluat varmistaa, että sisältö indeksoida ja indeksi päivitetään, huomioi seuraavat seikat:</span><span class="sxs-lookup"><span data-stu-id="77648-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="77648-107">Varmista, että sisältö löytyy [tekemällä sivuston sisällöstä haettavissa](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="77648-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="77648-108">Kun hallittua ominaisuutta on muutettu tai kun indeksoinnin ja hallittujen ominaisuuksien yhdistämis määrityksiä on muutettu, toimi paikka on indeksoida uudelleen, ennen kuin muutokset näkyvät haku indeksissä.</span><span class="sxs-lookup"><span data-stu-id="77648-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="77648-109">Koska tekemäsi muutokset tehdään etsintä rakenteessa eikä varsi naessa sivustossa, verkkohakuri ei indeksoi sivustoa automaattisesti uudelleen.</span><span class="sxs-lookup"><span data-stu-id="77648-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="77648-110">Lisä tietoja on kohdassa [sivuston, kirjaston tai luettelon indeksoinnin ja uudelleenindeksoinnin pyytäminen manuaalisesti](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="77648-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="77648-111">Odota vähintään 24 tuntia sen jälkeen, kun olet pyytänyt indeksointia ja täyttä uudelleenindeksiä, jotta näet, onko ongelma edelleen.</span><span class="sxs-lookup"><span data-stu-id="77648-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="77648-112">Jos indeksoinnin aloittamisen jälkeen on kulunut yli 24 tuntia ja täydellinen uudelleenindeksi, kirjaudu tuki palvelu pyynnön lokiin.</span><span class="sxs-lookup"><span data-stu-id="77648-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="77648-113">Monissa tapa uksissa olemme jo tekemässä ratkaisua.</span><span class="sxs-lookup"><span data-stu-id="77648-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="77648-114">Ole hyvä ja anna meille vähintään 24 tuntia aikaa ratkaisun suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="77648-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="77648-115">Jos sivusto, asia kirja (Kirjasto) tai luettelo poistettiin ja se näkyy haku tuloksissa, käyttäjien pitäisi saada **virhe 404 tiedostoa ei löydy** yritettäessä käyttää sitä.</span><span class="sxs-lookup"><span data-stu-id="77648-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="77648-116">Tätä kysymystä olisi pidettävä kirjautuneena tuki tapauksena lisä tutkimuksia varten.</span><span class="sxs-lookup"><span data-stu-id="77648-116">This issue should be logged as a support case for further investigation.</span></span> 



