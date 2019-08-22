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
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539162"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="69cc1-102">Määritä Saapuneet-kansion säännön toimintaa seurantalokeja</span><span class="sxs-lookup"><span data-stu-id="69cc1-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="69cc1-103">Compliance Centerin Office 365 Security-& valvonta kirjaa haun avulla voit tarkastella Saapuneet-kansion säännön tapahtumat (luominen, muokkaaminen ja poistaminen Saapuneet-kansion sääntöjä).</span><span class="sxs-lookup"><span data-stu-id="69cc1-103">You can use audit log search in the Office 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="69cc1-104">Kirjautua sisään [Office 365 & noudattamista Tietoturvakeskus](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="69cc1-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="69cc1-105">Siirry **Etsinnän** > **Audit log** etsintäsivun.</span><span class="sxs-lookup"><span data-stu-id="69cc1-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="69cc1-106">Valitse **aloituspäivä** - ja **päättymispäivä** -kenttiin päivämääräalue.</span><span class="sxs-lookup"><span data-stu-id="69cc1-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="69cc1-107">Tarkista kohdasta **Exchange-postilaatikon toimintaa** **toimintaa** -kentän arvo on **Uusi-InboxRule Luo/Muokkaa/käyttöön/poistaa käytöstä Saapuneet-kansion sääntö**.</span><span class="sxs-lookup"><span data-stu-id="69cc1-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="69cc1-108">Valitse **Etsi**.</span><span class="sxs-lookup"><span data-stu-id="69cc1-108">Click **Search**.</span></span>

<span data-ttu-id="69cc1-109">Valitse tulosten koskeva seurantatietue.</span><span class="sxs-lookup"><span data-stu-id="69cc1-109">In the results, select an audit record.</span></span> <span data-ttu-id="69cc1-110">Valitse tiedot-valikon avauspainike **Lisätietoja**.</span><span class="sxs-lookup"><span data-stu-id="69cc1-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="69cc1-111">Lisätietoja Saapuneet-kansion säännön **Parametrit** -kentässä näkyy.</span><span class="sxs-lookup"><span data-stu-id="69cc1-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="69cc1-112">Saat lisätietoja, [Jos käyttäjän luoman luodun säännön Saapuneet-kansion määrittäminen](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="69cc1-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
