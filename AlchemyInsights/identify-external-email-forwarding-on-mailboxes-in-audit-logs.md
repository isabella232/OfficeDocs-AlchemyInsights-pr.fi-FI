---
title: Valvonta lokien posti laatikoiden ulkoinen sähkö postin lähettäminen edelleen
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696294"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Määritä, milloin ulkoinen sähkö postin välitys on määritetty posti laatikoihin

Kun Microsoft 365-käyttäjä määrittää posti laatikon ulkoiseen sähkö postin lähettämiseen, toiminta tarkastetaan osana **joukko posti laatikon cmdlet-** komentosovelmaa. Voit tarkastella aktiviteettia valvonta loki haun avulla tieto turva-& yhteensopivuus keskuksessa.

1. Kirjaudu sisään [Microsoft 365-tieto turva & Compliance Centeriin](https://protection.office.com/).

2. Siirry **haun**  >  **valvonta lokien haku** sivulle.

3. Valitse päivämäärä väli **alkamis päivä** -ja **päättymis päivä** -kenttiin. Sinun ei tarvitse määrittää käyttäjä nimeä. Varmista, että **aktiviteetit** -kenttä on valittu **näyttämään kaikkien toimintojen tulokset**.

4. Valitse **Hae**.

Valitse tulokset-kohdassa **Suodata tulokset** ja kirjoita **Määritä-posti laatikko** aktiviteetin suodatus-ruutuun. Valitse seuranta tietue tuloksista. Valitse **tiedot** -valikosta **lisä tietoja**. Sinun on tarkasteltava kunkin valvonta tietueen tietoja määrittääksesi, onko toiminto yhteydessä sähkö postin lähettämiseen.

- **ObjectID**: muutetun posti laatikon alias-arvo.

- **Parametrit**: _fordingingsmtpaddress_ osoittaa kohde Sähkö posti osoitteen.

- **UserID**: käyttäjä, joka määritti sähkö postin lähettämisen **objectID** -kentässä olevalle posti laatikolle.

Lisä tietoja [on kohdassa sähkö postin lähettämisen määrittäminen Posti laatikolle](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
