---
title: Saapuneet-kansion sääntöaktiviteetin tunnistaminen valvontalokeissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716421"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="c8030-102">Saapuneet-kansion sääntöaktiviteetin tunnistaminen valvontalokeissa</span><span class="sxs-lookup"><span data-stu-id="c8030-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="c8030-103">Microsoft 365 Security & Compliance Centerin valvontalokihaun avulla voit tarkastella Saapuneet-kansion sääntötapahtumia (Saapuneet-kansion sääntöjen luominen, muokkaaminen ja poistaminen).</span><span class="sxs-lookup"><span data-stu-id="c8030-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="c8030-104">Kirjaudu Microsoft [365 Security & Compliance Centeriin.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="c8030-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="c8030-105">Siirry **Haun** > **valvontalokin hakusivulle.**</span><span class="sxs-lookup"><span data-stu-id="c8030-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="c8030-106">Valitse päivämääräväli **Aloituspäivä-** ja **Päättymispäivä-kentissä.**</span><span class="sxs-lookup"><span data-stu-id="c8030-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="c8030-107">Tarkista **Exchange-postilaatikkoaktiviteetit**-kohdassa, että **Aktiviteetit-kentän** arvoksi on määritetty **Uusi Saapuneet-kansion sääntö Luo/muokkaa/ota käyttöön tai poista käytöstä .**</span><span class="sxs-lookup"><span data-stu-id="c8030-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="c8030-108">Valitse **Hae**.</span><span class="sxs-lookup"><span data-stu-id="c8030-108">Click **Search**.</span></span>

<span data-ttu-id="c8030-109">Valitse tuloksista valvontatietue.</span><span class="sxs-lookup"><span data-stu-id="c8030-109">In the results, select an audit record.</span></span> <span data-ttu-id="c8030-110">Valitse tiedot-pikaikkunassa **Lisätietoja**.</span><span class="sxs-lookup"><span data-stu-id="c8030-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="c8030-111">Saapuneet-kansion säännön asetusten tiedot näkyvät **Parametrit-kentässä.**</span><span class="sxs-lookup"><span data-stu-id="c8030-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="c8030-112">Lisätietoja on [ohjeaiheessa Sen määrittäminen, onko käyttäjä luonut Saapuneet-kansion säännön](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="c8030-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
