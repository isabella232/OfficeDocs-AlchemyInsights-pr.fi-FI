---
title: Tarvitseeko sinun merkitä toimialue tai sähköpostin lähettäjä turvalliseksi?
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
- "9002921"
- "5673"
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319945"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Tarvitseeko sinun merkitä toimialue tai sähköpostin lähettäjä turvalliseksi?

- Turvallisten **lähettäjien luetteloiden käyttöä** ei suositella, koska se avaa organisaatiosi roskaposti-, osoite- ja osoitetushyökkäyksille.
- Jos kyse on liiketoiminnan vaatimuksesta, suosittelemme **kuitenkin** käyttämään **[tähän Flow sähköpostisääntöjä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Ohjeemme varmistavat lähettäjän todennuksen (varmistaa, että toimialueen lähetystä ei osoiteta). 
    **Huomautus:** Emme suosittele virheellisten positiivisten tietojen hallintaa turvallisten lähettäjien luetteloiden avulla, koska roskapostisuodatuksen poikkeukset voivat avata organisaatiosi suojaushyökkäyksiin. Jos käyttäjäsi saavat viestit, jotka on merkitty virheellisesti roskapostiksi, Ilmoita viesteistä ja **[tiedostoista Microsoftille.](https://protection.office.com/reportsubmission)**
- Lokero Roskapostin estokäytäntöjen lähettäjät, Outlook, Sallittujen lähettäjien  luettelot tai sallittujen toimialueiden luettelot on syytä välttää, koska lähettäjät ohittavat kaiken roskapostin, tekeutumisen ja tietojen estosuojauksen sekä lähettäjän todennuksen (SPF, DKIM, DMARC). Tätä menetelmää käytetään parhaiten vain tilapäistesteissä.
- Vahvistus, jonka mukaan tietty sähköposti ohitettu Roskapostin arviointi voidaan tehdä tarkistamalla viestin otsikko X-Forefront-Antispam-Report (SFV:SFE, SFV:SKA, SFV:SKN), katso roskapostiviestien **[otsikot.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Koska Microsoft haluaa pitää asiakkaat turvassa [oletusarvoisesti,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)jotkin vuokraajan ohitukset eivät koske haittaohjelmia ja tietojen kalastelua. Ohitus: o Sallittujen lähettäjien luettelot tai sallitut toimialueluettelot (roskapostin estokäytännöt) o Outlook Lokero o IP Sallittujen lähettäjien luettelo (yhteyden suodatus) 
- Ainoa ohitus, joka sallii suuren luottamuksellisen tietojenkalasteluviestin ohittamisen, on Exchange (kutsutaan myös siirtosäännöksi). Jos haluat käyttää postinkulkusääntöjä suodatuksen ohittamiseen, katso roskapostin luottamusvälin **[(SCL)](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)** määrittäminen viesteissä postinkulkusääntöjen avulla.