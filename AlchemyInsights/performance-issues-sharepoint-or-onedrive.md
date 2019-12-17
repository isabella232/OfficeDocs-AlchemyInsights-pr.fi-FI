---
title: Suorituskyky ongelmat-SharePoint tai OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068396"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="c471f-102">SharePoint tai OneDrive hidas, ei käytettävissä tai ei saatavilla useille käyttäjille</span><span class="sxs-lookup"><span data-stu-id="c471f-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="c471f-103">SharePoint tai OneDrive voi olla hidas, ei käytettävissä tai se ei ole saatavilla, tai se saattaa näyttää palvelun poissa käytöstä tai 503 virhettä useista syistä:</span><span class="sxs-lookup"><span data-stu-id="c471f-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="c471f-104">Jos SharePoint-tai OneDrive-sivustosi on hidas tai viivästynyt useille käyttäjille, saattaa olla tilapäinen palvelu ongelma, jossa käyttäjät kokevat ajoittaisia viiveitä tai siirtymis virheitä SharePoint-sivustoja tai OneDrive-sisältöä käytettäessä.</span><span class="sxs-lookup"><span data-stu-id="c471f-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="c471f-105">Tarkista [palvelun kunnon koonti näytöstä](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , onko organisaatiossasi vaikutusta.</span><span class="sxs-lookup"><span data-stu-id="c471f-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="c471f-106">Käyttäjät saattavat saada *503-palvelimen, on varattu* -virhe yritettäessä siirtyä SharePoint-tai OneDrive-sivustoihin.</span><span class="sxs-lookup"><span data-stu-id="c471f-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="c471f-107">Tämä virhe voi johtua rajoittamalla SharePoint-palvelussa.</span><span class="sxs-lookup"><span data-stu-id="c471f-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="c471f-108">SharePoint Online käyttää rajoituksia SharePoint Online-palvelun optimaalisen suoritus kyvyn ja luotettavuuden ylläpitämiseen.</span><span class="sxs-lookup"><span data-stu-id="c471f-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="c471f-109">Rajoitus rajoittaa käyttäjän toimien tai samanaikaisten kutsujen (komento sarjojen tai koodien) määrää resurssien liikan käytön estämiseksi.</span><span class="sxs-lookup"><span data-stu-id="c471f-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="c471f-110">Jos haluat lisä tietoja kuristus kohdasta, [Vältä rajoittumatta tai estetty SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="c471f-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="c471f-111">Jos suoritus kyky on hidas **perinteisen** tai **modernin** SharePoint-sivuston tai-sivun avulla, analysoi sivut [sivun diagnostiikka työkalulla](https://aka.ms/perftool) .</span><span class="sxs-lookup"><span data-stu-id="c471f-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="c471f-112">Jos kohtaat edelleen yleistä hidasta suoritus kykyä, Lue tämän artikkelin alaosassa olevat resurssit: [johdanto SharePoint Onlinen suoritus kyvyn säätöön](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="c471f-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  