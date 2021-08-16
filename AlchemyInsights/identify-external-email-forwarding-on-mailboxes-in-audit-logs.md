---
title: Ulkoisen sähköpostin edelleenlähetysten tunnistaminen postilaatikoissa valvontalokeihin
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028731"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ulkoisen sähköpostin edelleenlähetysmäärityksen tunnistaminen postilaatikoissa

Kun Microsoft 365 määrittää postilaatikon ulkoisen sähköpostin edelleenlähetystä, toiminta valvotaan osana **Set-Mailbox-cmdlet-komentoa.** Näet toiminnon valvontalokihaun avulla tietoturva- & yhteensopivuuskeskuksessa.

1. Kirjaudu Microsoft 365 [yhteensopivuuskeskukseen.](https://protection.office.com/)

2. Siirry haun   >  **valvontalokihakusivulle.**

3. Valitse päivämääräalue Alkamispäivä- ja **Päättymispäivä-kentistä.**  Käyttäjänimeä ei tarvitse määrittää. Tarkista, **että Toiminnot-kentän** **arvoksi on määritetty Näytä kaikkien toimintojen tulokset**.

4. Valitse **Hae**.

Valitse tuloksissa **Suodata tulokset** ja kirjoita **Toimintasuodatin-ruutuun Set-Mailbox.** Valitse valvontatietue tuloksista. Valitse **Tiedot-pikaikkunassa** **Lisätietoja**. Sinun on tarkastettava kunkin valvontatietueen tiedot sen määrittämiseksi, liittyykö toiminto sähköpostin edelleenlähetystän.

- **ObjectId:** Muokatun postilaatikon aliasarvo.

- **Parametrit:** _ForwardingSmtpAddress osoittaa_ kohdesähköpostiosoitteen.

- **UserId:** Käyttäjä, joka määritti sähköpostin edelleenlähetystä postilaatikossa **ObjectId-kentässä.**

Lisätietoja on kohdassa [Postilaatikon sähköpostin edelleenlähetysten määritysten selvittäminen.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
