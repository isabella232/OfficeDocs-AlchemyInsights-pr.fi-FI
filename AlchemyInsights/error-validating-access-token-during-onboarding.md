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
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Työpöytäanalyysin käyttöönottaessa tapahtui tunnuksen kelvollinenvirhe -virhe

Tämä virhe ilmenee yleensä, kun todennustunnus vanhenee. Yleensä sivun päivittäminen päivittää tunnuksen. Ongelma voi kuitenkin jatkua, jos taulutietokoneen työpöytäanalyysissa käytettävässä tilissä on käytössä ehdollisia käyttöoikeuskäytäntöjä. Voit tarkastella Azure AD:n kirjautumislokeja Azure-portaalissa ja tarkistaa, onko työpöytäanalyysin käyttöön otettavassa tilissä kirjautumisvirheitä.

Saat lisätietoja ehdollisesta käyttöomme ista [ehdollisen käyttöoikeuden käyttöönoton suunnitteleminen -kohdassa.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)