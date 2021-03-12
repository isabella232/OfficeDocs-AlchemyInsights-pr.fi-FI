---
title: Office 365:n Microsoft Defenderin yleisimmät ongelmat
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
ms.openlocfilehash: 05fa518ece7ea40fd7b4cea57115d9cd60370b01
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746824"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a><span data-ttu-id="53e89-102">Office 365:n Microsoft Defenderin yleisimmät ongelmat</span><span class="sxs-lookup"><span data-stu-id="53e89-102">Fix common problems with Microsoft Defender for Office 365</span></span>

<span data-ttu-id="53e89-103">Seuraavassa on joitakin ratkaisuja yleisiin Office 365:n Microsoft Defenderin ongelmiin:</span><span class="sxs-lookup"><span data-stu-id="53e89-103">Here are some solutions to common problems with Microsoft Defender for Office 365:</span></span>

- <span data-ttu-id="53e89-104">**Viestin viive:** Jos sinulla on ongelmia, joissa viestin toimitus viivästyy,  sinun on käytettävä Turvallisten liitteiden käytännön Dynaaminen toimitus -asetuksia.</span><span class="sxs-lookup"><span data-stu-id="53e89-104">**Message delay:** If you're experiencing issues where message delivery is delayed, you'll want to use the **Dynamic Delivery** options within your Safe Attachments policy.</span></span> <span data-ttu-id="53e89-105">Lisätietoja on kohdassa Dynaaminen [toimitus turvallisten liitteiden käytännöistä.](https://go.microsoft.com/fwlink/?linkid=2094106)</span><span class="sxs-lookup"><span data-stu-id="53e89-105">To learn more, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2094106).</span></span>
- <span data-ttu-id="53e89-106">**Virheellisten positiivisten tai negatiivisten tulosten raportoiminen:** Ilmoita viestistä Microsoftille tämän linkin avulla: [Microsoft Defender Response Portal.](https://go.microsoft.com/fwlink/?linkid=2092835)</span><span class="sxs-lookup"><span data-stu-id="53e89-106">**Report false positive or negative results:** Report the message to Microsoft using this link: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835).</span></span>
- <span data-ttu-id="53e89-107">**Ota turvallinen linkkisuojaus käyttöön:**</span><span class="sxs-lookup"><span data-stu-id="53e89-107">**Enable Safe Link protection:**</span></span>
    1. <span data-ttu-id="53e89-108">Kirjaudu Office [365:n tietoturva- & yhteensopivuuskeskukseen.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="53e89-108">Sign in to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
    2. <span data-ttu-id="53e89-109">Siirry **uhkien**  >  **hallintakäytännön**  >  **turvallisten linkkien ohjeisiin.**</span><span class="sxs-lookup"><span data-stu-id="53e89-109">Go to **Threat Management** > **Policy** > **Safe Links.**</span></span>
    3. <span data-ttu-id="53e89-110">Avaa **määritetty käytäntö tiettyihin vastaanottajiin** sovellettavassa käytännöt-kohdassa.</span><span class="sxs-lookup"><span data-stu-id="53e89-110">Under **Policies that apply to specific recipients**, open the policy configured.</span></span>
    4. <span data-ttu-id="53e89-111">Valitse **Asetukset-kohdassa** **Käytä turvallisia linkkejä organisaatiossa lähetetyissä viesteissä.**</span><span class="sxs-lookup"><span data-stu-id="53e89-111">Under **Settings**, select **Apply safe links to messages sent within the organization**.</span></span>
