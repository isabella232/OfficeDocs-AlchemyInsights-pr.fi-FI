---
title: SharePoint-siirto Ja SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931547"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="b79a4-102">SharePoint-siirto Ja SPMT</span><span class="sxs-lookup"><span data-stu-id="b79a4-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="b79a4-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="b79a4-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b79a4-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="b79a4-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b79a4-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="b79a4-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b79a4-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="b79a4-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b79a4-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="b79a4-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b79a4-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="b79a4-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b79a4-109">**SharePoint-siirtotyökalu**</span><span class="sxs-lookup"><span data-stu-id="b79a4-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="b79a4-110">SharePoint Migration Tool -työkalu on suunniteltu käytettäväksi pienimmistä tiedostoista suuriin yrityssiirtoihin, ja sen avulla voit siirtää tietosi pilveen ja hyödyntää uusinta yhteistyötä, älykkyyttä ja tietoturvaratkaisuja Office 365:n avulla.</span><span class="sxs-lookup"><span data-stu-id="b79a4-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="b79a4-111">SharePoint Migration Tool -työkalun lataaminen ja asentaminen</span><span class="sxs-lookup"><span data-stu-id="b79a4-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="b79a4-112">Yleisten SPMT-ongelmien ja -virheiden vianmääritys</span><span class="sxs-lookup"><span data-stu-id="b79a4-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="b79a4-113">SPMT-asennusongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="b79a4-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
