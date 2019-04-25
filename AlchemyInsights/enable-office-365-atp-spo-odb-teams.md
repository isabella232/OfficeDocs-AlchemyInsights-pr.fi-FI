---
title: 'ATP Office 365: n käyttöön SharePoint ja Microsoft-ryhmien OneDrive'
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403030"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="8e4e3-102">Ota käyttöön Office 365 kehittyneen uhkien suojaa SharePoint Online, OneDrive ja Microsoftin työryhmät</span><span class="sxs-lookup"><span data-stu-id="8e4e3-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="8e4e3-103">Siirry https://protection.office.com ja kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="8e4e3-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="8e4e3-104">Valitse **Threat management** > **käytännön** > **Turvalliset liitetiedostot**.</span><span class="sxs-lookup"><span data-stu-id="8e4e3-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="8e4e3-105">Valitse **ATP SharePoint, OneDrive-ja Microsoft-ryhmien käyttöön**, ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="8e4e3-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="8e4e3-106">(Suositus) Yleinen järjestelmänvalvoja tai SharePoint Online järjestelmänvalvojana Suorita [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet **DisallowInfectedFileDownload** -parametrin arvoksi *true*.</span><span class="sxs-lookup"><span data-stu-id="8e4e3-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="8e4e3-107">(Suositus) [Määritä hälytykset](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) havaittiin tiedostoja.</span><span class="sxs-lookup"><span data-stu-id="8e4e3-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="8e4e3-108">ATP on nJos haluat skannaus SharePoint Online OneDrive tai Microsoftin Teams kaikki yhteen tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="8e4e3-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="8e4e3-109">Tiedostot tarkistetaan asynkronisesti, prosessi, joka käyttää jakamisen ja Vieras toiminnan tapahtumat, älykäs ja uhka signaalien tunnistamiseen vahingollisia tiedostoja kautta.</span><span class="sxs-lookup"><span data-stu-id="8e4e3-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="8e4e3-110">Katso [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="8e4e3-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>