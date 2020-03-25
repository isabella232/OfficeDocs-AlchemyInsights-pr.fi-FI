---
title: SharePointin siirron rajoittaminen 503-virheillä
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931655"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="a8c06-102">SharePointin siirron rajoittaminen 503-virheillä</span><span class="sxs-lookup"><span data-stu-id="a8c06-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="a8c06-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="a8c06-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a8c06-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="a8c06-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a8c06-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="a8c06-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a8c06-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="a8c06-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a8c06-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="a8c06-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a8c06-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="a8c06-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a8c06-109">**503 virheitä siirryttäessä SharePoint Onlineen**</span><span class="sxs-lookup"><span data-stu-id="a8c06-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="a8c06-110">Näyttää siltä, että olet siirtymässä SharePoint Onlineen ja saat 503-virheitä.</span><span class="sxs-lookup"><span data-stu-id="a8c06-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="a8c06-111">Noudata alla olevia ohjeita, jotta voimme auttaa sinua mahdollisimman pian.</span><span class="sxs-lookup"><span data-stu-id="a8c06-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="a8c06-112">Valitse **Ota yhteyttä tukeen**ja sitten Uusi **palvelupyyntö**.</span><span class="sxs-lookup"><span data-stu-id="a8c06-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="a8c06-113">Kirjoita otsikkoa ja kuvausta varten **SharePoint Migration Throttling with 503**.</span><span class="sxs-lookup"><span data-stu-id="a8c06-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="a8c06-114">Kun lippu on lähetetty, päivitä se seuraavilla tiedoilla:</span><span class="sxs-lookup"><span data-stu-id="a8c06-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="a8c06-115">Kuinka paljon muuttoa on jäljellä (esimerkiksi kuinka monta pbs?).</span><span class="sxs-lookup"><span data-stu-id="a8c06-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="a8c06-116">Siirron alkamis- ja päättymispäivä.</span><span class="sxs-lookup"><span data-stu-id="a8c06-116">Migration start and end date.</span></span>
    - <span data-ttu-id="a8c06-117">Kuvaile, mistä siirrät sisältöä, kuten SharePoint Serveristä, Boxista, GDrivesta, jaetuista tiedostorekiveistä jne..</span><span class="sxs-lookup"><span data-stu-id="a8c06-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="a8c06-118">Arvioi rajoitusvirheiden määrä (esimerkiksi x kaasuviputinti tunnissa?) ja milloin rajoitus tapahtui.</span><span class="sxs-lookup"><span data-stu-id="a8c06-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="a8c06-119">Käyttämäsi siirtotyökalu (esimerkiksi SPMT tai ShareGate).</span><span class="sxs-lookup"><span data-stu-id="a8c06-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


