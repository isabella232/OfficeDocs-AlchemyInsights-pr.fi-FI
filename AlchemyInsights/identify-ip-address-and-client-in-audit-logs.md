---
title: IP-osoitteen ja asiakkaan tunnistaminen valvontalokeja varten
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: fcad71bcc5ea6036bc8fa25a9be38caabc4d0889ee01ea86e23065333d5fce0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014897"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-osoitteen ja asiakkaan tunnistaminen valvontalokeja varten

Ip-osoite, joka vastaa käyttäjän Microsoft 365 tai järjestelmänvalvojan toimintaa, näkyy Valvontalokit-issa. Asiakkaan tiedot kirjataan myös lokiin. Näiden tietojen tunnistusvaiheet

1. Kirjaudu Microsoft 365 [yhteensopivuuskeskukseen.](https://protection.office.com/)

2. Siirry haun   >  **valvontalokihakusivulle.**

   Jos olet kiinnostunut tietystä aktiviteetista, valitse se **Toiminnot-luettelosta.** Jos ei, kaikki toiminnot palautetaan valitulle käyttäjälle (oletusasetus).

   **Huomautus:** Tietyt toiminnot eivät ehkä ole käytettävissä **Toiminnot-valikossa;** Nämä valvontakohteet palautetaan kuitenkin, jos **Näytä kaikkien toimintojen tulokset** on valittuna (oletusasetus).

3. Määritä käyttäjänimi **Käyttäjät-kentässä,** valitse sopiva päivämääräalue aktiviteetille ja valitse sitten **Hae**.

Tuloksissa näet toiminnon IP-osoitteen tulosruudussa. Valitsemalla valvontatietueen näet yksityiskohtaiset  tiedot Tiedot-pikaikkunassa (esimerkiksi Asiakas, käyttäjä, joka suoritti toiminnon jne.).

Lisätietoja on kohdassa [Sen tietokoneen IP-osoitteen selvittäminen, jota käytetään vaarantunutta tiliä varten.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
