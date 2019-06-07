---
title: ATP-OneDrive, SharePoint ja Microsoft-ryhmien
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765014"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="6cf20-102">ATP-OneDrive, SharePoint ja Microsoft-ryhmien</span><span class="sxs-lookup"><span data-stu-id="6cf20-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="6cf20-103">Advanced Threat Protection käyttöön seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="6cf20-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="6cf20-104">Siirry [https://protection.office.com](https://protection.office.com) ja Yleinen järjestelmänvalvoja tai järjestelmänvalvojan suojaustilin kirjautumalla.</span><span class="sxs-lookup"><span data-stu-id="6cf20-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="6cf20-105">Valitse vasemmasta siirtymisruudusta **uhka**hallinta, **käytännön** \> **Turvalliset liitetiedostot**.</span><span class="sxs-lookup"><span data-stu-id="6cf20-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="6cf20-106">Valitse **ATP SharePoint, OneDrive-ja Microsoft-ryhmien käyttöön**.</span><span class="sxs-lookup"><span data-stu-id="6cf20-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="6cf20-107">Saat ilmoituksen, kun emme tunnista haittaohjelmien tiedostot [luoda hälytyksen käytännön toimintaa](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) .</span><span class="sxs-lookup"><span data-stu-id="6cf20-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="6cf20-108">Täydelliset ohjeet Katso tätä [aihetta](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="6cf20-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="6cf20-109">**Huomautus**: tarkoituksellista, ATP ei Etsi kaikki yhteen tiedostoon, SharePoint Online, OneDrive työ tai Microsoftin Teams.</span><span class="sxs-lookup"><span data-stu-id="6cf20-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="6cf20-110">Tiedostot tarkistetaan asynkronisesti prosessi, joka käyttää Vieras tehtävän jakaminen toiminnan ja uhka signaaleja, Määritä vahingollisia tiedostoja.</span><span class="sxs-lookup"><span data-stu-id="6cf20-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="6cf20-111">Lisätietoja Katso tätä [aihetta](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="6cf20-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
