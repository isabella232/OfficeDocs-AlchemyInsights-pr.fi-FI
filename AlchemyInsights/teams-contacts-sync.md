---
title: Teams synkronoiminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004610"
- "11540"
ms.openlocfilehash: 0ffa91f0e31a4904db87f0df6d9b4c51b05ae2758a5ce0d96c77ef4456f6d033
ms.sourcegitcommit: 71501cde5bcb73f4dcf23944d400a4db10f37033
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/09/2021
ms.locfileid: "57814210"
---
# <a name="teams-contacts-sync"></a>Teams synkronoiminen

Teams käyttää organisaation Active Directory -yhteystietoja ja käyttäjän oletuskansioon Outlook yhteystietoja. Jos yhteystiedot eivät näy Microsoft Teams, kokeile seuraavaa:

**Huomautus:** Jos yhden tai useamman yhteystiedon tiedot on äskettäin päivitetty, yhteystietojen synkronointi voi kestää jopa 48 tuntia.

1. Kirjaudu ulos Teams uudelleen. Tarkista, näkyykö yhteystiedot.
1. Tyhjennä Teams välimuisti:
    1. Siirry kansioon **%appdata%\Microsoft\Teams**.
    1. Poista kansion sisältö.
    1. Käynnistä tietokone uudelleen ja käynnistä Teams.
1. Jos yhteyshenkilö on Outlook, muista lisätä se yhteystietoluetteloon. Valitse Outlook-kohdassa osoiteriviltä **Tiedosto** ja valitse sitten **Lisää yhteystietoihin**.
1. Varmista, että käyttäjän Exchange on isännöity verkossa (ei paikallinen). Lisätietoja on kohdassa Miten [Exchange ja Microsoft Teams toimia.](/microsoftteams/exchange-teams-interact)
1. Varmista, että yhteyshenkilön puhelinnumero on lisätty yhteystietoihin.
1. Hae yhteyshenkilön sähköpostiviestejä hakupalkissa. Yhteystiedot, jotka voit noutaa yhteystietoluetteloon synkronoitaessa.
