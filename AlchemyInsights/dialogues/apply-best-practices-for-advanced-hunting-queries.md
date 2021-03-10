---
title: Parhaiden käytäntöjen käyttäminen edistyneissä hakukyselyissä
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694275"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="fd872-102">Parhaiden käytäntöjen käyttäminen edistyneissä hakukyselyissä</span><span class="sxs-lookup"><span data-stu-id="fd872-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="fd872-103">Jos haluat saada tulokset nopeammin ja välttää aikakatkaisut monimutkaisia kyselyjä suorittamalla, käytä seuraavia parhaita käytäntöjä:</span><span class="sxs-lookup"><span data-stu-id="fd872-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="fd872-104">Kun yrität uusia kyselyjä, käytä aina rajaa, jotta et saa erittäin suuria tulosjoukkoja.</span><span class="sxs-lookup"><span data-stu-id="fd872-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="fd872-105">Käytä myös tulosjoukon koon `count` alkuarviointia.</span><span class="sxs-lookup"><span data-stu-id="fd872-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="fd872-106">Käytä ensin aikasuodattimia.</span><span class="sxs-lookup"><span data-stu-id="fd872-106">Use time filters first.</span></span> <span data-ttu-id="fd872-107">Ihanne parasta, rajaa kyselyt seitsemään päivään.</span><span class="sxs-lookup"><span data-stu-id="fd872-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="fd872-108">Lisää kyselyn alkuun heti aikasuodattimen jälkeen suodattimet, jotka todennäköisesti poistavat suurimman osan tiedoista.</span><span class="sxs-lookup"><span data-stu-id="fd872-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="fd872-109">Kun etsit täysiä tunnuksia, käytä `has` operaattoria sen sijaan, että `contains` etsisit kokonaisia tunnuksia.</span><span class="sxs-lookup"><span data-stu-id="fd872-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="fd872-110">Suorita haku tietyssä sarakkeessa kaikkien sarakkeiden sijaan.</span><span class="sxs-lookup"><span data-stu-id="fd872-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="fd872-111">Kun liität taulukoita, määritä ensin taulukko, jossa on vähemmän rivejä.</span><span class="sxs-lookup"><span data-stu-id="fd872-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="fd872-112">`project` vain tarvittavat sarakkeet taulukoista, jotka olet yhdistänyt.</span><span class="sxs-lookup"><span data-stu-id="fd872-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="fd872-113">Lisätietoja on ohjeaiheessa Edistyneet [hakukyselyn parhaat käytännöt.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="fd872-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
