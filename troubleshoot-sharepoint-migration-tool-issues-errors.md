---
title: SharePoint-siirtotyökalun ongelmien ja virheiden vianmääritys
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931115"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="29cc0-102">SharePoint-siirtotyökalun ongelmien ja virheiden vianmääritys</span><span class="sxs-lookup"><span data-stu-id="29cc0-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="29cc0-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="29cc0-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="29cc0-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="29cc0-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="29cc0-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="29cc0-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="29cc0-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="29cc0-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="29cc0-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="29cc0-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="29cc0-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="29cc0-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="29cc0-109">**Yleisiä ongelmia ja virheitä**</span><span class="sxs-lookup"><span data-stu-id="29cc0-109">**Common issues and errors**</span></span>

<span data-ttu-id="29cc0-110">SharePoint Migration Tool (SPMT) -työkalua käytettäessä saattaa ilmetä joitakin yleisiä ongelmia ja virheitä.</span><span class="sxs-lookup"><span data-stu-id="29cc0-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="29cc0-111">Katso alla olevista linkeistä lisätietoja.</span><span class="sxs-lookup"><span data-stu-id="29cc0-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="29cc0-112">Yleisten SPMT-ongelmien ja -virheiden vianmääritys</span><span class="sxs-lookup"><span data-stu-id="29cc0-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="29cc0-113">SPMT:n asennusongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="29cc0-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)