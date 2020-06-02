---
title: Poista viestitapahtumat valvontalokeissa
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
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508985"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Poistettujen sähköpostiviestien lokien valvonta

Microsoft on oletusarvoisesti ottanut postilaatikoiden valvontalokin käyttöön tammikuusta 2019 alkaen. Muussa tapauksessa voit tarkastella tietyn käyttäjän poista viestitapahtumia manuaalisesti, jotta poistotoiminnot voidaan ottaa käyttöön manuaalisesti valvontaa varten. Jos postilaatikon valvontaloki on jo otettu käyttöön organisaatiossasi tai tietylle käyttäjälle, noudata seuraavia ohjeita.

1. Kirjautuminen [Microsoft 365 Security & Compliance Centeriin](https://protection.office.com/)

2. Valitse **Haku ja tutkinta** ja valitse **Valvontalokin haku**.

3. Valitse päivämääräalue **Aloituspäivä-** ja **Päättymispäivä-kentissä.** Määritä käyttäjälle käyttäjänimi, jota haluat tutkia (käyttäjä, joka on poistanut kohteet). Valitse **Aktiviteetit-kentässä** **Poistetut viestit Poistetut-kansiosta** ja **Siirretty viestit Poistetut-kansioon**.

4. Valitse **Hae**.

Valitse tuloksista valvontatietue. Valitse lisätietojen pikaikkunassa **Lisätietoja**. Lisätietoja poistetusta kohteesta (esimerkiksi aiherivi ja nimikkeen sijainti, kun se poistettiin) näkyvät **Vaikutuskohde-kentässä.** **ClientInfoString-ominaisuus** näyttää, tapahtuiko poisto Outlookissa, Outlookin verkkoversiossa (aiemmin Outlook Web App) tai missä tahansa muussa laitteessa.

Lisätietoja on [ohjeaiheessa Postilaatikon sähköpostin edelleenlähetyksen määrittäminen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Huomautus:** Poistettuja kohteita ei voi noutaa valvontalokitoiminnon avulla. Lisätietoja poistettujen viestien noutamista Outlookin verkkoversiossa on [ohjeaiheessa Poistettujen kohteiden palauttaminen Outlook Web Appissa](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
