---
title: Ovatko käyttäjät saaneet haitallisia sähköpostiviestejä?
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326663"
---
# <a name="did-your-users-receive-malicious-email"></a>Ovatko käyttäjät saaneet haitallisia sähköpostiviestejä?

Voit nyt raportoida vahingollisen sähköpostin Microsoftille käyttämällä [lähetykset Microsoft 365 Defender portaalissa.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Järjestelmänvalvojien [ilmoituksiin lähetetyt](https://security.microsoft.com/reportsubmission?viewid=admin) viestit tarkistetaan ja yksityiskohtaisen pikaikkunan alla näkyvät tulokset:

- Jos lähettäjän sähköpostin todennus epäonnistui toimituksen aikana.
- Tietoja kaikista käytäntöosumista, jotka ovat voineet vaikuttaa viestin päätökseen tai ohittaa sen.
- Nykyiset tarkistustulokset, joista selviää, ovatko viestin URL-osoitteet tai tiedostot haitallisia.
- Palaute arvostelijoilta

Tarkistus suoritetaan uudelleen usean minuutin sisällä, jos ohitus löytyy. Palautteessa voi kestää korkeintaan vuorokausi, jos sähköpostin todentamisessa ei ollut ongelmia tai ohitus ei vaikuttanut toimitukseen.

Lähetä viesti uudelleen vuorokauden kuluttua tarkistusta varten, jos olet eri mieltä viestin, URL-osoitteen tai tiedoston (estetty tai ei estetty) lopullisesta päätöksestä. On mahdollista, että päätös muuttuu viestin uudelleen lähettämisen jälkeen.

Tällä välin voit poistaa haitallisia sähköpostiviestejä käyttäjien Saapuneet-kansioista noudattamalla [tämän artikkelin ohjeita](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Office 365:n Microsoft Defenderin asiakkaat voivat:
  - Epäilyttävien [sähköpostiviestien etsiminen ja poistaminen Threat Explorerilla](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Haitallisen URL Lokero n käytön estäminen linkit-linkin](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) avulla
  - Seuraa käyttäjiä, jotka napsauttit ja kävivät käsiksi haitallisiin URL-osoitteisiin: Tarkastele tietojen kalastelun URL-osoitetta ja valitse [verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)  &  [Get-URLTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Automaattisen tutkimuksen [käynnistäminen manuaalisesti](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Voit myös suojautua haitallisia URL-osoitteita ja tiedostoja vastaan noudattamalla näitä ohjeita:[Suojaus haitallisilta URL-osoitteilta ja tiedostoilta](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
