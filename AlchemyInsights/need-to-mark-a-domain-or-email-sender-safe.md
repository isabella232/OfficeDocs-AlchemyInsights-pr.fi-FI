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
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286677"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Tarvitseeko sinun merkitä toimialue tai sähköpostin lähettäjä turvalliseksi?

- Turvallisten **lähettäjien luetteloiden käyttöä** ei suositella, koska se avaa organisaatiosi roskaposti-, osoite- ja osoitetushyökkäyksille.
- Jos kyse on liiketoiminnan vaatimuksesta, **suosittelemme** kuitenkin käyttämään **[tähän Flow sähköpostisääntöjä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Ohjeemme varmistavat lähettäjän todennuksen (varmistaa, että toimialueen lähetystä ei osoiteta). **Huomautus:** Emme suosittele virheellisten positiivisten tietojen hallintaa turvallisten lähettäjien luetteloiden avulla, koska roskapostisuodatuksen poikkeukset voivat avata organisaatiosi suojaushyökkäyksiin. Jos käyttäjäsi saavat virheellisesti roskapostiksi merkittyjä viestejä, ilmoita viesteistä ja tiedostoista **[Microsoftille.](https://protection.office.com/reportsubmission)**
- Roskapostin estokäytäntöjen Outlook turvallisten lähettäjien, sallittujen lähettäjien, sallittujen lähettäjien tai sallittujen toimialueiden luetteloiden käyttöä on vältettävä, koska lähettäjät ohittavat kaikki roskapostit, osoitekaapin ja tietojen estosuojauksen sekä lähettäjän todennuksen (SPF, DKIM, DMARC).  Tätä menetelmää käytetään parhaiten vain tilapäistesteissä.
- Vahvistus, jonka mukaan tietty sähköposti ohitettu Roskapostin arviointi voidaan tehdä tarkistamalla viestin otsikko "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), katso roskapostiviestien **[otsikot.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Koska Microsoft haluaa pitää asiakkaat turvassa [oletusarvoisesti,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)jotkin vuokraajan ohitukset eivät koske haittaohjelmia ja tietojen kalastelua. Näitä ohituskäytäntöjä ovat seuraavat: o Sallittujen lähettäjien luettelot tai sallitut toimialueluettelot (roskapostin estokäytännöt) o Outlook turvalliset lähettäjät o IP:n sallittujen lähettäjien luettelo (yhteyden suodatus) 
- Ainoa ohitus, joka sallii suuren luottamusta kalasteluviestin ohittamisen, on Exchange (kutsutaan myös siirtosäännöksi). Jos haluat käyttää postinkulkusääntöjä suodatuksen ohittamiseen, tutustu kohtaan SCL (spam confidence level) -roskapostitason **[määrittäminen viesteissä postinkulkusääntöjen avulla.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**