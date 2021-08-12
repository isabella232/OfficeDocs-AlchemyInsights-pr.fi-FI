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
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946612"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Työpöytäanalyysin käyttöönottaessa tapahtui tunnuksen kelvollinenvirhe -virhe

Tämä virhe ilmenee yleensä, kun todennustunnus vanhenee. Yleensä sivun päivittäminen päivittää tunnuksen. Ongelma voi kuitenkin jatkua, jos taulutietokoneen työpöytäanalyysissa käytettävässä tilissä on käytössä ehdollisia käyttöoikeuskäytäntöjä. Voit tarkastella Azure AD:n kirjautumislokeja Azure-portaalissa ja tarkistaa, onko työpöytäanalyysin käyttöön otettavassa tilissä kirjautumisvirheitä.

Saat lisätietoja ehdollisesta käyttöomme ista [ehdollisen käyttöoikeuden käyttöönoton suunnitteleminen -kohdassa.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)