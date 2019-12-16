---
title: Hallitse haku rakennetta SharePoint Onlinessa
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042960"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="fa7bf-102">Hallitse haku rakennetta SharePoint Onlinessa</span><span class="sxs-lookup"><span data-stu-id="fa7bf-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="fa7bf-103">Haku rakenne ohjaa sitä, mitä käyttäjät voivat etsiä, miten käyttäjät voivat etsiä tietoja ja miten voit esittää tulokset haku sivustoilla.</span><span class="sxs-lookup"><span data-stu-id="fa7bf-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="fa7bf-104">Lisä tietoja on Ohje aiheessa [SharePoint Onlinen haku mallin hallinta](https://docs.microsoft.com/sharepoint/manage-search-schema) :</span><span class="sxs-lookup"><span data-stu-id="fa7bf-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="fa7bf-105">Muuta etsintä rakennetta.</span><span class="sxs-lookup"><span data-stu-id="fa7bf-105">Change the search schema.</span></span>
- <span data-ttu-id="fa7bf-106">Luo hallitut ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="fa7bf-106">Create managed properties.</span></span>
- <span data-ttu-id="fa7bf-107">Map selatun kartan indeksi ominaisuudet hallitut ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="fa7bf-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="fa7bf-108">Huomaa seuraavat seikat, jotka koskevat haku mallin hallintaa:</span><span class="sxs-lookup"><span data-stu-id="fa7bf-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="fa7bf-109">Jos saat varoituksen, jossa ilmoitetaan, **että sovellus on keskeytetty** , kun teet rakenteen muutoksen, tämä on vain väliaikaista, koska palvelun ylläpito tapahtuu.</span><span class="sxs-lookup"><span data-stu-id="fa7bf-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="fa7bf-110">Jos yli 24 tuntia on kulunut ja sinulla on edelleen varoitus, ole hyvä ja kirjaa tuki palvelu pyynnön.</span><span class="sxs-lookup"><span data-stu-id="fa7bf-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="fa7bf-111">Kun hallittuja ominaisuuksia muutetaan tai uusia lisätään, muutokset tulevat voimaan vasta, kun sisältö on indeksoitu uudelleen.</span><span class="sxs-lookup"><span data-stu-id="fa7bf-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="fa7bf-112">SharePoint Onlinessa indeksoinnin tapahtuu automaattisesti määritetyn indeksointi aikataulun perusteella.</span><span class="sxs-lookup"><span data-stu-id="fa7bf-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="fa7bf-113">Jos haluat varmistaa, että tekemäsi muutokset indeksoidaan, voit pyytää erityisesti [luettelon tai kirjaston uudelleenindeksointia.](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="fa7bf-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="fa7bf-114">Täydellinen yleiskuva haku mallista on kohdassa [haku mallin esittely](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="fa7bf-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


