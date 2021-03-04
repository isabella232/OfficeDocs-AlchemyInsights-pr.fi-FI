---
title: IP-osoitteen etsiminen valvontalokista
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429504"
---
# <a name="find-the-ip-address-in-audit-log"></a>IP-osoitteen etsiminen valvontalokista

1. Käyttäjän tai järjestelmänvalvojan suorittamaa toimintaa vastaava IP-osoite näkyy valvontalokeissa. Asiakkaan tiedot kirjataan myös lokiin. Voit tunnistaa IP-osoitteen näin:

1. Siirry [Office 365:n tietoturva- & yhteensopivuuskeskukseen.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Valitse **Haun**  >  **[valvontalokihaku.](https://go.microsoft.com/fwlink/?linkid=2103759)**
    > [!NOTE]
    > Jos näet ilmoituksen, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt. Jos tätä ominaisuutta ei ole otettu käyttöön, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.
1. Jos olet kiinnostunut tietystä aktiviteetista, valitse se **Toiminnot-luettelosta.** Muussa tapauksessa kaikki toiminnot palautetaan oletusarvoisesti valitulle käyttäjälle. Huomaa, että tietyt toiminnot eivät ehkä ole käytettävissä **Toiminnot-valikossa;** Nämä valvontakohteet palautetaan kuitenkin, jos **Näytä kaikkien toimintojen** tulokset on valittuna (oletusasetus).
1. Määritä päivämääräalue ja valitse **Käyttäjät-kentässä** sen käyttäjän käyttäjänimi, jonka haluat tutkia.
1. Valitse **Hae.** Toiminnot näkyvät **Tulokset-kohdassa.** Näet kunkin toiminnon IP-osoitteen.
1. Voit tarkastella tietoja valitsemalla aktiviteetin ja valitsemalla **sitten Lisätietoja.**

Lisätietoja on ohjeaiheessa Office [365:n valvontalokista etsiminen yleisimpiä skenaarioita varten.](https://go.microsoft.com/fwlink/?linkid=2103944)