---
title: Ongelmat tietojen siirtämisessä SharePoint Onlineen
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931691"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="ee807-102">Ongelmat tietojen siirtämisessä SharePoint Onlineen</span><span class="sxs-lookup"><span data-stu-id="ee807-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="ee807-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="ee807-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ee807-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="ee807-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ee807-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="ee807-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ee807-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="ee807-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ee807-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="ee807-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ee807-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="ee807-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ee807-109">**Yli 100 Tt:n tietojen siirtäminen**</span><span class="sxs-lookup"><span data-stu-id="ee807-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="ee807-110">Näyttää siltä, että siirrät yli 100 Tt tietoja SharePoint Onlineen.</span><span class="sxs-lookup"><span data-stu-id="ee807-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="ee807-111">Noudata alla olevia ohjeita, jotta voimme auttaa sinua mahdollisimman pian.</span><span class="sxs-lookup"><span data-stu-id="ee807-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="ee807-112">Valitse **Uusi palvelupyyntö**ja sitten **Uusi palvelupyyntö**.</span><span class="sxs-lookup"><span data-stu-id="ee807-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="ee807-113">Jätä otsikko ja kuvaus **SharePoint-siirroksi yli 100 Tt**: n k.</span><span class="sxs-lookup"><span data-stu-id="ee807-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="ee807-114">Kun lippu on lähetetty, päivitä se seuraavilla tiedoilla:</span><span class="sxs-lookup"><span data-stu-id="ee807-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="ee807-115">Siirron arvioitu koko.</span><span class="sxs-lookup"><span data-stu-id="ee807-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="ee807-116">Arvio siitä, milloin haluat aloittaa ja suorittaa siirron loppuun.</span><span class="sxs-lookup"><span data-stu-id="ee807-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="ee807-117">Kuvaile, mistä siirrät sisältöä, kuten SharePoint Serveristä, Boxista, GDrivesta, jaetuista tiedostorekiveistä jne..</span><span class="sxs-lookup"><span data-stu-id="ee807-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

