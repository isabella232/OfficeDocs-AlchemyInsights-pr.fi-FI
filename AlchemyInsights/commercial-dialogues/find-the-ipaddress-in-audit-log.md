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
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303574"
---
# <a name="find-the-ip-address-in-audit-log"></a>IP-osoitteen etsiminen valvontalokista

Käyttäjän tai järjestelmänvalvojan suorittamaa toimintaa vastaava IP-osoite näkyy valvontalokeissa. Asiakkaan tiedot kirjataan myös lokiin. Voit tunnistaa IP-osoitteen näin:

1. Tee jokin seuraavista:
   - Valitse Microsoft 365 -yhteensopivuuskeskus <https://compliance.microsoft.com> -palvelussa **Ratkaisujen** \> **valvonta.** Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://compliance.microsoft.com/auditlogsearch> -
   - Valitse Microsoft 365 Defender <https://security.microsoft.com> -portaalissa **Valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://security.microsoft.com/auditlogsearch> -

    **Huomautus:** Jos näet ilmoituksen, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt. Jos tämä toiminto ei ole käytössä, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.

2. Varmista **Valvonta-sivulla,** että **Haku-välilehti** on valittuna, ja määritä sitten seuraavat asetukset:
   - **Päivämäärä- ja aikaalue:** Valitse päivämäärä-/aika-alue Aloitus- ja **Lopetus-ruuduista.** 
   - **Toiminnot:** Jos olet kiinnostunut tietystä aktiviteetista, valitse se luettelosta; Muussa tapauksessa oletusarvo Näytä **kaikkien toimintojen tulokset** palauttaa kaikki toiminnot. Huomaa, että tietyt toiminnot eivät ehkä ole käytettävissä valittavissa; Nämä valvontakohteet palautetaan kuitenkin, jos **Näytä kaikkien toimintojen** tulokset on valittuna.
   - **Käyttäjät:** Voit palauttaa kaikkien käyttäjien tulokset hyväksymällä tyhjän oletusarvon tai kirjoittamalla yhden tai useamman käyttäjän.

3. Kun olet valmis, valitse **Hae**. Toiminnot näkyvät uudella **Valvontahaku-sivulla.**

4. Valitse tuloksissa **Suodata tulokset** ja kirjoita **Toimintasuodatin-ruutuun Set-Mailbox.**

5. Avaa Tiedot-pikaikkuna valitsemalla valvontatietue tuloksista. 

Lisätietoja on kohdassa [Valvontalokista etsiminen yleisimpiä tukiongelmia tutkimista varten.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
