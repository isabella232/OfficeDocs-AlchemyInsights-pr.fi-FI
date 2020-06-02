---
title: 1491-haku-ei-palaa-odotettu-tulokset
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510569"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="d0e46-102">Sisältöhaku ei palauta odotettuja tuloksia</span><span class="sxs-lookup"><span data-stu-id="d0e46-102">Content Search not returning expected results</span></span>

<span data-ttu-id="d0e46-103">Kun suoritat sisältöhakuja Microsoft 365:n tietoturva- & Compliance Centeristä, saatat saada odottamattomia hakutuloksia.</span><span class="sxs-lookup"><span data-stu-id="d0e46-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="d0e46-104">Mieti seuraavia asioita, jotka voivat vaikuttaa hakutuloksiin:</span><span class="sxs-lookup"><span data-stu-id="d0e46-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="d0e46-105">**Sisältösijainnit ja hakuehdot**: Varmista, että olet valinnut oikeat sisältösijainnit ja hakuehdot.</span><span class="sxs-lookup"><span data-stu-id="d0e46-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="d0e46-106">Jos teit suuren haun (jossa on useita sijainteja), harkitse sen jakamista useisiin hakuihin.</span><span class="sxs-lookup"><span data-stu-id="d0e46-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="d0e46-107">**Osittain indeksoidut kohteet:** Postilaatikoiden [osittain indeksoidut kohteet](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) sisältyvät arvioituihin hakutuloksiin.</span><span class="sxs-lookup"><span data-stu-id="d0e46-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="d0e46-108">SharePointin ja OneDriven sivustojen osittain indeksoidut kohteet eivät kuitenkaan sisälly hakuarvioon.</span><span class="sxs-lookup"><span data-stu-id="d0e46-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="d0e46-109">**Hakuvirheet**: Kun etsit suurta määrää postilaatikoita (yli 100 000 postilaatikkoa), saatat saada hakuvirheitä virhekoodeilla, kuten CS008-009 ja CS012-002).</span><span class="sxs-lookup"><span data-stu-id="d0e46-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="d0e46-110">Yritä tässä tapauksessa etsiä vain epäonnistuneita sisältösijainteja uudelleen.</span><span class="sxs-lookup"><span data-stu-id="d0e46-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="d0e46-111">Lisätietoja [on tässä artikkelissa.](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)</span><span class="sxs-lookup"><span data-stu-id="d0e46-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
