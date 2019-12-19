---
title: Virhe tarkistettaessa käyttö tunnus virhettä Desktop Analyticsin aikana-lennolle
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741166"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Virhe tarkistettaessa käyttö tunnus sanomaa"-virhe Desktop Analyticsin perehdytys-toiminnon aikana

Tämä virhe havaitaan normaalisti, kun todennus tunnus vanhenee. Yleensä sivun päivittäminen päivittää tunnuksen. Tämä ongelma voi kuitenkin jatkua, jos ehdolliseen käyttöön liittyvät käytännöt on käytetty tilillä, jota käytetään tieto kone analytiikan käytössä. Voit tarkastella Azure AD Sign in-lokeja Azure-portaalissa ja tarkistaa, onko tilillä kirjautumisvirheitä, joita käytetään Desktop Analyticsin perehdytys-kohdassa.

Lisä tietoja ehdollisesta käyttö oikeus-kohdasta on [Suunnittele ehdollisen käytön käyttöönotto](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).