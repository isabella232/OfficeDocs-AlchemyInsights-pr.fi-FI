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
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792129"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Tarvitseeko sinun merkitä toimialue tai sähköpostin lähettäjä turvalliseksi?

- Turvallisten **lähettäjien luetteloiden käyttöä** ei suositella, koska se avaa organisaatiosi roskaposti-, osoite- ja osoitetushyökkäyksille.
- Jos liiketoimintaa kuitenkin vaaditaan, suosittelemme käyttämään **tähän** **[postinkulkusääntöjä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Ohjeemme varmistavat lähettäjän todennuksen (varmistaa, että toimialueen lähetystä ei osoiteta). **Huomautus:** Emme suosittele virheellisten positiivisten tietojen hallintaa turvallisten lähettäjien luetteloiden avulla, koska roskapostisuodatuksen poikkeukset voivat avata organisaatiosi suojaushyökkäyksiin. Jos käyttäjäsi saavat virheellisesti roskapostiksi merkittyjä viestejä, ilmoita viesteistä ja tiedostoista **[Microsoftille.](https://protection.office.com/reportsubmission)**
- Turvallisten lähettäjien käyttöä Outlookissa, Sallittujen lähettäjien  luetteloa tai sallittujen toimialueiden luetteloa roskapostin estokäytäntöjen avulla on vältettävä, koska lähettäjät ohittavat kaiken roskapostin, tekeutumisen ja tietojen lähettäjän suojauksen sekä lähettäjän todennuksen (SPF, DKIM, DMARC). Tätä menetelmää käytetään parhaiten vain tilapäistesteissä.
