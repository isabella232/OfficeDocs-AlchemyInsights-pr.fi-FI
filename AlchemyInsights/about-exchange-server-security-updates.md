---
title: Tietoja Exchange Serverin suojauspäivityksistä
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481392"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="6522b-102">Tietoja Exchange Serverin suojauspäivityksistä</span><span class="sxs-lookup"><span data-stu-id="6522b-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="6522b-103">Microsoft on julkaissut joukon tärkeitä suojauspäivityksiä paikallisiin Exchange Serveriin.</span><span class="sxs-lookup"><span data-stu-id="6522b-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="6522b-104">Nämä palvelinversiot ovat Exchange Server 2010:n, 2013:n, 2016:n ja 2019:n päivitystasoja.</span><span class="sxs-lookup"><span data-stu-id="6522b-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="6522b-105">Tämä ei vaikuta Exchange Onlineen, mutta jos sinulla on joitakin paikallisia Exchange-palvelimia yhdistelmäkokoonpanon vuoksi, ne voivat olla haavoittuvia.</span><span class="sxs-lookup"><span data-stu-id="6522b-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="6522b-106">Jotta voit päivittää paikallisen palvelimen, käytössä on oltava vähintään seuraavat Exchange-versiot:</span><span class="sxs-lookup"><span data-stu-id="6522b-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="6522b-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="6522b-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="6522b-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="6522b-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="6522b-109">Exchange Server 2016 CU 19 tai CU 18</span><span class="sxs-lookup"><span data-stu-id="6522b-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="6522b-110">Exchange Server 2019 CU 8 tai CU 7</span><span class="sxs-lookup"><span data-stu-id="6522b-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="6522b-111">Katso korjausten sijaintitiedot seuraavasta [ilmoituksesta: Julkaistu: Maaliskuun 2021 Exchange Serverin suojauspäivitykset](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="6522b-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="6522b-112">**Tärkeitä huomautuksia:**</span><span class="sxs-lookup"><span data-stu-id="6522b-112">**Important notes:**</span></span>

<span data-ttu-id="6522b-113">Päivitysten asentaminen ei toimi, jos paikallisissa palvelimissa ei ole käytössä vaadittuja Exchange-versioita yllä olevassa luettelossa.</span><span class="sxs-lookup"><span data-stu-id="6522b-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="6522b-114">Jos asennat päivitykset manuaalisesti, lue tärkeitä tietoja päivitysten KB-artikkeleiden Tunnetut ongelmat -osasta.</span><span class="sxs-lookup"><span data-stu-id="6522b-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="6522b-115">Suojauspäivitykset ON suoritettava järjestelmänvalvojana suoritettavasta CMD-/PowerShell-kehotteesta.</span><span class="sxs-lookup"><span data-stu-id="6522b-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
