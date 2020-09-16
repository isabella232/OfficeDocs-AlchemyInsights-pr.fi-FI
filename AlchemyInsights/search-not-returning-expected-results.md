---
title: 1491-haku-ei-palautus-odotetut tulokset
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740471"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="ab307-102">Sisältö haku ei palauta odotettuja tuloksia</span><span class="sxs-lookup"><span data-stu-id="ab307-102">Content Search not returning expected results</span></span>

<span data-ttu-id="ab307-103">Kun sisältö haut suoritetaan Microsoft 365-tieto turva & yhteensopivuus keskuksesta, näyttöön voi tulla odottamattomia haku tuloksia.</span><span class="sxs-lookup"><span data-stu-id="ab307-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="ab307-104">Ota huomioon seuraavat asiat, jotka voivat vaikuttaa haku tuloksiin:</span><span class="sxs-lookup"><span data-stu-id="ab307-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="ab307-105">**Sisältö sijainnit ja haku ehdot**: Varmista, että olet valinnut oikeat sisältö sijainnit ja haku ehdot.</span><span class="sxs-lookup"><span data-stu-id="ab307-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="ab307-106">Jos suoritit suuren haun (monissa sijainneissa), harkitse sen jakamista useaan hakuun.</span><span class="sxs-lookup"><span data-stu-id="ab307-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="ab307-107">**Osittain indeksoidut kohteet**:  [osittain indeksoidut kohteet](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) posti laatikoista sisällytetään arvio ituihin haku tuloksiin.</span><span class="sxs-lookup"><span data-stu-id="ab307-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="ab307-108">Kuitenkin osittain indeksoidut kohteet SharePointin ja OneDriven kohteista eivät sisälly haku arvioon.</span><span class="sxs-lookup"><span data-stu-id="ab307-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="ab307-109">**Haku**virheet: kun haet suurta määrää posti laatikoita (yli 100 000 posti laatikkoa), saatat saada haku virheitä, joissa on virhe koodit, kuten CS008-009 ja CS012-002).</span><span class="sxs-lookup"><span data-stu-id="ab307-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="ab307-110">Tässä tapa uksessa yritä hakea vain epäonnistuneista sisältö sijainneista.</span><span class="sxs-lookup"><span data-stu-id="ab307-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="ab307-111">Katso lisä tietoja  [tästä artikkelista](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="ab307-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
