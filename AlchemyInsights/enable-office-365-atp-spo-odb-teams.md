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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506915"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="ae2f8-102">Office 365:n Advanced Threat Protectionin ottaminen käyttöön SharePoint Onlinessa, OneDrivessa ja Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="ae2f8-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="ae2f8-103">Mene https://protection.office.com sisään ja kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="ae2f8-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="ae2f8-104">Valitse **Uhkien**  >  **hallintakäytännön**  >  **turvalliset liitteet**.</span><span class="sxs-lookup"><span data-stu-id="ae2f8-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="ae2f8-105">Valitse **Ota ATP käyttöön SharePointissa, OneDrivessa ja Microsoft Teamsissa**ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="ae2f8-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="ae2f8-106">(Suositus) Suorita [Set-SPOTenant-cmdlet-komento](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) yleisenä järjestelmänvalvojana tai SharePoint Online -järjestelmänvalvojana siten, että **DisallowInfectedFileDownload-parametrin** arvo on *true*.</span><span class="sxs-lookup"><span data-stu-id="ae2f8-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="ae2f8-107">(Suositus) [Määritä havaittujen tiedostojen hälytykset.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)</span><span class="sxs-lookup"><span data-stu-id="ae2f8-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="ae2f8-108">ATP tarkistaa jokaisen tiedoston SharePoint Onlinessa, OneDrivessa tai Microsoft Teamsissa.</span><span class="sxs-lookup"><span data-stu-id="ae2f8-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="ae2f8-109">Tiedostot skannataan asynkronisesti jakamis- ja vierastoimintatapahtumia käyttävän prosessin kautta sekä älykkäiden heuristiikka- ja uhkasignaalien avulla haitallisten tiedostojen tunnistamiseen.</span><span class="sxs-lookup"><span data-stu-id="ae2f8-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="ae2f8-110">Katso [SHAREPointin, OneDriven ja Microsoft Teamsin ATP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="ae2f8-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>