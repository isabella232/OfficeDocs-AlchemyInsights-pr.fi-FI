---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383832"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="dbea1-102">Tuota odotettuja tuloksia sisällöstä etsiminen</span><span class="sxs-lookup"><span data-stu-id="dbea1-102">Content Search not returning expected results</span></span>

<span data-ttu-id="dbea1-103">Kun sisällön hakujen suorittaminen Office 365: n suojauksen & Compliance Centeriin, näyttöön saattaa tulla odottamaton hakutuloksia.</span><span class="sxs-lookup"><span data-stu-id="dbea1-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="dbea1-104">Ota huomioon seuraavat asiat, jotka vaikuttavat hakutulosten:</span><span class="sxs-lookup"><span data-stu-id="dbea1-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="dbea1-105">**Sisällön sijainnit ja hakuehdot**: Varmista, että olet valinnut oikean sisällön sijainnit ja hakuehdot.</span><span class="sxs-lookup"><span data-stu-id="dbea1-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="dbea1-106">Jos suoritit (useissa paikoissa) suuri etsintä, ota huomioon jakaminen useita hakuja.</span><span class="sxs-lookup"><span data-stu-id="dbea1-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="dbea1-107">**Osittain Indeksoidut kohteet**: arvioidun hakutulosten postilaatikoista [osittain Indeksoidut kohteet](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) sisällytetään.</span><span class="sxs-lookup"><span data-stu-id="dbea1-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="dbea1-108">Kuitenkin osittain indeksoidut objektit sivustojen SharePoint-ja OneDrive eivät sisälly Haku-arvio.</span><span class="sxs-lookup"><span data-stu-id="dbea1-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="dbea1-109">**Etsi virheet**: Kun etsit on paljon (yli 100 000 postilaatikot) postilaatikoita, voit saada Etsi virheet, virhekoodit kuten CS008-009 ja CS012-002).</span><span class="sxs-lookup"><span data-stu-id="dbea1-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="dbea1-110">Tässä tapauksessa yrittää vain epäonnistuneet sisällön sijaintien osalta.</span><span class="sxs-lookup"><span data-stu-id="dbea1-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="dbea1-111">Katso lisätietoja [tämän artikkelin](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="dbea1-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
