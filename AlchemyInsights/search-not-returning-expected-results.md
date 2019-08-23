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
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 094da9d75013aae56ca219b7ae03e85736ce5ee0
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551412"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="abd33-102">Tuota odotettuja tuloksia sisällöstä etsiminen</span><span class="sxs-lookup"><span data-stu-id="abd33-102">Content Search not returning expected results</span></span>

<span data-ttu-id="abd33-103">Kun sisällön hakujen suorittaminen Office 365: n suojauksen & Compliance Centeriin, näyttöön saattaa tulla odottamaton hakutuloksia.</span><span class="sxs-lookup"><span data-stu-id="abd33-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="abd33-104">Ota huomioon seuraavat asiat, jotka vaikuttavat hakutulosten:</span><span class="sxs-lookup"><span data-stu-id="abd33-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="abd33-105">**Sisällön sijainnit ja hakuehdot**: Varmista, että olet valinnut oikean sisällön sijainnit ja hakuehdot.</span><span class="sxs-lookup"><span data-stu-id="abd33-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="abd33-106">Jos suoritit (useissa paikoissa) suuri etsintä, ota huomioon jakaminen useita hakuja.</span><span class="sxs-lookup"><span data-stu-id="abd33-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="abd33-107">**Osittain Indeksoidut kohteet**: arvioidun hakutulosten postilaatikoista [osittain Indeksoidut kohteet](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) sisällytetään.</span><span class="sxs-lookup"><span data-stu-id="abd33-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="abd33-108">Kuitenkin osittain indeksoidut objektit sivustojen SharePoint-ja OneDrive eivät sisälly Haku-arvio.</span><span class="sxs-lookup"><span data-stu-id="abd33-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="abd33-109">**Etsi virheet**: Kun etsit on paljon (yli 100 000 postilaatikot) postilaatikoita, voit saada Etsi virheet, virhekoodit kuten CS008-009 ja CS012-002).</span><span class="sxs-lookup"><span data-stu-id="abd33-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="abd33-110">Tässä tapauksessa yrittää vain epäonnistuneet sisällön sijaintien osalta.</span><span class="sxs-lookup"><span data-stu-id="abd33-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="abd33-111">Katso lisätietoja [tämän artikkelin](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="abd33-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
