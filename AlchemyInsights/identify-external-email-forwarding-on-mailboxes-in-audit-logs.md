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
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539098"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Tunnistaa, kun postilaatikoita ulkoisen sähköpostin edelleenlähetys on määritetty

Kun Office 365-käyttäjä määrittää postilaatikkoon ulkoisen sähköpostin edelleenlähetys, toimintaa tarkistetaan osana **Set-Mailbox** -cmdlet-komennolla. Voit tarkastella tehtävän tarkastuksen lokista etsintää käyttämällä suojauksen & Compliance Centeriin.

1. Kirjautua sisään [Office 365 & noudattamista Tietoturvakeskus](https://protection.office.com/).

2. Siirry **Etsinnän** > **Audit log** etsintäsivun.

3. Valitse **aloituspäivä** - ja **päättymispäivä** -kenttiin päivämääräalue. Sinun ei tarvitse määrittää käyttäjänimi. Tarkista tulokset **kaikista** **aktiviteetit** -kentässä on määritetty.

4. Valitse **Etsi**.

**Suodatuksen tulokset** valitsemalla tulokset ja kirjoita Suodata-ruutuun aktiviteetin **Set-Mailbox** . Valitse tuloksia koskeva seurantatietue. Valitse **tiedot** -valikon avauspainike **Lisätietoja**. On tarkasteltavan määrittääkseen, jos tehtävä liittyy sähköpostin edelleenlähetys kunkin valvontatietueen tietojen.

- **ObjectId**: tunnuksen arvo postilaatikko, johon tehtiin muutoksia.

- **Parametrit**: _ForwardingSmtpAddress_ ilmaisee kohteen sähköpostiosoite.

- **Käyttäjätunnus**: käyttäjä, joka on määritetty sähköpostin edelleenlähetys postilaatikon **ObjectId** -kentässä.

Lisätietoja [määrittäminen, joka määrittää sähköpostiviestin välittäminen postilaatikkoon](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
