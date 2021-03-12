---
title: Microsoft Defender for Office 365:n ottaminen käyttöön SharePoint Onlinessa, OneDrivessa ja Microsoft Teamsissa
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745307"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="4bfa0-102">Microsoft Defender for Office 365:n ottaminen käyttöön SharePoint Onlinessa, OneDrivessa ja Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="4bfa0-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="4bfa0-103">Kirjaudu [Office 365:n](https://protection.office.com/)tietoturva- ja yhteensopivuuskeskukseen yleisen järjestelmänvalvojan tai suojauksen järjestelmänvalvojan tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="4bfa0-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="4bfa0-104">Valitse **vasemmasta** ruudusta Uhkien hallinta ja valitse sitten **Käytännön**  >  [turvalliset liitteet.](https://protection.office.com/safeattachment)</span><span class="sxs-lookup"><span data-stu-id="4bfa0-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="4bfa0-105">Valitse **Ota Microsoft Defender for Office 365 käyttöön SharePointissa, OneDrivessa ja Microsoft Teamsissa** ja valitse sitten **Tallenna.**</span><span class="sxs-lookup"><span data-stu-id="4bfa0-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="4bfa0-106">Suorita yleisenä järjestelmänvalvojana tai SharePoint Online -järjestelmänvalvojana seuraava PowerShell-cmdlet-komento, jonka **DisallowInfectedFileDownload-parametrin** arvoksi on määritetty *tosi:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="4bfa0-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="4bfa0-107">Tunnistettuihin tiedostoihin määritettyjen ilmoitusten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="4bfa0-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="4bfa0-108">Lisätietoja on [sharePointin, OneDriven ja Microsoft Teamsin Microsoft Defender for Office 365:ssä.](https://go.microsoft.com/fwlink/?linkid=2092041)</span><span class="sxs-lookup"><span data-stu-id="4bfa0-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
