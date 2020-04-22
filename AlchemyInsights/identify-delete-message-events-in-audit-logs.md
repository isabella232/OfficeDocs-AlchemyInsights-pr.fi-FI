---
title: Valvontalokien sanomatapahtumien poistaminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716493"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Valvo poistettujen sähköpostiviestien lokit

Tammikuusta 2019 alkaen Microsoft ottaa postilaatikon valvontalokin käyttöön oletusarvoisesti. Jos haluat tarkastella tietyn käyttäjän poistoviestitapahtumia, sinun on otettava poistotoiminnot valvonnan yhteydessä manuaalisesti käyttöön. Jos postilaatikon valvontaloki on jo otettu käyttöön organisaatiossa tai tietylle käyttäjälle, noudata seuraavia ohjeita.

1. Kirjaudu Microsoft [365 Security & Compliance Centeriin](https://protection.office.com/)

2. Valitse **Etsi ja tutki** ja valitse **Valvontalokin haku**.

3. Valitse päivämääräväli **Aloituspäivä-** ja **Päättymispäivä-kentissä.** Määritä tutkittavan käyttäjän käyttäjänimi (käyttäjä, joka poisti kohteet). Valitse **Aktiviteetit-kentässä** **Poistetut viestit Poistetut-kansiosta** ja **Siirretyt viestit Poistetut-kansioon**.

4. Valitse **Hae**.

Valitse tuloksista valvontatietue. Valitse tiedot-pikaikkunassa **Lisätietoja**. Lisätietoja poistetusta kohteesta (esimerkiksi aiherivi ja nimikkeen sijainti, kun se poistettiin) näkyy **Haavoittuvuuden kohteet** -kentässä. **ClientInfoString-ominaisuus** näyttää, tapahtuiko poisto Outlookissa, Outlookin verkkoversiossa (aiemmin Outlook Web App) tai missä tahansa muussa laitteessa.

Lisätietoja on ohjeaiheessa [Postilaatikon sähköpostin edelleenlähetyksen määrittäminen](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Huomautus**: Et voi hakea poistettuja kohteita valvontalokiominaisuuden avulla. Lisätietoja poistettujen viestien noutamiseen Outlookin verkkoversiossa on [ohjeaiheessa Poistettujen kohteiden palauttaminen Outlook Web Appissa](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
