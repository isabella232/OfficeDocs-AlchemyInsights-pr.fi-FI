---
title: Virhe tarkistettaessa tuki tunnus virhettä Työpöytä tietojen analysoinnin aikana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783548"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="a430e-102">Virhe tarkistettaessa käyttö oikeus tunnusta-virhe Työpöytä analytiikan aikana</span><span class="sxs-lookup"><span data-stu-id="a430e-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="a430e-103">Tämä virhe havaitaan tavallisesti, kun todennus tunnus vanhenee.</span><span class="sxs-lookup"><span data-stu-id="a430e-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="a430e-104">Yleensä sivun päivittäminen päivittää tunnuksen.</span><span class="sxs-lookup"><span data-stu-id="a430e-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="a430e-105">Tämä ongelma voi kuitenkin jatkua, jos käytössä on muita ehdollisen käyttö oikeuden käytäntöjä, joita käytetään taulu tieto koneen Työpöytä analytiikkaan käytettävän tilin yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="a430e-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="a430e-106">Voit tarkistaa Azure-mainosten kirjautumislokit Azure-portaalissa, jotta näet, onko tilin Työpöytä analytiikkaan kirjautumiseen käytettävää tiliä varten kirjautumisvirheitä.</span><span class="sxs-lookup"><span data-stu-id="a430e-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="a430e-107">Lisä tietoja ehdollisesta käyttö oikeus-kohdasta on Ohje aiheessa [ehdollisen käytön käyttöönoton suunnitteleminen](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="a430e-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>