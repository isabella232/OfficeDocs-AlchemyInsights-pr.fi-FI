---
title: Valvonta lokien Poista viesti tapahtumat-kohdan määrittäminen
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696510"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Poistettujen Sähkö posti viestien valvonta lokit

Tammi kuusta 2019 lähtien Microsoft on siirtymässä posti laatikon valvonta lokiin oletusarvoisesti. Jos haluat tarkastella tietyn käyttäjän Poista viesti tapahtumia, sinun on otettava manuaalisesti käyttöön valvonnan poistamis toiminnot. Jos posti laatikon valvonta loki on jo otettu käyttöön organisaatiossa tai tietyssä käyttäjälle, noudata seuraavia ohjeita.

1. Kirjaudu sisään [Microsoft 365-tieto turva & Compliance Centeriin](https://protection.office.com/)

2. Valitse **haku ja tutkinta** ja valitse **valvonta lokien haku**.

3. Valitse päivämäärä väli **alkamis päivä** -ja **päättymis päivä** -kenttiin. Määritä sen käyttäjän käyttäjä nimi, jonka haluat tutkia (kohteet poistaneen käyttäjän). Valitse **aktiviteetit** -kentässä poistetut **viestit Poistetut-kansiosta** ja **siirretyt viestit Poistetut-kansioon**.

4. Valitse **Hae**.

Valitse tulokset-kohdassa valvonta tietue. Valitse tiedot-valikosta **lisä tietoja**. Lisä tietoja poistetusta kohteesta (esimerkiksi aihe-rivi ja kohteen sijainti, kun kohde on poistettu) näkyy **Affetecitems** -kentässä. **Clialinfostring** -ominaisuus näkyy, jos poisto on tapahtunut Outlookissa, Outlookin verkko versiossa (aiemmin Outlook Web App) tai missä tahansa muussa laitteessa.

Lisä tietoja [on kohdassa sähkö postin lähettämisen määrittäminen Posti laatikolle](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Huomautus**: poistettuja kohteita ei voi noutaa valvonta loki-toiminnon avulla. Lisä tietoja poistettujen viestien hakemisesta Outlookin verkko versiossa on Ohje aiheessa [poistettujen kohteiden palauttaminen Outlook Web Appissa](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
