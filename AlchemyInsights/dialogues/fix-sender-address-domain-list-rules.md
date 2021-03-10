---
title: Lähettäjän osoitteen tai toimialueen luettelon sääntöjen ratkaiseminen
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
ms.openlocfilehash: a57016ce0b5e8ed741889a50e3858c68578c6713
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694303"
---
# <a name="fix-sender-addressdomain-list-rules"></a><span data-ttu-id="234b6-102">Lähettäjän osoitteen tai toimialueen luettelon sääntöjen ratkaiseminen</span><span class="sxs-lookup"><span data-stu-id="234b6-102">Fix Sender Address/Domain list rules</span></span>

<span data-ttu-id="234b6-103">Tämä viesti vaikuttaa vuokraajan roskapostin estokäytäntöön.</span><span class="sxs-lookup"><span data-stu-id="234b6-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="234b6-104">Viestin lähettäjä löytyi Sallittu- tai Estä-luettelosta.</span><span class="sxs-lookup"><span data-stu-id="234b6-104">The sender of the message was found in an Allow or Block list.</span></span> <span data-ttu-id="234b6-105">Voit tarkistaa käytännön seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="234b6-105">To review the policy, do the following:</span></span>

1. <span data-ttu-id="234b6-106">Siirry [Office 365:n tietoturva- & yhteensopivuuskeskukseen](https://go.microsoft.com/fwlink/p/?linkid=2077143)ja siirry sitten **uhkien**  >  **hallintakäytäntöön**  >  [roskapostin estoon.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="234b6-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="234b6-107">Jos **vakioasetukset** on otettu käyttöön, **valitse** Vakio-välilehdessä Salli **luettelot ja** **Estä luettelot.**</span><span class="sxs-lookup"><span data-stu-id="234b6-107">On the **Standard** tab, if **Standard settings** is enabled, check the **Allow lists** and **Block lists**.</span></span>
3. <span data-ttu-id="234b6-108">Jos **Mukautetut asetukset**  on otettu käyttöön Mukautettu-välilehdessä, tarkista käytännöt valitsemalla Muokkaa käytäntöä ja valitsemalla **Salli-luettelot** ja **Esto-luettelot.** </span><span class="sxs-lookup"><span data-stu-id="234b6-108">On the **Custom** tab, if the **Custom settings** is enabled, review the policies by selecting **Edit policy** and checking the **Allow lists** and **Block lists**.</span></span>

<span data-ttu-id="234b6-109">Lisätietoja roskapostin suodatuskäytäntöjen määrittämisestä on kohdassa [Roskapostisuodatinkäytäntöjen määrittäminen.](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="234b6-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
