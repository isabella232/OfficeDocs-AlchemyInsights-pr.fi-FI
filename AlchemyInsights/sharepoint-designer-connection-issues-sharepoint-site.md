---
title: Käyttöoikeustasoja SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760690"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="6f1bc-102">SharePoint Designer-yhteysongelmat</span><span class="sxs-lookup"><span data-stu-id="6f1bc-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="6f1bc-103">Jos SharePoint Designer on ilmennyt ongelmia yhteyden SharePoint-sivustoihin, yritä seuraavia yhteisiä ratkaisuja.</span><span class="sxs-lookup"><span data-stu-id="6f1bc-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="6f1bc-104">Vaihe 1: Tarkista SharePoint Designer on päivitetty.</span><span class="sxs-lookup"><span data-stu-id="6f1bc-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="6f1bc-105">SharePoint Designer-2013</span><span class="sxs-lookup"><span data-stu-id="6f1bc-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="6f1bc-106">SharePoint Designerin Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="6f1bc-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="6f1bc-107">Päivitä SharePoint Designer-2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="6f1bc-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="6f1bc-108">Vaihe 2: Poista tiedostot paikalliseen välimuistiin</span><span class="sxs-lookup"><span data-stu-id="6f1bc-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="6f1bc-109">Sulje SharePoint Designer-2013.</span><span class="sxs-lookup"><span data-stu-id="6f1bc-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="6f1bc-110">Selaa paikallisessa tietokoneessa, voit poistaa välimuistiin tallennetut tiedostot seuraaviin kansioihin.</span><span class="sxs-lookup"><span data-stu-id="6f1bc-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="6f1bc-111">Valitse Käynnistä, suorita ja poista kaikki tiedostot löytyy jokaisesta kohdasta sijainteihin alla.</span><span class="sxs-lookup"><span data-stu-id="6f1bc-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="6f1bc-112">Palvelimen %APPDATA%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="6f1bc-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="6f1bc-113">Avaa SharePoint Designer 2013 ja tili uudelleen ja katso jos se toimii.</span><span class="sxs-lookup"><span data-stu-id="6f1bc-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="6f1bc-114">Vaihe 3: [käyttöön Nykyaikainen Office 2013 laitteissa Windows-todennuksen](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="6f1bc-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="6f1bc-115">Vaihe 4: Järjestelmänvalvojat on mukautetun komentosarjan avulla voit sallia yhteyden SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="6f1bc-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="6f1bc-116">Saat yksityiskohtaisia ohjeita ja esimerkkejä huomioon otettavia seikkoja [Salli tai estä mukautetun komentosarjan](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="6f1bc-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


