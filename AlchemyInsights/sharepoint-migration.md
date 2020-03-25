---
title: Asetusten siirtäminen SharePoint Onlineen
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932727"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="ad1eb-102">Asetusten siirtäminen SharePoint Onlineen</span><span class="sxs-lookup"><span data-stu-id="ad1eb-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="ad1eb-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="ad1eb-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ad1eb-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="ad1eb-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ad1eb-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="ad1eb-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ad1eb-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="ad1eb-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ad1eb-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="ad1eb-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ad1eb-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="ad1eb-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ad1eb-109">**Siirron asetukset**</span><span class="sxs-lookup"><span data-stu-id="ad1eb-109">**Migration options**</span></span>

<span data-ttu-id="ad1eb-110">On olemassa erilaisia vaihtoehtoja siirtää sisältöä SharePoint Online, riippuen koosta ja määrästä tiedostoja sinun täytyy nähdä luettelo vaihtoehdoista [täällä](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="ad1eb-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="ad1eb-111">Lisätietoja sisällön siirrosta on alla olevissa linkeissä.</span><span class="sxs-lookup"><span data-stu-id="ad1eb-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="ad1eb-112">SharePoint-siirtotyökalu</span><span class="sxs-lookup"><span data-stu-id="ad1eb-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="ad1eb-113">Siirron hallinnan käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="ad1eb-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="ad1eb-114">Sharepoint Onlinen ja ODB:n siirtonopeus</span><span class="sxs-lookup"><span data-stu-id="ad1eb-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="ad1eb-115">SharePoint Onlinessa ei saa kuristaa tai estää</span><span class="sxs-lookup"><span data-stu-id="ad1eb-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="ad1eb-116">SharePoint-siirron arviointityökalu (SMAT)</span><span class="sxs-lookup"><span data-stu-id="ad1eb-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="ad1eb-117">**Huomautus:** Tällä hetkellä SharePoint Migration -työkalu tukee vain SharePoint 2010:stä ja 2013:sta peräisin olevia siirtoja.</span><span class="sxs-lookup"><span data-stu-id="ad1eb-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="ad1eb-118">Versiota 2016 tai 2019 ei tueta tällä hetkellä.</span><span class="sxs-lookup"><span data-stu-id="ad1eb-118">Version 2016 or 2019 are not supported at this time.</span></span>
