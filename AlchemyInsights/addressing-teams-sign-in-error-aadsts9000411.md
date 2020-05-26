---
title: Ryhmien kirjautumisvirheen käsitteleminen AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357550"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Ryhmien kirjautumisvirheen käsitteleminen AADSTS9000411

Kun kirjaudut Microsoft Teamsiin, näyttöön saattaa tulla virhe: **Valitettavasti sinulla on ongelmia kirjautumisessa AADSTS9000411: Pyyntöä ei ole muotoiltu oikein. Parametri "login_hint" on monistettu.**

Voit korjata tämän ongelman varmistamalla, että Microsoft Teams -asiakkaasi päivitetään. Lisätietoja asiakkaan päivittämisestä on ohjeaiheessa [Microsoft Teamsin päivittäminen](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Jos asiakasohjelmaa ei jostain syystä voi päivittää, asiakkaan uloskirjautuminen tyhjentää useimmat välimuistissa olevat tiedot. Jos sinulla on kuitenkin ongelmia uloskirjautumisen/kirjautumisen jälkeen, sulje Teams ja tyhjennä asiakasvälimuisti seuraavasti:
1. Sulje Microsoft Teams.
2. Siirry kohtaan: %appdata%\microsoft\teams ja poista kaikki tiedostot.
3. Avaa Microsoft Teams uudelleen.
