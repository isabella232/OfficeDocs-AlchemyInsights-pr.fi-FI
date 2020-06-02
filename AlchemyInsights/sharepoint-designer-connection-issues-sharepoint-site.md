---
title: SharePoint Designerin yhteysongelmat
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511541"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="5184e-102">SharePoint Designerin yhteysongelmat</span><span class="sxs-lookup"><span data-stu-id="5184e-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="5184e-103">Jos SharePoint Designerilla on yhteysongelmia SharePoint-sivustoihin, kokeile seuraavia yleisiä ratkaisuja.</span><span class="sxs-lookup"><span data-stu-id="5184e-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="5184e-104">Vaihe 1: Varmista, että SharePoint Designer 2013:n [sharepoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja [SharePoint Designer 2013:n 2.8.2016 -päivitys](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)päivittyvät.</span><span class="sxs-lookup"><span data-stu-id="5184e-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="5184e-105">Vaihe 2: Tyhjennä paikalliset välimuistitiedostot:</span><span class="sxs-lookup"><span data-stu-id="5184e-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="5184e-106">Sulje SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="5184e-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="5184e-107">Poista paikallisessa tietokoneessa kaikki seuraavista kansioista löydetyt tiedostot.</span><span class="sxs-lookup"><span data-stu-id="5184e-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="5184e-108">%APPDATA%\Microsoft\Web-palvelinlaajennukset\Välimuisti</span><span class="sxs-lookup"><span data-stu-id="5184e-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="5184e-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="5184e-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="5184e-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="5184e-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="5184e-111">Avaa SharePoint Designer 2013 ja anna tili uudelleen, jotta näet toimiiko se.</span><span class="sxs-lookup"><span data-stu-id="5184e-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="5184e-112">Vaihe 3: [Ota office 2013:n nykyaikainen todennus käyttöön Windows-laitteissa](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="5184e-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="5184e-113">Vaihe 4: Järjestelmänvalvojien on **sallittava mukautettu komentosarja** SharePoint-hallintakeskuksen asetuksissa, jotta SharePoint Designer -yhteys voidaan muodostaa.</span><span class="sxs-lookup"><span data-stu-id="5184e-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="5184e-114">Lisätietoja [on ohjeaiheessa Mukautetun komentosarjan salliminen tai estäminen.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="5184e-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


