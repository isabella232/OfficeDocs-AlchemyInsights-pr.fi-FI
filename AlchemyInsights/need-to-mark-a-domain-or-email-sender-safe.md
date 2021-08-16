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
ms.openlocfilehash: 7058b6419e52fce94f3359d0bd8e1d67c5aa5ef6743abf4ed39f45bad49e1d07
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025607"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Tarvitseeko sinun merkitä toimialue tai sähköpostin lähettäjä turvalliseksi?

- Turvallisten **lähettäjien luetteloiden käyttöä** ei suositella, koska se avaa organisaatiosi roskaposti-, osoite- ja osoitetushyökkäyksille.
- Jos kyse on liiketoiminnan vaatimuksesta, **suosittelemme** kuitenkin käyttämään **[tähän Flow sähköpostisääntöjä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Ohjeemme varmistavat lähettäjän todennuksen (varmistaa, että toimialueen lähetystä ei osoiteta). **Huomautus:** Emme suosittele virheellisten positiivisten tietojen hallintaa turvallisten lähettäjien luetteloiden avulla, koska roskapostisuodatuksen poikkeukset voivat avata organisaatiosi suojaushyökkäyksiin. Jos käyttäjäsi saavat virheellisesti roskapostiksi merkittyjä viestejä, ilmoita viesteistä ja tiedostoista **[Microsoftille.](https://protection.office.com/reportsubmission)**
- Lokero Roskapostin estokäytäntöjen Outlook, Sallittujen lähettäjien luettelo  tai sallittujen toimialueiden luettelo on syytä välttää, koska lähettäjät ohittavat kaiken roskapostin, osoitevirheiden ja tietojen estosuojauksen sekä lähettäjän todennuksen (SPF, DKIM, DMARC). Tätä menetelmää käytetään parhaiten vain tilapäistesteissä.
- Vahvistus, jonka mukaan tietty sähköposti ohitettu Roskapostin arviointi voidaan tehdä tarkistamalla viestin otsikko "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), katso roskapostiviestien **[otsikot.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Koska Microsoft haluaa pitää asiakkaat turvassa [oletusarvoisesti,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)jotkin vuokraajan ohitukset eivät koske haittaohjelmia ja tietojen kalastelua. Ohitus: o Sallittujen lähettäjien luettelot tai sallitut toimialueluettelot (roskapostin estokäytännöt) o Outlook Lokero o IP Sallittujen lähettäjien luettelo (yhteyden suodatus) 
- Ainoa ohitus, joka sallii suuren luottamusta kalasteluviestin ohittamisen, on Exchange (kutsutaan myös siirtosäännöksi). Jos haluat käyttää postinkulkusääntöjä suodatuksen ohittamiseen, tutustu kohtaan SCL (spam confidence level) -roskapostitason **[määrittäminen viesteissä postinkulkusääntöjen avulla.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**