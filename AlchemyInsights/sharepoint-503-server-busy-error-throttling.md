---
title: SharePoint Onlinen rajoitus
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931223"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="61403-102">SharePoint Onlinen rajoitus</span><span class="sxs-lookup"><span data-stu-id="61403-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="61403-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="61403-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="61403-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="61403-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="61403-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="61403-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="61403-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="61403-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="61403-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="61403-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="61403-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="61403-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="61403-109">**503 palvelin on varattu virhe**</span><span class="sxs-lookup"><span data-stu-id="61403-109">**503 server is busy error**</span></span>

<span data-ttu-id="61403-110">Käyttäjät saattavat saada 503-palvelimen olevan varattu virhe yritettäessä siirtyä SharePoint- tai OneDrive-sivustoihin.</span><span class="sxs-lookup"><span data-stu-id="61403-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="61403-111">Tämä virhe voi johtua sharepoint-palvelun kuristamisesta.</span><span class="sxs-lookup"><span data-stu-id="61403-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="61403-112">SharePoint Online käyttää rajoitusta SharePoint Online -palvelun optimaalisen suorituskyvyn ja luotettavuuden ylläpitämiseen.</span><span class="sxs-lookup"><span data-stu-id="61403-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="61403-113">Kuristus rajoittaa käyttäjän toimintojen tai samanaikaisten kutsujen määrää (komentosarjan tai koodin mukaan) resurssien liikakäytön estämiseksi.</span><span class="sxs-lookup"><span data-stu-id="61403-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="61403-114">Lisätietoja kuristamisesta on [ohjeaiheessa Vältä kuristamisen tai estymisen estäminen SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="61403-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="61403-115">Jos uskot, että tämä virhe ei liity kuristukseen, voit tarkistaa, onko vuokraajassa aktiivista ylläpitoa, siirtymällä [Viestikeskukseen](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="61403-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="61403-116">Varmista lopuksi, että käyt [Palvelun kunto -sivulla](https://portal.office.com/adminportal/home#/servicehealth) ja tarkistat mahdolliset tiedotteet/tapahtumat.</span><span class="sxs-lookup"><span data-stu-id="61403-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

