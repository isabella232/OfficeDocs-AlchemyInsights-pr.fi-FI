---
title: IP-osoitteen ja asiakkaan tunnistaminen valvontalokeissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716385"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-osoitteen ja asiakkaan tunnistaminen valvontalokeissa

Valvontalokeissa näkyy IP-osoite, joka vastaa Microsoft 365 -käyttäjän tai -järjestelmänvalvojan toimintaa. Myös asiakastiedot kirjataan lokiin. Seuraavassa on ohjeet tällaisten tietojen tunnistamiseen

1. Kirjaudu Microsoft [365 Security & Compliance Centeriin.](https://protection.office.com/)

2. Siirry **Haun** > **valvontalokin hakusivulle.**

   Jos olet kiinnostunut tietystä aktiviteetista, valitse se **Aktiviteetit-luettelosta.** Jos näin ei ole, kaikki toiminnot palautetaan valitulle käyttäjälle (oletusasetus).

   **Huomautus**: Tietyt toiminnot eivät ehkä ole käytettävissä **Aktiviteetit-valikossa.** Nämä valvontakohteet palautetaan kuitenkin, jos **Näytä kaikkien aktiviteettien tulokset** on valittuna (oletusasetus).

3. Määritä käyttäjänimi Käyttäjät-kentässä, valitse aktiviteetille sopiva päivämääräalue ja valitse sitten **Etsi**. **Users**

Tuloksissa kyseisen aktiviteetin IP-osoite näkyy tulosruudussa. Valitse valvontatietue, jos haluat nähdä **yksityiskohtaiset** tiedot Tiedot-pikaikkunassa (esimerkiksi Asiakas, Toiminnon suorittanut käyttäjä jne.).

Lisätietoja on [ohjeaiheessa Vaarantuneen tilin käyttämiseen käytettävän tietokoneen IP-osoitteen etsiminen](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
