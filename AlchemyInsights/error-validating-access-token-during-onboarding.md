---
title: Käyttötunnusvirheen kelvollinen tapahtui työpöytäanalyysin käytön aikana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813685"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="c998c-102">Työpöytäanalyysin käyttöönottaessa tapahtui tunnuksen kelvollinenvirhe -virhe</span><span class="sxs-lookup"><span data-stu-id="c998c-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="c998c-103">Tämä virhe ilmenee yleensä, kun todennustunnus vanhenee.</span><span class="sxs-lookup"><span data-stu-id="c998c-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="c998c-104">Yleensä sivun päivittäminen päivittää tunnuksen.</span><span class="sxs-lookup"><span data-stu-id="c998c-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="c998c-105">Ongelma voi kuitenkin jatkua, jos taulutietokoneen työpöytäanalyysissa käytettävässä tilissä on käytössä ehdollisia käyttöoikeuskäytäntöjä.</span><span class="sxs-lookup"><span data-stu-id="c998c-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="c998c-106">Voit tarkastella Azure AD:n kirjautumislokeja Azure-portaalissa ja tarkistaa, onko työpöytäanalyysin käyttöön otettavassa tilissä kirjautumisvirheitä.</span><span class="sxs-lookup"><span data-stu-id="c998c-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="c998c-107">Saat lisätietoja ehdollisesta käyttöomme ista [ehdollisen käyttöoikeuden käyttöönoton suunnitteleminen -kohdassa.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="c998c-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>