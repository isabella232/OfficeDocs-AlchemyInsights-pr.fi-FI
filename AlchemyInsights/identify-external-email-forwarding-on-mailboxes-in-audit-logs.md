---
title: Ulkoisen sähköpostin edelleenlähetyksen tunnistaminen valvontalokeissa
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
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508949"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ulkoisen sähköpostin edelleenlähetyksen määrittäminen postilaatikoissa

Kun Microsoft 365 -käyttäjä määrittää postilaatikon ulkoisen sähköpostin edelleenlähetyksen, aktiviteettia valvotaan osana **Set-Mailbox-cmdlet-komentoa.** Voit tarkastella toimintaa valvontalokin haun avulla Suojaus- & Yhteensopivuuskeskuksessa.

1. Kirjaudu Microsoft [365 Security & Compliance Centeriin.](https://protection.office.com/)

2. Siirry **Haun**  >  **valvontalokin hakusivulle.**

3. Valitse päivämääräalue **Aloituspäivä-** ja **Päättymispäivä-kentissä.** Käyttäjänimeä ei tarvitse määrittää. Tarkista, että **Aktiviteetit-kentän** arvoksi on määritetty **Näytä kaikkien aktiviteettien tulokset**.

4. Valitse **Hae**.

Valitse tuloksista **Suodata tulokset** ja kirjoita aktiviteettisuodatinruutuun **Set-Mailbox.** Valitse seurantatietue tuloksista. Valitse **Details** Tiedot-pikaikkunassa **Lisätietoja**. Sinun on tarkasteltava kunkin valvontatietueen tietoja ja määritettävä, liittyykö aktiviteetti sähköpostin edelleenlähetykseen.

- **ObjectId**: Muokattavan postilaatikon aliasarvo.

- **Parametrit**: _ForwardingSmtpAddress_ ilmaisee kohdesähköpostiosoitteen.

- **UserId**: Käyttäjä, joka on määrittänyt sähköpostin edelleenlähetyksen **postilaatikkoon ObjectId-kentässä.**

Lisätietoja on [ohjeaiheessa Postilaatikon sähköpostin edelleenlähetyksen määrittäminen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
