---
title: IP-osoitteen ja asiakas ohjelman tunnistaminen valvonta lokeissa
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
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668307"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-osoitteen ja asiakas ohjelman tunnistaminen valvonta lokeissa

Microsoft 365-käyttäjän tai-järjestelmänvalvojan toimintaa vastaava IP-osoite näkyy valvonta lokeissa. Myös asiakas tiedot kirjataan lokiin. Näiden tietojen tunnistamisen vaiheet

1. Kirjaudu sisään [Microsoft 365-tieto turva & Compliance Centeriin](https://protection.office.com/).

2. Siirry **haun**  >  **valvonta lokien haku** sivulle.

   Jos olet kiinnostunut tietystä aktiviteetista, valitse se **aktiviteetit** -luettelosta. Jos näin ei ole, valitun käyttäjän kaikki toiminnot palautetaan (oletus asetus).

   **Huomautus**: tietyt toiminnot eivät ehkä ole käytettävissä **aktiviteetit** -valikossa. Nämä valvonta kohteet palautetaan, jos **kaikkien aktiviteettien Näytä tulokset** -vaihto ehto on valittuna (oletus asetus).

3. Määritä käyttäjä nimi **käyttäjät** -kentässä, valitse aktiviteetille sopiva päivämäärä alue ja valitse sitten **Hae**.

Tuloksissa näkyy kyseisen toiminnon IP-osoite tulokset-ruudussa. Valitse valvonta tietue, jos haluat nähdä yksityiskohtaisia tietoja tietojen pikavalikosta (esimerkiksi asiakas, käyttäjä, **joka on suorittanut** toiminnon jne.).

Lisä tietoja on kohdassa [sen tieto koneen IP-osoitteen etsiminen, jota käytetään vaarantuneen tilin käyttämiseen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
