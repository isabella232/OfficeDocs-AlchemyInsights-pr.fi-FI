---
title: SharePoint Onlinen rajoitus
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931439"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="022dc-102">SharePoint Onlinen rajoitus</span><span class="sxs-lookup"><span data-stu-id="022dc-102">SharePoint Online throttling</span></span>

<span data-ttu-id="022dc-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="022dc-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="022dc-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="022dc-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="022dc-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="022dc-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="022dc-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="022dc-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="022dc-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="022dc-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="022dc-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="022dc-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="022dc-109">**SharePoint Onlinen rajoitus**</span><span class="sxs-lookup"><span data-stu-id="022dc-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="022dc-110">SharePoint Online käyttää rajoitusta SharePoint Online -palvelun optimaalisen suorituskyvyn ja luotettavuuden ylläpitämiseen.</span><span class="sxs-lookup"><span data-stu-id="022dc-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="022dc-111">Kuristus rajoittaa käyttäjän toimintojen tai samanaikaisten kutsujen määrää (komentosarjan tai koodin mukaan) resurssien liikakäytön estämiseksi.</span><span class="sxs-lookup"><span data-stu-id="022dc-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="022dc-112">Lisätietoja on alla olevissa linkeissä.</span><span class="sxs-lookup"><span data-stu-id="022dc-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="022dc-113">SharePoint Onlinessa ei saa kuristaa tai estää</span><span class="sxs-lookup"><span data-stu-id="022dc-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="022dc-114">Tietojen siirto ja spo-rajoitus</span><span class="sxs-lookup"><span data-stu-id="022dc-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="022dc-115">SharePoint Onlinen ja OneDriven siirtonopeus</span><span class="sxs-lookup"><span data-stu-id="022dc-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="022dc-116">SharePoint Onlinen kuristimen käsitteleminen eksponentiaalisen perääntymisen avulla</span><span class="sxs-lookup"><span data-stu-id="022dc-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="022dc-117">Kapasiteetin suunnittelu ja kuormituksen testaus SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="022dc-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

