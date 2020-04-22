---
title: Postilaatikoiden ulkoisen sähköpostin edelleenlähetyksen tunnistaminen valvontalokeissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716457"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Tunnista, milloin ulkoinen sähköpostin edelleenlähetys on määritetty postilaatikoissa

Kun Microsoft 365 -käyttäjä määrittää postilaatikon ulkoisen sähköpostin edelleenlähetyksen, aktiviteettia valvotaan osana **Set-Mailbox-cmdlet-tiedostoa.** Toiminta näkyy valvontalokihaun avulla Suojaus-& yhteensopivuuskeskuksessa.

1. Kirjaudu Microsoft [365 Security & Compliance Centeriin.](https://protection.office.com/)

2. Siirry **Haun** > **valvontalokin hakusivulle.**

3. Valitse päivämääräväli **Aloituspäivä-** ja **Päättymispäivä-kentissä.** Käyttäjänimeä ei tarvitse määrittää. Tarkista, että **Aktiviteetit-kentän** arvo on **Näytä kaikkien aktiviteettien tulokset**.

4. Valitse **Hae**.

Valitse tuloksista **Suodata tulokset** ja kirjoita aktiviteettisuodatinruutuun **Set-Mailbox.** Valitse tuloksista valvontatietue. Valitse **Tiedot-pikaikkunassa** **Lisätietoja**. Sinun on tarkasteltava kunkin valvontatietueen tietoja selvittääksesi, liittyykö aktiviteetti sähköpostin edelleenlähettämiseen.

- **ObjectId**: Muokatun postilaatikon aliasarvo.

- **Parametrit**: _ForwardingSmtpAddress_ ilmaisee kohdesähköpostiosoitteen.

- **UserId**: Käyttäjä, joka on määrittänyt sähköpostin edelleenlähetyksen postilaatikkoon **ObjectId-kentässä.**

Lisätietoja on ohjeaiheessa [Postilaatikon sähköpostin edelleenlähetyksen määrittäminen](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
