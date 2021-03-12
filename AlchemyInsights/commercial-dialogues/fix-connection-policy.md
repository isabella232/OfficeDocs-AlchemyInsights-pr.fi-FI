---
title: Yhteyskäytännön ratkaiseminen
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746753"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="7c956-102">Yhteyskäytännön ratkaiseminen</span><span class="sxs-lookup"><span data-stu-id="7c956-102">Fix connection policy</span></span>

<span data-ttu-id="7c956-103">Sähköposti on merkitty turvalliseksi ja toimitettu käyttäjän Saapuneet-kansioon, koska lähettävä IP-osoite on merkitty turvalliseksi Yhteyssuodatin-käytännön avulla.</span><span class="sxs-lookup"><span data-stu-id="7c956-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="7c956-104">Voit tarkistaa käytännön seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="7c956-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="7c956-105">Siirry [Office 365:n tietoturva- & yhteensopivuuskeskukseen](https://go.microsoft.com/fwlink/p/?linkid=2077143)ja siirry sitten **uhkien**  >  **hallintakäytäntöön**  >  [roskapostin estoon.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="7c956-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="7c956-106">Valitse **Mukautettu-välilehdessä** **Yhteyssuodatin-käytäntö** ja valitse sitten **Muokkaa käytäntöä.**</span><span class="sxs-lookup"><span data-stu-id="7c956-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="7c956-107">Tarkista **SALLITTUJEN IP-osoitteiden** luettelo.</span><span class="sxs-lookup"><span data-stu-id="7c956-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="7c956-108">Katso, **onko turvallinen luettelo** käytössä.</span><span class="sxs-lookup"><span data-stu-id="7c956-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="7c956-109">Microsoft tilaa luotettavien lähettäjien kolmannen osapuolen lähteitä.</span><span class="sxs-lookup"><span data-stu-id="7c956-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="7c956-110">Jos **turvallinen luettelo** on käytössä, näitä luotettavia lähettäjiä ei merkitä vahingossa roskapostiksi.</span><span class="sxs-lookup"><span data-stu-id="7c956-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="7c956-111">Suosittelemme tämän asetuksen valitsemista, koska se vähentää vastaanottamiasi virheellisiä positiivisia viestejä (roskapostiksi luokiteltuja hyviä viestejä).</span><span class="sxs-lookup"><span data-stu-id="7c956-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
