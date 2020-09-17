---
title: Saapuneet-kansion säännön aktiviteetin määrittäminen valvonta lokeissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779048"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="ea6fe-102">Saapuneet-kansion säännön aktiviteetin määrittäminen valvonta lokeissa</span><span class="sxs-lookup"><span data-stu-id="ea6fe-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="ea6fe-103">Voit käyttää valvonta loki hakua Microsoft 365-tieto turva & yhteensopivuus keskuksessa, jos haluat tarkastella Saapuneet-kansion säännön tapahtumia (Saapuneet-kansion sääntöjen luominen, muokkaaminen ja poistaminen).</span><span class="sxs-lookup"><span data-stu-id="ea6fe-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="ea6fe-104">Kirjaudu sisään [Microsoft 365-tieto turva & Compliance Centeriin](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ea6fe-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ea6fe-105">Siirry **haun**  >  **valvonta lokien haku** sivulle.</span><span class="sxs-lookup"><span data-stu-id="ea6fe-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="ea6fe-106">Valitse päivämäärä väli **alkamis päivä** -ja **päättymis päivä** -kenttiin.</span><span class="sxs-lookup"><span data-stu-id="ea6fe-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="ea6fe-107">Tarkista **Exchange-posti laatikon aktiviteetit**-kohdassa **aktiviteetit** -kentän arvoksi on valittu **New-inboxrule Luo/Muokkaa/Ota käyttöön tai Poista käytöstä Saapuneet-kansion sääntö**.</span><span class="sxs-lookup"><span data-stu-id="ea6fe-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="ea6fe-108">Valitse **Hae**.</span><span class="sxs-lookup"><span data-stu-id="ea6fe-108">Click **Search**.</span></span>

<span data-ttu-id="ea6fe-109">Valitse tulokset-kohdassa valvonta tietue.</span><span class="sxs-lookup"><span data-stu-id="ea6fe-109">In the results, select an audit record.</span></span> <span data-ttu-id="ea6fe-110">Valitse tiedot-valikosta **lisä tietoja**.</span><span class="sxs-lookup"><span data-stu-id="ea6fe-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="ea6fe-111">Tietoja Saapuneet-kansion säännön asetuksista näkyy **Parametrit** -kentässä.</span><span class="sxs-lookup"><span data-stu-id="ea6fe-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="ea6fe-112">Lisä tietoja on kohdassa [sen määrittäminen, onko käyttäjä luonut Saapuneet-kansion säännön](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="ea6fe-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
