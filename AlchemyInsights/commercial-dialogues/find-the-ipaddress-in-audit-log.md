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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902257"
---
# <a name="find-the-ip-address-in-audit-log"></a>IP-osoitteen etsiminen valvontalokista

Käyttäjän tai järjestelmänvalvojan suorittamaa toimintaa vastaava IP-osoite näkyy valvontalokeissa. Asiakkaan tiedot kirjataan myös lokiin. Voit tunnistaa IP-osoitteen näin:

1. Tee jokin seuraavista:
   - Valitse Microsoft 365 -yhteensopivuuskeskus <https://compliance.microsoft.com> :ssä Ratkaisujen  \> **valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://compliance.microsoft.com/auditlogsearch> -
   - Valitse Microsoft 365 Defender -portaalissa <https://security.microsoft.com> **Valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://security.microsoft.com/auditlogsearch> -

    > [!NOTE]
    > Jos huomaat, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt. Jos tämä toiminto ei ole käytössä, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.

2. Varmista **Valvonta-sivulla,** että **Haku-välilehti** on valittuna, ja määritä sitten seuraavat asetukset:
   - **Päivämäärä- ja aikaalue:** Valitse päivämäärä-/aika-alue Aloitus- ja **Lopetus-ruuduista.** 
   - **Toiminnot:** Jos olet kiinnostunut tietystä aktiviteetista, valitse se luettelosta; Muussa tapauksessa oletusarvo Näytä **kaikkien toimintojen tulokset** palauttaa kaikki toiminnot. Huomaa, että tietyt toiminnot eivät ehkä ole käytettävissä valittavissa; Nämä valvontakohteet palautetaan kuitenkin, jos **Näytä kaikkien toimintojen** tulokset on valittuna.
   - **Käyttäjät:** Voit palauttaa kaikkien käyttäjien tulokset hyväksymällä tyhjän oletusarvon tai kirjoittamalla yhden tai useamman käyttäjän.

3. Kun olet valmis, valitse **Hae**. Toiminnot näkyvät uudella **Valvontahaku-sivulla.**

4. Valitse tuloksissa **Suodata tulokset** ja kirjoita **Toimintasuodatin-ruutuun Set-Mailbox.**

5. Avaa Tiedot-pikaikkuna valitsemalla valvontatietue tuloksista. 

Lisätietoja on kohdassa [Valvontalokista etsiminen yleisimpiä tukiongelmia tutkimista varten.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
