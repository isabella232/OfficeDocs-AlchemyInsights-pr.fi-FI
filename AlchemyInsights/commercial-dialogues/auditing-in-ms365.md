---
title: Valvonta Microsoft 365:ssä
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481599"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="24593-102">Valvonta Microsoft 365:ssä</span><span class="sxs-lookup"><span data-stu-id="24593-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="24593-103">Seuraavassa on muutamia asioita, jotka kannattaa tietää Microsoft 365:n tarkastuksesta:</span><span class="sxs-lookup"><span data-stu-id="24593-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="24593-104">Exchange-järjestelmänvalvojan toiminnot valvotaan oletusarvoisesti.</span><span class="sxs-lookup"><span data-stu-id="24593-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="24593-105">Postilaatikon valvonta on oletusarvoisesti käytössä kaikille käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="24593-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="24593-106">Jos haluat lisätietoja tästä, napsauta [tätä.](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171)</span><span class="sxs-lookup"><span data-stu-id="24593-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="24593-107">Siihen asti, jos haluat, että ohjeet otetaan käyttöön manuaalisesti yhdelle henkilölle tai koko organisaatiolle, valitse alla oleva Ota postilaatikon valvonta käyttöön -painike.</span><span class="sxs-lookup"><span data-stu-id="24593-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="24593-108">Microsoft 365 -ryhmien postilaatikot ja yleisen kansion postilaatikot eivät tue valvontalokiin kirjaamista.</span><span class="sxs-lookup"><span data-stu-id="24593-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="24593-109">SharePointin/OneDriven valvonta ei vaadi lisämäärityksiä.</span><span class="sxs-lookup"><span data-stu-id="24593-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="24593-110">Lisätietoja valvotuista toiminnoista on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="24593-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="24593-111">Tiedostotoiminnot</span><span class="sxs-lookup"><span data-stu-id="24593-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="24593-112">Kansiotoiminnot</span><span class="sxs-lookup"><span data-stu-id="24593-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="24593-113">[Jakamis- ja käyttötoiminnot.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)</span><span class="sxs-lookup"><span data-stu-id="24593-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="24593-114">Luettelo kaikista valvotuista toiminnoista palvelun mukaan on kohdassa [Valvotut toiminnot.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)</span><span class="sxs-lookup"><span data-stu-id="24593-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
