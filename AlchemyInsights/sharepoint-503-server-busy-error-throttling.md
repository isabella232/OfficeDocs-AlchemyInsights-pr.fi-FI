---
title: SharePoint Onlinen rajoitus
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 50b2c29db1fd294abe6c9e60f067156109de392b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742206"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="fe10b-102">SharePoint Onlinen rajoitus</span><span class="sxs-lookup"><span data-stu-id="fe10b-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="fe10b-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="fe10b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="fe10b-104">**503 palvelin on varattu virhe**</span><span class="sxs-lookup"><span data-stu-id="fe10b-104">**503 server is busy error**</span></span>

<span data-ttu-id="fe10b-105">Käyttäjät saattavat saada 503-palvelimen olevan varattu virhe yritettäessä siirtyä SharePoint- tai OneDrive-sivustoihin.</span><span class="sxs-lookup"><span data-stu-id="fe10b-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="fe10b-106">Tämä virhe voi johtua sharepoint-palvelun kuristamisesta.</span><span class="sxs-lookup"><span data-stu-id="fe10b-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="fe10b-107">SharePoint Online käyttää rajoittamista SharePoint Online -palvelun optimaalisen suorituskyvyn ja luotettavuuden ylläpitämiseen.</span><span class="sxs-lookup"><span data-stu-id="fe10b-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="fe10b-108">Rajoittaminen rajoittaa käyttäjien toimien tai samanaikaisten kutsujen määrää (komentosarjojen tai koodin avulla), jotta resurssien liikakäyttö estetään.</span><span class="sxs-lookup"><span data-stu-id="fe10b-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="fe10b-109">Lisätietoja kuristamisesta on [ohjeaiheessa Vältä kuristamisen tai estymisen estäminen SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="fe10b-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="fe10b-110">Jos uskot, että tämä virhe ei liity kuristukseen, voit tarkistaa, onko vuokraajassa aktiivista ylläpitoa, siirtymällä [Viestikeskukseen](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="fe10b-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="fe10b-111">Varmista lopuksi, että käyt [Palvelun kunto -sivulla](https://portal.office.com/adminportal/home#/servicehealth) ja tarkistat mahdolliset tiedotteet/tapahtumat.</span><span class="sxs-lookup"><span data-stu-id="fe10b-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

