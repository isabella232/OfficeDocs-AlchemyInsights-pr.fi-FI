---
title: SharePointin online-rajoitus
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751885"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="74829-102">SharePointin online-rajoitus</span><span class="sxs-lookup"><span data-stu-id="74829-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="74829-103">Käyttäjät saattavat saada 503-palvelimen, on varattu-virhe yritettäessä siirtyä SharePoint-tai OneDrive-sivustoihin.</span><span class="sxs-lookup"><span data-stu-id="74829-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="74829-104">Tämä virhe voi johtua rajoittamalla SharePoint-palvelussa.</span><span class="sxs-lookup"><span data-stu-id="74829-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="74829-105">SharePoint Online käyttää rajoituksia SharePoint Online-palvelun optimaalisen suoritus kyvyn ja luotettavuuden ylläpitämiseen.</span><span class="sxs-lookup"><span data-stu-id="74829-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="74829-106">Rajoitus rajoittaa käyttäjän toimien tai samanaikaisten kutsujen (komento sarjojen tai koodien) määrää resurssien liikan käytön estämiseksi.</span><span class="sxs-lookup"><span data-stu-id="74829-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="74829-107">Jos saat throttled, 99% ajasta se johtuu mukautetun koodin.</span><span class="sxs-lookup"><span data-stu-id="74829-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="74829-108">Jos haluat lisä tietoja kuristus kohdasta, [Vältä rajoittumatta tai estetty SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="74829-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="74829-109">Jos epäilet, että tämä virhe ei liity rajoittamiseen, voit tarkistaa, onko vuokraajassasi aktiivinen ylläpito, siirtymällä [viesti keskukseen](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="74829-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="74829-110">Varmista lopuksi, että käyt [palvelun kunto](https://portal.office.com/adminportal/home#/servicehealth) -sivulla tarkistaataasi mahdollisesti ilmenneitä neuvoja/tapahtumia.</span><span class="sxs-lookup"><span data-stu-id="74829-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

