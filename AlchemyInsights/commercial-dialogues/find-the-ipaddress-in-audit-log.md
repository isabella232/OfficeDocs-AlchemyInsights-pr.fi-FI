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
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017129"
---
# <a name="find-the-ip-address-in-audit-log"></a>IP-osoitteen etsiminen valvontalokista

1. Käyttäjän tai järjestelmänvalvojan suorittamaa toimintaa vastaava IP-osoite näkyy valvontalokeissa. Asiakkaan tiedot kirjataan myös lokiin. Voit tunnistaa IP-osoitteen näin:

1. Siirry Office 365 [tietoturva- & yhteensopivuuskeskukseen.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Valitse **Haun**  >  **[valvontalokihaku](https://go.microsoft.com/fwlink/?linkid=2103759)**.
    > [!NOTE]
    > Jos huomaat, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt. Jos tämä toiminto ei ole käytössä, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.
1. Jos olet kiinnostunut tietystä aktiviteetista, valitse se **Toiminnot-luettelosta.** Muussa tapauksessa kaikki toiminnot palautetaan oletusarvoisesti valitulle käyttäjälle. Huomaa, että tietyt toiminnot eivät ehkä ole käytettävissä **Toiminnot-valikossa;** Nämä valvontakohteet palautetaan kuitenkin, jos **Näytä kaikkien toimintojen tulokset** on valittuna (oletusasetus).
1. Määritä päivämääräalue ja valitse **Käyttäjät-kentässä** sen käyttäjän käyttäjänimi, jonka haluat tutkia.
1. Valitse **Hae**. Toiminnot näkyvät **Tulokset-kohdassa.** Näet kunkin toiminnon IP-osoitteen.
1. Voit tarkastella tietoja valitsemalla toiminnon ja valitsemalla sitten **Lisätietoja**.

Lisätietoja on ohjeaiheessa Valvontalokin [Office 365 yleisimmät skenaariot.](https://go.microsoft.com/fwlink/?linkid=2103944)