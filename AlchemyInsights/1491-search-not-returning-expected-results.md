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
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964851"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="617b9-102">Tuota odotettuja tuloksia sisällöstä etsiminen</span><span class="sxs-lookup"><span data-stu-id="617b9-102">Content Search not returning expected results</span></span>

<span data-ttu-id="617b9-p101">Kun sisällön hakujen suorittaminen Office 365: n suojauksen & Compliance Centeriin, näyttöön saattaa tulla odottamaton hakutuloksia. Ota huomioon seuraavat asiat, jotka vaikuttavat hakutulosten:</span><span class="sxs-lookup"><span data-stu-id="617b9-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="617b9-p102">**Sisällön sijainnit ja hakuehdot**: Varmista, että olet valinnut oikean sisällön sijainnit ja hakuehdot. Jos suoritit (useissa paikoissa) suuri etsintä, ota huomioon jakaminen useita hakuja.</span><span class="sxs-lookup"><span data-stu-id="617b9-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="617b9-p103">**Osittain Indeksoidut kohteet**: arvioidun hakutulosten postilaatikoista [osittain Indeksoidut kohteet](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) sisällytetään. Kuitenkin osittain indeksoidut objektit sivustojen SharePoint-ja OneDrive eivät sisälly Haku-arvio.</span><span class="sxs-lookup"><span data-stu-id="617b9-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="617b9-p104">**Etsi virheet**: Kun etsit on paljon (yli 100 000 postilaatikot) postilaatikoita, voit saada Etsi virheet, virhekoodit kuten CS008-009 ja CS012-002). Tässä tapauksessa yrittää vain epäonnistuneet sisällön sijaintien osalta. Katso lisätietoja [tämän artikkelin](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="617b9-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
