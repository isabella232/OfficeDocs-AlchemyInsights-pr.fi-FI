---
title: Suorituskyky ongelmat-SharePoint tai OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771898"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="c03e8-102">SharePointin tai OneDriven hidas, saavuttamattomissa tai poissa käytöstä useille käyttäjille</span><span class="sxs-lookup"><span data-stu-id="c03e8-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="c03e8-103">SharePoint tai OneDrive voi olla hidas, käyttökelvoton tai ei käytettävissä tai se voi näyttää palvelua ei ole käytettävissä tai 503-virheitä useista syistä:</span><span class="sxs-lookup"><span data-stu-id="c03e8-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="c03e8-104">Jos SharePoint-tai OneDrive-sivustosi on hidas tai viivästynyt useille käyttäjille, kyseessä saattaa olla väliaikainen palvelu ongelma, jossa käyttäjät saavat ajoittaisia viiveitä tai siirtymis virheitä SharePoint-sivustoja tai OneDrive-sisältöä käytettäessä.</span><span class="sxs-lookup"><span data-stu-id="c03e8-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="c03e8-105">Tarkista [palvelun kunnon koonti näytöstä](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , onko organisaatiosi vaikuttanut siihen.</span><span class="sxs-lookup"><span data-stu-id="c03e8-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="c03e8-106">Käyttäjät voivat saada *503-palvelin on varattu* -virhe, kun yrität siirtyä SharePoint-tai OneDrive-sivustoihin.</span><span class="sxs-lookup"><span data-stu-id="c03e8-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="c03e8-107">Tämä virhe voi johtua siitä, että SharePoint-palvelussa käytetään rajoitusta.</span><span class="sxs-lookup"><span data-stu-id="c03e8-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="c03e8-108">SharePoint Online käyttää rajoittamista SharePoint Online -palvelun optimaalisen suorituskyvyn ja luotettavuuden ylläpitämiseen.</span><span class="sxs-lookup"><span data-stu-id="c03e8-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="c03e8-109">Rajoittaminen rajoittaa käyttäjien toimien tai samanaikaisten kutsujen määrää (komentosarjojen tai koodin avulla), jotta resurssien liikakäyttö estetään.</span><span class="sxs-lookup"><span data-stu-id="c03e8-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="c03e8-110">Lisä tietoja rajoittimen käyttämisestä on Ohje aiheessa [SharePoint Onlinessa ei saa estää tai estää niiden käytön estämistä](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="c03e8-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="c03e8-111">Jos suoritus kyky on hidas **perinteisen** tai **modernin** SharePoint-sivuston tai-sivun avulla, analysoi sivut käyttämällä [sivun diagnostiikka-työkalua](https://aka.ms/perftool) .</span><span class="sxs-lookup"><span data-stu-id="c03e8-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="c03e8-112">Jos sinulla on edelleen yleinen hidas suoritus kyky, tutustu tämän artikkelin lopussa oleviin resursseihin: [SharePoint Onlinen suoritus kyvyn](https://go.microsoft.com/fwlink/?linkid=2024334) parantaminen</span><span class="sxs-lookup"><span data-stu-id="c03e8-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  