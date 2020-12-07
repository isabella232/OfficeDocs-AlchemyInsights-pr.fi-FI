---
title: Mitä tehdä, jos Azure-ominaisuudet eivät toimi oikein Microsoft Edgessä
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583463"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="8eed3-102">Mitä tehdä, jos Azure-ominaisuudet eivät toimi oikein Microsoft Edgessä</span><span class="sxs-lookup"><span data-stu-id="8eed3-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="8eed3-103">Microsoft Edgessä on [tunnettuja ongelmia](https://go.microsoft.com/fwlink/?linkid=2140608) , jotka liittyvät turva vyöhykkeisiin ja saattavat vaikuttaa siihen, miten Azure-käyttäjät kirjautuvat Windows Admin Centeriin.</span><span class="sxs-lookup"><span data-stu-id="8eed3-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="8eed3-104">Jos sinulla on ongelmia Azure-ominaisuuksien käyttämisessä Microsoft Edgessä, kokeile seuraavia vaiheita:</span><span class="sxs-lookup"><span data-stu-id="8eed3-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="8eed3-105">Etsi **Käynnistä** -valikosta **Internet-asetukset** ja valitse se.</span><span class="sxs-lookup"><span data-stu-id="8eed3-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="8eed3-106">Valitse **Internet-ominaisuudet** -valinta ikkunassa **turvallisuus** -väli lehti.</span><span class="sxs-lookup"><span data-stu-id="8eed3-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="8eed3-107">Valitse **Luotetut sivustot** -vyöhyke ja valitse sitten **sivustot** -painike.</span><span class="sxs-lookup"><span data-stu-id="8eed3-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="8eed3-108">Lisää **Luotetut sivustot** -valinta ikkunaan yhdyskäytävän URL-osoite sekä [https://login.microsoftonline.com](https://login.microsoftonline.com) ja ja [https://login.live.com](https://login.live.com) Valitse sitten **Sulje**.</span><span class="sxs-lookup"><span data-stu-id="8eed3-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="8eed3-109">Valitse **Internet-ominaisuudet** -valinta ikkunassa **tieto suoja** -väli lehti.</span><span class="sxs-lookup"><span data-stu-id="8eed3-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="8eed3-110">Valitse **ponnahdus ikkunoiden esto-** osassa **Asetukset**.</span><span class="sxs-lookup"><span data-stu-id="8eed3-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="8eed3-111">Lisää avautuvaan valinta ikkunaan yhdyskäytävän URL-osoite sekä [https://login.microsoftonline.com](https://login.microsoftonline.com) ja ja [https://login.live.com](https://login.live.com) Valitse sitten **Sulje**.</span><span class="sxs-lookup"><span data-stu-id="8eed3-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
