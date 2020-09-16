---
title: Haku rakenteen hallinta SharePoint Onlinessa
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770548"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="104a3-102">Haku rakenteen hallinta SharePoint Onlinessa</span><span class="sxs-lookup"><span data-stu-id="104a3-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="104a3-103">Haku rakenne määrittää, mitä käyttäjät voivat etsiä, miten käyttäjät voivat hakea sitä ja miten voit esittää tulokset haku sivustoissa.</span><span class="sxs-lookup"><span data-stu-id="104a3-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="104a3-104">Lisä tietoja on artikkelissa [haku rakenteen hallinta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/manage-search-schema) :</span><span class="sxs-lookup"><span data-stu-id="104a3-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="104a3-105">Muuta haku rakennetta.</span><span class="sxs-lookup"><span data-stu-id="104a3-105">Change the search schema.</span></span>
- <span data-ttu-id="104a3-106">Luo hallitut ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="104a3-106">Create managed properties.</span></span>
- <span data-ttu-id="104a3-107">Yhdistä selattujen karttojen indeksoidut ominaisuudet hallittuihin ominaisuuksiin.</span><span class="sxs-lookup"><span data-stu-id="104a3-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="104a3-108">Huomaa seuraavat asiat, jotka koskevat haku rakenteen hallintaa:</span><span class="sxs-lookup"><span data-stu-id="104a3-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="104a3-109">Jos näyttöön tulee varoitus, jossa ilmoitetaan, **että sovellus on keskeytetty** , kun rakenne muuttuu, tämä on vain väliaikaista, koska palvelun ylläpito tapahtuu.</span><span class="sxs-lookup"><span data-stu-id="104a3-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="104a3-110">Jos yli 24 tuntia on kulunut ja varoitus tulee edelleen näkyviin, kirjaudu tuki pyyntöön.</span><span class="sxs-lookup"><span data-stu-id="104a3-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="104a3-111">Kun muutat hallittuja ominaisuuksia tai lisäät uusia, muutokset tulevat voimaan vasta, kun sisältö on indeksoitu uudelleen.</span><span class="sxs-lookup"><span data-stu-id="104a3-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="104a3-112">SharePoint Onlinessa selaaminen tapahtuu automaattisesti määritetyn indeksointi aikataulun perusteella.</span><span class="sxs-lookup"><span data-stu-id="104a3-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="104a3-113">Jos haluat varmistaa, että muutokset indeksoidaan, voit erityisesti [pyytää luettelon tai kirjaston uudelleenindeksointia](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) .</span><span class="sxs-lookup"><span data-stu-id="104a3-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="104a3-114">Täydellinen yleiskatsaus haku rakenteeseen on Ohje aiheessa [haku rakenteen esittely](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="104a3-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


