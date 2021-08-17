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
ms.openlocfilehash: 080b3df3934781ebf0d0cd5243787bf6975fc5f123b5b1593c0b6d9ada4eae5d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887497"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-osoitteen ja asiakkaan tunnistaminen valvontalokeja varten

Käyttäjän tai järjestelmänvalvojan toimintaa vastaava IP-osoite Microsoft 365 valvontalokeissa. Asiakkaan tiedot kirjataan myös lokiin. Näiden tietojen tunnistusvaiheet

1. Kirjaudu Microsoft 365 [yhteensopivuuskeskukseen.](https://protection.office.com/)

2. Siirry haun   >  **valvontalokihakusivulle.**

   Jos olet kiinnostunut tietystä aktiviteetista, valitse se **Toiminnot-luettelosta.** Jos ei, kaikki toiminnot palautetaan valitulle käyttäjälle (oletusasetus).

   **Huomautus:** Tietyt toiminnot eivät ehkä ole käytettävissä **Toiminnot-valikossa;** Nämä valvontakohteet palautetaan kuitenkin, jos **Näytä kaikkien toimintojen tulokset** on valittuna (oletusasetus).

3. Määritä käyttäjänimi **Käyttäjät-kentässä,** valitse sopiva päivämääräalue aktiviteetille ja valitse sitten **Hae**.

Tuloksissa näet toiminnon IP-osoitteen tulosruudussa. Valitsemalla valvontatietueen näet yksityiskohtaiset  tiedot Tiedot-pikaikkunassa (esimerkiksi Asiakas, käyttäjä, joka suoritti toiminnon jne.).

Lisätietoja on kohdassa [Sen tietokoneen IP-osoitteen selvittäminen, jota käytetään vaarantunutta tiliä varten.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
