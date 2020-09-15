---
title: ATP SharePointissa, OneDrivessa ja Microsoft Teamsissa
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
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715558"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="5ff43-102">ATP SharePointissa, OneDrivessa ja Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="5ff43-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="5ff43-103">Ota Advanced Threat Protectionin suojaus käyttöön seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="5ff43-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="5ff43-104">Siirry [https://protection.office.com](https://protection.office.com) ja Kirjaudu sisään yleisen valvojan tai suojausvalvojan tilillä.</span><span class="sxs-lookup"><span data-stu-id="5ff43-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="5ff43-105">Valitse vasemman siirtymis ruudun **uhkien hallinta**-kohdassa **käytännön** \> **turvalliset liitteet**.</span><span class="sxs-lookup"><span data-stu-id="5ff43-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="5ff43-106">Valitse **Ota käyttöön SharePoint-, OneDrive-ja Microsoft TEAMSIN ATP**.</span><span class="sxs-lookup"><span data-stu-id="5ff43-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="5ff43-107">[Luo toiminta ilmoitus käytäntöä](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) ilmoitusten vastaanottamista varten, kun tunnistamme vahingollisia tiedostoja.</span><span class="sxs-lookup"><span data-stu-id="5ff43-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="5ff43-108">Katso täydelliset ohjeet tästä [aiheesta](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="5ff43-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="5ff43-109">**Huomautus**: kun ATP on suunniteltu, se ei tarkista jokaista tiedostoa SharePoint Onlinessa, OneDrive for Businessissa tai Microsoft teamsissa.</span><span class="sxs-lookup"><span data-stu-id="5ff43-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="5ff43-110">Tiedostot tarkistetaan asynkronisesti prosessi, joka käyttää jakamis toimintaa, vieras toimintaa ja uhka signaaleja haitallisten tiedostojen tunnistamiseksi.</span><span class="sxs-lookup"><span data-stu-id="5ff43-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="5ff43-111">Lisä tietoja [on tässä artikkelissa](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="5ff43-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
