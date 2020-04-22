---
title: Office 365 ATP:n ottaminen käyttöön SharePointissa, OneDrivessa ja Microsoft Teamsissa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703423"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="d006b-102">Office 365 Advanced Threat Protectionin ottaminen käyttöön SharePoint Onlinessa, OneDrivessa ja Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="d006b-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="d006b-103">Mene https://protection.office.com sisään ja kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="d006b-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="d006b-104">Valitse **Uhkien** > **hallintakäytännön** > **turvalliset liitteet**.</span><span class="sxs-lookup"><span data-stu-id="d006b-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="d006b-105">Valitse **Ota ATP sharepointiin, OneDriveen ja Microsoft Teamsiin käyttöön**ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="d006b-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="d006b-106">(Suositus) Yleisenä järjestelmänvalvojana tai SharePoint Online -järjestelmänvalvojana suorita [Set-SPOTenant-cmdlet-tiedosto,](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) jonka **DisallowInfectedFileDownload-parametrin** arvo on *true*.</span><span class="sxs-lookup"><span data-stu-id="d006b-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="d006b-107">(Suositus) [Määritä havaittujen tiedostojen hälytykset.](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)</span><span class="sxs-lookup"><span data-stu-id="d006b-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="d006b-108">ATP tarkistaa jokaisen tiedoston SharePoint Onlinessa, OneDrivessa tai Microsoft Teamsissa.</span><span class="sxs-lookup"><span data-stu-id="d006b-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="d006b-109">Tiedostot skannataan asynkronisesti prosessilla, joka käyttää jakamista ja asiakkaiden toimintatapahtumia sekä älykkäitä heuristiikkaa ja uhkasignaaleja haitallisten tiedostojen tunnistamiseen.</span><span class="sxs-lookup"><span data-stu-id="d006b-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="d006b-110">Katso [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="d006b-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>