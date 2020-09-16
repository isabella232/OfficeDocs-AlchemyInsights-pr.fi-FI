---
title: SharePoint Designer-yhteys ongelmat
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727168"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="025e1-102">SharePoint Designer-yhteys ongelmat</span><span class="sxs-lookup"><span data-stu-id="025e1-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="025e1-103">Jos SharePoint Designerissa on SharePoint-sivuston yhteys ongelmia, kokeile seuraavia yleisiä ratkaisuja.</span><span class="sxs-lookup"><span data-stu-id="025e1-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="025e1-104">Vaihe 1: Varmista, että SharePoint Designer 2013 on päivitetty SharePoint [Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja [2016 SharePoint Designer 2013-päivitys](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="025e1-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="025e1-105">Vaihe 2: paikallisten väli muisti tiedostojen tyhjentäminen:</span><span class="sxs-lookup"><span data-stu-id="025e1-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="025e1-106">Sulje SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="025e1-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="025e1-107">Poista paikallisessa tieto koneessa kaikki tiedostot, jotka löytyvät seuraavista kansioista.</span><span class="sxs-lookup"><span data-stu-id="025e1-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="025e1-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="025e1-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="025e1-109">%APPDATA%\Microsoft\SharePoint Designer\proxetassembrootcache</span><span class="sxs-lookup"><span data-stu-id="025e1-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="025e1-110">%USERPROFILE%\AppData Local \ Microsoft\websitecache</span><span class="sxs-lookup"><span data-stu-id="025e1-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="025e1-111">Avaa SharePoint Designer 2013 ja anna tili uudelleen, jotta näet, toimiiko se.</span><span class="sxs-lookup"><span data-stu-id="025e1-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="025e1-112">Vaihe 3: [Ota käyttöön moderni todennus Office 2013-palvelua varten Windows-laitteissa](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="025e1-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="025e1-113">Vaihe 4: järjestelmänvalvojien on sallittava SharePoint Designer-yhteyden salliminen **mukautetun komento sarjan** avulla SharePoint-hallinta keskuksen asetuksissa.</span><span class="sxs-lookup"><span data-stu-id="025e1-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="025e1-114">Lisä tietoja on kohdassa [mukautetun komento sarjan salliminen tai estäminen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="025e1-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


