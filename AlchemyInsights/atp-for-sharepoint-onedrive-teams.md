---
title: Microsoft Defender for Office 365 for SharePoint, OneDrive ja Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543574"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="54a5c-102">Microsoft Defender for Office 365 for SharePoint, OneDrive ja Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="54a5c-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="54a5c-103">Ota Microsoft Defender käyttöön seuraavien Office 365:</span><span class="sxs-lookup"><span data-stu-id="54a5c-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="54a5c-104">Siirry yleisen [https://protection.office.com](https://protection.office.com) järjestelmänvalvojan tai suojauksen järjestelmänvalvojan tiliin ja kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="54a5c-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="54a5c-105">Valitse vasemman siirtymisruudun **Uhkien hallinta**-kohdassa **Käytännön** \> **turvalliset liitteet**.</span><span class="sxs-lookup"><span data-stu-id="54a5c-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="54a5c-106">Valitse **Ota Defender käyttöön for Office 365 for SharePoint, OneDrive ja Microsoft Teams.**</span><span class="sxs-lookup"><span data-stu-id="54a5c-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="54a5c-107">[Luo toimintailmoituskäytäntö, joka](/microsoft-365/compliance/create-activity-alerts) vastaanottaa ilmoituksia, kun havaitsemme vahingollisia tiedostoja.</span><span class="sxs-lookup"><span data-stu-id="54a5c-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="54a5c-108">Katso täydelliset ohjeet tästä [ista Turvallisten liitteiden käyttöönottaminen SharePoint OneDrive ja Microsoft Teams.](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="54a5c-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="54a5c-109">**Huomautus:** Microsoft Defender for Office 365 ei tarkista jokaista SharePoint Onlinessa, OneDrive for Business tai Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="54a5c-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="54a5c-110">Tiedostoja skannataan asynkronisesti prosessi, joka käyttää jakamistoimintaa, vierastoimintaa ja uhkien signaaleja haittaohjelmien tunnistamiseen.</span><span class="sxs-lookup"><span data-stu-id="54a5c-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="54a5c-111">Lisätietoja on kohdassa [Turvalliset liitteet SharePoint, OneDrive ja Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="54a5c-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
