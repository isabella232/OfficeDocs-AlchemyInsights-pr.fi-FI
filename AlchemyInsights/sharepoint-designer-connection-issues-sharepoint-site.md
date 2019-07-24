---
title: SharePoint Designer-yhteysongelmat
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840548"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="5583c-102">SharePoint Designer-yhteysongelmat</span><span class="sxs-lookup"><span data-stu-id="5583c-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="5583c-103">Jos SharePoint Designer on ilmennyt ongelmia yhteyden SharePoint-sivustoihin, yritä seuraavia yhteisiä ratkaisuja.</span><span class="sxs-lookup"><span data-stu-id="5583c-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="5583c-104">Vaihe 1: Varmista, että SharePoint Designer 2013 päivitetään [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja [2. elokuuta 2016 päivittää SharePoint Designer-2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="5583c-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="5583c-105">Vaihe 2: Poista tiedostot paikalliseen välimuistiin:</span><span class="sxs-lookup"><span data-stu-id="5583c-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="5583c-106">Sulje SharePoint Designer-2013.</span><span class="sxs-lookup"><span data-stu-id="5583c-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="5583c-107">Paikallisen tietokoneen poistaa kaikki tiedostot löytyvät seuraavista kansioista.</span><span class="sxs-lookup"><span data-stu-id="5583c-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="5583c-108">%APPDATA%\Microsoft\Web palvelimen Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="5583c-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="5583c-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="5583c-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="5583c-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="5583c-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="5583c-111">Avaa SharePoint Designer 2013 ja tili uudelleen ja katso jos se toimii.</span><span class="sxs-lookup"><span data-stu-id="5583c-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="5583c-112">Vaihe 3: [käyttöön Nykyaikainen Office 2013 laitteissa Windows-todennuksen](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="5583c-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="5583c-113">Vaihe 4: Järjestelmänvalvojien on **Mukautetun komentosarjan avulla** SharePoint-hallintakeskukseen asetukset SharePoint Designer-yhteys.</span><span class="sxs-lookup"><span data-stu-id="5583c-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="5583c-114">Katso [Salli tai estä mukautetun komentosarjan](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) lisätietoja.</span><span class="sxs-lookup"><span data-stu-id="5583c-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


