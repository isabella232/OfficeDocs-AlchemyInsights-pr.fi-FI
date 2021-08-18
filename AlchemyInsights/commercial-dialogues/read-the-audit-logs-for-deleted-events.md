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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324730"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Poistettujen tapahtumien valvontalokien lukeminen

Voit tehdä tämän näin:

1. Tee jokin seuraavista:
   - Valitse Microsoft 365 -yhteensopivuuskeskus <https://compliance.microsoft.com> -palvelussa **Ratkaisujen** \> **valvonta.** Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://compliance.microsoft.com/auditlogsearch> -
   - Valitse Microsoft 365 Defender <https://security.microsoft.com> -portaalissa **Valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://security.microsoft.com/auditlogsearch> -

    **Huomautus:** Jos näet ilmoituksen, että sinun on ottaa ominaisuus käyttöön, ota se käyttöön nyt. Jos ominaisuus ei ole käytössä, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.

2. Määritä **Valvonta-sivun** **Haku-välilehdessä** seuraavat asetukset:
   - **Päivämäärä- ja aikaalue:** Valitse päivämäärä-/aika-alue Aloitus- ja **Lopetus-ruuduista.** 
   - **Toiminnot:** Exchange **postilaatikon toiminnot** ja valitse sitten seuraavat arvot:
     - **Poistetut-kansiosta poistetut viestit**
     - **Viestit siirretty Poistetut-kansioon**

       Kun olet valmis, pienennä Toiminnot-ruutu napsauttamalla ruudun **ulkopuolella.**

   - **Käyttäjät:** Voit palauttaa kaikkien käyttäjien tulokset hyväksymällä tyhjän oletusarvon tai kirjoittamalla yhden tai useamman käyttäjän.

3. Kun olet valmis, valitse **Hae**. Toiminnot näkyvät uudella **Valvontahaku-sivulla.**

4. Avaa tietojen pikaikkuna valitsemalla toiminto tuloksista. Poistettua kohdetta koskevat lisätiedot, kuten aiherivi ja kohteen sijainti, kun kohde poistettiin, näkyvät **AffectedItems-kentässä.**

   **Huomautus:** Poistettuja kohteita ei voi palauttaa valvontalokitoiminnolla. Lisätietoja poistettujen kohteiden palauttamisesta [on kohdassa Poistettujen sähköpostiviestien palauttaminen Outlookin verkkoversio.](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)

Lisätietoja on kohdassa [Valvontalokista etsiminen yleisimpiä tukiongelmia tutkimista varten.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
