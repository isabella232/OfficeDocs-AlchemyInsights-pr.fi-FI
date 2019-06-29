---
title: Määritä ulkoisen sähköpostin välityksen seurantalokeja postilaatikoita
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383094"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Tunnistaa, kun postilaatikoita ulkoisen sähköpostin edelleenlähetys on määritetty

Kun käyttäjä määrittää postilaatikkoon ulkoisen sähköpostin edelleenlähetys, toimintaa tarkistetaan osana **Set-Mailbox** -cmdlet-komennolla. Voit tarkastella tehtävän tarkastuksen lokista etsintää käyttämällä suojauksen & Compliance Centeriin.

1. Kirjautua [Office 365-suojauksen & Compliance Centeriin](https://protection.office.com/)

2. **Etsi ja tutkimus** ja valitse **Valvo lokista etsintää**.

3. Valitse **aloituspäivä** - ja **päättymispäivä** -kenttiin päivämääräalue. Sinun ei tarvitse määrittää käyttäjänimi. Tarkista tulokset **kaikista** **aktiviteetit** -kentässä on määritetty.

4. Valitse **Etsi**.

**Suodatuksen tulokset** valitsemalla tulokset ja kirjoita Suodata-ruutuun aktiviteetin **Set-Mailbox** . Valitse tuloksia koskeva seurantatietue. Valitse **tiedot** -valikon avauspainike **Lisätietoja**. On tarkasteltavan määrittääkseen, jos tehtävä liittyy sähköpostin edelleenlähetys kunkin valvontatietueen tietojen.

- **ObjectId**: tunnuksen arvo postilaatikko, johon tehtiin muutoksia.

- **Parametrit**: _ForwardingSmtpAddress_ ilmaisee kohteen sähköpostiosoite.

- **Käyttäjätunnus**: käyttäjä, joka on määritetty sähköpostin edelleenlähetys postilaatikon **ObjectId** -kentässä.

Lisätietoja [määrittäminen, joka määrittää sähköpostiviestin välittäminen postilaatikkoon](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
