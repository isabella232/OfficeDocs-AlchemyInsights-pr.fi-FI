---
title: ATP Office 365 n käyttöönotto SharePoint, OneDrive ja Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543925"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="7eda5-102">Ota Käyttöön Microsoft Defender for Office 365 for SharePoint Online, OneDrive ja Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7eda5-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="7eda5-103">Siirry ja https://protection.office.com kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="7eda5-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="7eda5-104">Valitse **Uhkien**  >  **hallintakäytännön**  >  **turvalliset liitteet**.</span><span class="sxs-lookup"><span data-stu-id="7eda5-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="7eda5-105">Valitse **Turn on Defender for Office 365 for SharePoint, OneDrive and Microsoft Teams** ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="7eda5-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="7eda5-106">(Suositus) Suorita yleisenä järjestelmänvalvojana tai SharePoint Online [-järjestelmänvalvojana Set-SPOTenant-cmdlet-komento,](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) kun **DisallowInfectedFileDownload-parametrin** arvoksi on määritetty *tosi*.</span><span class="sxs-lookup"><span data-stu-id="7eda5-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="7eda5-107">(Suositus) [Määritä havaittujen](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tiedostojen ilmoitukset.</span><span class="sxs-lookup"><span data-stu-id="7eda5-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="7eda5-108">Microsoft Defender for Office 365 ei tarkista jokaista yksittäistä tiedostoa SharePoint Onlinessa, OneDrive tai Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7eda5-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="7eda5-109">Tiedostot tarkistetaan asynkronisesti jakamis- ja vierastoimintatapahtumia käyttävän prosessin sekä älykkäiden heurististen ja uhkien signaaleiden avulla haittaohjelmien tunnistamiseen.</span><span class="sxs-lookup"><span data-stu-id="7eda5-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="7eda5-110">Katso [Microsoft Defender for Office 365 for SharePoint, OneDrive ja Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="7eda5-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>