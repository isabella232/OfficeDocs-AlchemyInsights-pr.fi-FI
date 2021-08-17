---
title: Poistettujen tapahtumien valvontalokien lukeminen
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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896012"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Poistettujen tapahtumien valvontalokien lukeminen

Voit tehdä tämän näin:

1. Tee jokin seuraavista:
   - Valitse Microsoft 365 -yhteensopivuuskeskus <https://compliance.microsoft.com> :ssä Ratkaisujen  \> **valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://compliance.microsoft.com/auditlogsearch> -
   - Valitse Microsoft 365 Defender -portaalissa <https://security.microsoft.com> **Valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://security.microsoft.com/auditlogsearch> -

    > [!NOTE]
    > Jos huomaat, että sinun on ottaa ominaisuus käyttöön, ota se käyttöön nyt. Jos ominaisuus ei ole käytössä, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.

2. Määritä **Valvonta-sivun** **Haku-välilehdessä** seuraavat asetukset:
   - **Päivämäärä- ja aikaalue:** Valitse päivämäärä-/aika-alue Aloitus- ja **Lopetus-ruuduista.** 
   - **Toiminnot:** **Exchange postilaatikon toiminnot** ja valitse sitten seuraavat arvot:
     - **Poistetut-kansiosta poistetut viestit**
     - **Viestit siirretty Poistetut-kansioon**

       Kun olet valmis, pienennä Toiminnot-ruutu napsauttamalla ruudun **ulkopuolella.**

   - **Käyttäjät:** Voit palauttaa kaikkien käyttäjien tulokset hyväksymällä tyhjän oletusarvon tai kirjoittamalla yhden tai useamman käyttäjän.

3. Kun olet valmis, valitse **Hae**. Toiminnot näkyvät uudella **Valvontahaku-sivulla.**

4. Avaa tietojen pikaikkuna valitsemalla toiminto tuloksista. Poistettua kohdetta koskevat lisätiedot, kuten aiherivi ja kohteen sijainti, kun kohde poistettiin, näkyvät **AffectedItems-kentässä.**

   > [!NOTE]
   > Poistettuja kohteita ei voi palauttaa valvontalokitoiminnolla. Lisätietoja poistettujen kohteiden palauttamisesta [on kohdassa Poistettujen sähköpostiviestien palauttaminen Outlookin verkkoversio.](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)

Lisätietoja on kohdassa [Valvontalokista etsiminen yleisimpiä tukiongelmia tutkimista varten.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
