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
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929194"
---
# <a name="did-your-users-receive-malicious-email"></a>Ovatko käyttäjät saaneet haitallisia sähköpostiviestejä?

- Voit nyt raportoida haitalliset sähköpostiviestit Microsoftille käyttämällä [järjestelmänvalvojan viestejä tietoturva- ja yhteensopivuuskeskukselle](https://sip.protection.office.com/reportsubmission).

Tiedot, jotka lähetetään [järjestelmänvalvojan viesteinä](https://sip.protection.office.com/reportsubmission) tarkistetaan, ja tulokset näkyvät pikaikkunassa **lisätiedot**:

- Jos lähettäjän sähköpostin todennus epäonnistui toimituksen aikana.
- Tietoja kaikista käytäntöosumista, jotka ovat voineet vaikuttaa viestin päätökseen tai ohittaa sen.
- Nykyiset tarkistustulokset, joista selviää, ovatko viestin URL-osoitteet tai tiedostot haitallisia.
- Palaute arvostelijoilta

Tarkistus suoritetaan uudelleen usean minuutin sisällä, jos ohitus löytyy. Palautteessa voi kestää korkeintaan vuorokausi, jos sähköpostin todentamisessa ei ollut ongelmia tai ohitus ei vaikuttanut toimitukseen.

Lähetä viesti uudelleen vuorokauden kuluttua tarkistusta varten, jos olet eri mieltä viestin, URL-osoitteen tai tiedoston (estetty tai ei estetty) lopullisesta päätöksestä. On mahdollista, että päätös muuttuu viestin uudelleen lähettämisen jälkeen.

Tällä välin voit poistaa haitallisia sähköpostiviestejä käyttäjien Saapuneet-kansioista noudattamalla [tämän artikkelin ohjeita](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Office 365:n Microsoft Defenderin asiakkaat voivat:
    - käyttää [Threat Exploreria epäilyttävien sähköpostiviestien etsimiseen ja poistamiseen](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [käyttää Turvallisia linkkejä estämään](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) haitallisten URL-osoitteiden käytön
    - jäljittää käyttäjät, jotka napsauttivat haitallisia URL-osoitteita:[Tietojenkalastelun URL-osoitteet ja napsautustiedot](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Hanki URL-seuranta](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - aloittaa manuaalisesti [automatisoitu tutkimus](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Voit myös suojautua haitallisia URL-osoitteita ja tiedostoja vastaan noudattamalla näitä ohjeita:[Suojaus haitallisilta URL-osoitteilta ja tiedostoilta](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).