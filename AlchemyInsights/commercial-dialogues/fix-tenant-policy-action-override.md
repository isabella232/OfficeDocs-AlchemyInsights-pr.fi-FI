---
title: Vuokraajan käytännön korjauksen (toiminnon ohittaminen)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745885"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="8adfe-102">Vuokraajan käytännön korjauksen (toiminnon ohittaminen)</span><span class="sxs-lookup"><span data-stu-id="8adfe-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="8adfe-103">Tämä sanoma vaikuttaa vuokraajan roskapostin estokäytäntöön.</span><span class="sxs-lookup"><span data-stu-id="8adfe-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="8adfe-104">Voit tarkistaa käytännön seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="8adfe-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="8adfe-105">Siirry [Office 365:n tietoturva- & yhteensopivuuskeskukseen](https://go.microsoft.com/fwlink/p/?linkid=2077143)ja siirry sitten **uhkien**  >  **hallintakäytäntöön**  >  [roskapostin estoon.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="8adfe-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="8adfe-106">Tarkista, onko **käytäntölähde** ilmaise seuraavaa:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span><span class="sxs-lookup"><span data-stu-id="8adfe-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="8adfe-107">Jos näin on, tarkista Mukautetut-välilehdessä sen käytännön asetukset, johon viesti vaikuttaa. </span><span class="sxs-lookup"><span data-stu-id="8adfe-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="8adfe-108">On mahdollista, että  kaikkiin Exchange Online Protection -asiakkaisiin sovellettiin vakioasetuksia, joihin viesti vaikuttaa.</span><span class="sxs-lookup"><span data-stu-id="8adfe-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="8adfe-109">Lisätietoja roskapostin suodatuskäytäntöjen määrittämisestä on kohdassa [Roskapostisuodatinkäytäntöjen määrittäminen.](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="8adfe-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
