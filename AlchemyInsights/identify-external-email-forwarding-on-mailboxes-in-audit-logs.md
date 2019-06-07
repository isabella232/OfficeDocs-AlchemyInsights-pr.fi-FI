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
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34751997"
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
