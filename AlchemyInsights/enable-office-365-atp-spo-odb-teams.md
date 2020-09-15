---
title: Office 365 ATP:N käyttöönottaminen SharePointissa, OneDrivessa ja Microsoft Teamsissa
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709904"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="eb640-102">Office 365 Advanced Threat Protectionin käyttöönotto SharePoint Onlinessa, OneDrivessa ja Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="eb640-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="eb640-103">Siirry kohtaan https://protection.office.com ja Kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="eb640-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="eb640-104">Valitse **uhkien hallinta**  >  **käytännön**  >  **turvalliset liitteet**.</span><span class="sxs-lookup"><span data-stu-id="eb640-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="eb640-105">Valitse **Ota SharePoint-, OneDrive-ja Microsoft TEAMSIN ATP käyttöön**ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="eb640-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="eb640-106">Suositellut Jos sinulla on yleinen järjestelmänvalvojana tai SharePoint Online-järjestelmänvalvojana, suorita [-spoalion cmdlet-](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) komentosovelma, jonka **Disallowinfectedfiledownload** -parametrin arvona on *True*.</span><span class="sxs-lookup"><span data-stu-id="eb640-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="eb640-107">Suositellut [Määritä](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tunnistettuja tiedostoja koskevat ilmoitukset.</span><span class="sxs-lookup"><span data-stu-id="eb640-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="eb640-108">ATP tarkistaa kaikki yksittäiset tiedostot SharePoint Onlinessa, OneDrivessa tai Microsoft Teamsissa.</span><span class="sxs-lookup"><span data-stu-id="eb640-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="eb640-109">Tiedostot skannataan asynkronisesti käyttämällä jakamis-ja vieras toiminto tapahtumia sekä älykkään heuristiikkaa ja uhka signaaleja haitallisten tiedostojen tunnistamiseksi.</span><span class="sxs-lookup"><span data-stu-id="eb640-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="eb640-110">Katso [SharePointin, OneDriven ja Microsoft teamsin ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="eb640-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>