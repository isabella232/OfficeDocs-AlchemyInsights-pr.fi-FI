---
title: Haluatko merkitä verkkotunnuksen tai sähköpostin lähettäjän turvallisesti?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281145"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Haluatko merkitä verkkotunnuksen tai sähköpostin lähettäjän turvallisesti?

- **Turvallisten lähettäjien luetteloiden** käyttöä ei suositella, koska se avaa organisaatiosi roskapostille, phishille ja väärentämishyökkäyksille.
- Jos liiketoimintavaatimus kuitenkin on olemassa, **suosittelemme, että** käytät tähän Mail **[Flow -sääntöjä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Ohjeemme varmistaa lähettäjän todennuksen (tarkistaa, että toimialueen lähettämistä ei vallu). **Huomautus:** Emme suosittele väärien positiivisten tarkistusten hallintaa turvallisten lähettäjien luetteloiden avulla, koska roskapostin suodattamiseen tehdyt poikkeukset voivat avata organisaatiosi suojaushyökkäyksille. Jos käyttäjäsi saavat roskapostiksi tai roskapostiksi virheellisesti merkittyjä viestejä, **[ilmoita viesteistä ja tiedostoista Microsoftille.](https://protection.office.com/reportsubmission)**
- Turvalliset lähettäjät Outlookissa, Sallittu lähettäjäluettelo tai sallittu toimialueluettelo roskapostin vastaisissa käytännöissä **tulisi välttää,** koska lähettäjät ohittavat kaiken roskapostin, väärentämisen ja phish-suojauksen sekä lähettäjän todennuksen (SPF, DKIM, DMARC). Tätä menetelmää käytetään parhaiten vain tilapäisissä testeissä.
