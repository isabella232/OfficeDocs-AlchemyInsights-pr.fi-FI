---
title: Haluatko merkitä toimi alueen tai sähkö postin lähettäjän turvalliseksi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803242"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Haluatko merkitä toimi alueen tai sähkö postin lähettäjän turvalliseksi?

- **Turvallisten lähettäjien luetteloiden käyttöä ei suositella** , koska se avaa organisaation roska posti-, Phish-ja huijaus hyökkäyksille.
- Jos liiketoiminta vaatimus on olemassa, **suosittelemme** , että käytät siihen **[sähkö postin kulku sääntöjä](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** . Ohja uksen avulla varmistat, että lähettäjän todennus (tarkistaa, että lähettävä toimi alue ei ole väärennetty). **Huomautus**: emme suosittele väärien positiivisten viestien hallintaa turvallisten lähettäjien luetteloiden avulla, koska roska posti suodatukseen liittyvät poikkeukset voivat avata organisaatiosi tieto turva hyökkäyksille. Jos käyttäjä lähettää viestejä, jotka on merkitty virheellisesti roska postiksi tai roska postiksi, **[Ilmianna viestit ja tiedostot Microsoftille](https://protection.office.com/reportsubmission)**.
- Turvalliset lähettäjät Outlookissa, sallittujen lähettäjien luettelossa tai sallittujen toimi alueiden luettelossa roska postin vastaisessa politiikassa **tulee välttää** , koska lähettäjät ohittavat kaikki roska posti-, huijaus-ja Phish-suoja uksen ja lähettäjän todennuksen (SPF, DKIM, dMarc). Tätä menetelmää käytetään parhaiten vain väliaikaiseen testaukseen.
