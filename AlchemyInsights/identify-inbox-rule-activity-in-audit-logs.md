---
title: Määritä Saapuneet-kansion säännön toimintaa seurantalokeja
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755035"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="68329-102">Määritä Saapuneet-kansion säännön toimintaa seurantalokeja</span><span class="sxs-lookup"><span data-stu-id="68329-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="68329-103">Suojauksen & Compliance Centeriin audit log haun avulla voit tarkastella Saapuneet-kansion säännön tapahtumat (luominen, muokkaaminen ja poistaminen Saapuneet-kansion sääntöjä).</span><span class="sxs-lookup"><span data-stu-id="68329-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="68329-104">Kirjautua [Office 365-suojauksen & Compliance Centeriin](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="68329-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="68329-105">**Etsi ja tutkimus** ja valitse **Valvo lokista etsintää**.</span><span class="sxs-lookup"><span data-stu-id="68329-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="68329-106">Valitse **aloituspäivä** - ja **päättymispäivä** -kenttiin päivämääräalue.</span><span class="sxs-lookup"><span data-stu-id="68329-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="68329-107">Tarkista kohdasta **Exchange-postilaatikon toimintaa** **toimintaa** -kentän arvo on **Uusi-InboxRule Luo/Muokkaa/käyttöön/poistaa käytöstä Saapuneet-kansion sääntö**.</span><span class="sxs-lookup"><span data-stu-id="68329-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="68329-108">Valitse **Etsi**.</span><span class="sxs-lookup"><span data-stu-id="68329-108">Click **Search**.</span></span>

<span data-ttu-id="68329-109">Valitse tulosten koskeva seurantatietue.</span><span class="sxs-lookup"><span data-stu-id="68329-109">In the results, select an audit record.</span></span> <span data-ttu-id="68329-110">Valitse tiedot-valikon avauspainike **Lisätietoja**.</span><span class="sxs-lookup"><span data-stu-id="68329-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="68329-111">Lisätietoja Saapuneet-kansion säännön **Parametrit** -kentässä näkyy.</span><span class="sxs-lookup"><span data-stu-id="68329-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="68329-112">Saat lisätietoja, [Jos käyttäjän luoman luodun säännön Saapuneet-kansion määrittäminen](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="68329-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
