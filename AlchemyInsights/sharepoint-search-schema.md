---
title: SharePoint Online-haun rakenteen hallinta
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f49195bec64f115063ccfb5256e27fbecd4a54f6
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270098"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="542ff-102">SharePoint Online-haun rakenteen hallinta</span><span class="sxs-lookup"><span data-stu-id="542ff-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="542ff-103">Haun rakenteeksi määrittää, mitä käyttäjät voivat etsiä ja miten käyttäjät voivat etsiä siitä miten pystyy esittämään tulokset Etsi WWW-sivustoista.</span><span class="sxs-lookup"><span data-stu-id="542ff-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="542ff-104">[Hallitse SharePoint Online-haun rakenteeksi](https://docs.microsoft.com/sharepoint/manage-search-schema) , saat nähdä miten:</span><span class="sxs-lookup"><span data-stu-id="542ff-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="542ff-105">Muuta haun rakenteeksi.</span><span class="sxs-lookup"><span data-stu-id="542ff-105">Change the search schema.</span></span>
- <span data-ttu-id="542ff-106">Hallittujen ominaisuuksien luominen</span><span class="sxs-lookup"><span data-stu-id="542ff-106">Create managed properties.</span></span>
- <span data-ttu-id="542ff-107">Tietokartan selattu selattuja ominaisuuksia hallittuihin ominaisuuksiin.</span><span class="sxs-lookup"><span data-stu-id="542ff-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="542ff-108">Haun rakenteen hallinta tilaamassa seuraavat seikat:</span><span class="sxs-lookup"><span data-stu-id="542ff-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="542ff-109">Jos näyttöön tulee varoitus ilmoittaa **sovellus on keskeytetty** tehdessään rakenteen muuttaminen, tämä on vain tilapäinen palvelun ylläpito on esiintyvä.</span><span class="sxs-lookup"><span data-stu-id="542ff-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="542ff-110">Jos kohtaat edelleen varoitus yli 24 tuntia on kulunut, kirjaudu tukipyynnön.</span><span class="sxs-lookup"><span data-stu-id="542ff-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="542ff-111">Kun muutat hallittuja ominaisuuksia tai lisätä uusia, muutokset tulevat voimaan vasta, kun on uudelleen selattu sisältö.</span><span class="sxs-lookup"><span data-stu-id="542ff-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="542ff-112">SharePoint Online-indeksointi tapahtuu automaattisesti määritetyn indeksoinnin aikataulun mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="542ff-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="542ff-113">Varmista, että muutokset selataan, erityisesti [pyyntöä indeksoidaan uudelleen luettelon tai kirjaston](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) voi</span><span class="sxs-lookup"><span data-stu-id="542ff-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="542ff-114">Katso [Esittely haun rakenteen](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/) yleiskatsaus haun rakenteeksi,</span><span class="sxs-lookup"><span data-stu-id="542ff-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


