---
title: SharePoint Onlinen rajoittaminen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773844"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="042b1-102">SharePoint Onlinen rajoittaminen</span><span class="sxs-lookup"><span data-stu-id="042b1-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="042b1-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="042b1-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="042b1-104">**503-palvelin on varattu-virhe**</span><span class="sxs-lookup"><span data-stu-id="042b1-104">**503 server is busy error**</span></span>

<span data-ttu-id="042b1-105">Käyttäjät voivat saada 503-palvelin on varattu-virhe, kun yrität siirtyä SharePoint-tai OneDrive-sivustoihin.</span><span class="sxs-lookup"><span data-stu-id="042b1-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="042b1-106">Tämä virhe voi johtua siitä, että SharePoint-palvelussa käytetään rajoitusta.</span><span class="sxs-lookup"><span data-stu-id="042b1-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="042b1-107">SharePoint Online käyttää rajoittamista SharePoint Online -palvelun optimaalisen suorituskyvyn ja luotettavuuden ylläpitämiseen.</span><span class="sxs-lookup"><span data-stu-id="042b1-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="042b1-108">Rajoittaminen rajoittaa käyttäjien toimien tai samanaikaisten kutsujen määrää (komentosarjojen tai koodin avulla), jotta resurssien liikakäyttö estetään.</span><span class="sxs-lookup"><span data-stu-id="042b1-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="042b1-109">Lisä tietoja rajoittimen käyttämisestä on Ohje aiheessa [SharePoint Onlinessa ei saa estää tai estää niiden käytön estämistä](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="042b1-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="042b1-110">Jos uskot, että tämä virhe ei liity kuristamiseen, voit tarkistaa, onko vuokra ajan käytössä aktiivista kunnossapitoa, siirtymällä [viesti keskukseen](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="042b1-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="042b1-111">Varmista lopuksi, että vierailet [palvelun kunto](https://portal.office.com/adminportal/home#/servicehealth) -sivulla, jotta voit tarkistaa kaikki mahdollisesti tapahtuvat varoitukset ja häiriöt.</span><span class="sxs-lookup"><span data-stu-id="042b1-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

