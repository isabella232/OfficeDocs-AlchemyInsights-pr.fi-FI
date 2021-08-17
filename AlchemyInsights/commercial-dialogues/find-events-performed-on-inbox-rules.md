---
title: Saapuneet-kansion sääntöjen tapahtumien etsiminen
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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313496"
---
# <a name="find-events-performed-on-inbox-rules"></a>Saapuneet-kansion sääntöjen tapahtumien etsiminen

Kun Saapuneet-kansion sääntöjä luodaan, muutetaan tai poistetaan, tapahtumat tallennetaan valvontalokiin. Voit tarkastella niitä näin:

1. Tee jokin seuraavista:
   - Valitse Microsoft 365 -yhteensopivuuskeskus <https://compliance.microsoft.com> -palvelussa **Ratkaisujen** \> **valvonta.** Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://compliance.microsoft.com/auditlogsearch> -
   - Valitse Microsoft 365 Defender <https://security.microsoft.com> -portaalissa **Valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://security.microsoft.com/auditlogsearch> -

    **Huomautus:** Jos näet ilmoituksen, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt. Jos tämä toiminto ei ole käytössä, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.
1. Valitse Toiminnot-kenttä, etsi Exchange postilaatikon toiminnot ja valitse New-InboxRule Luo Saapuneet-kansion sääntö Outlook Web App. Kun olet valmis, pienennä Toiminnot-ruutu napsauttamalla ruudun ulkopuolella.
1. Määritä päivämääräalue ja valitse sitten Käyttäjät-kentässä sen käyttäjän käyttäjänimi, jonka haluat tutkia. Voit valita useamman kuin yhden käyttäjän kerrallaan.
1. Valitse Hae. Toiminnot näkyvät Tulokset-kohdassa.
1. Voit tarkastella tietoja valitsemalla aktiviteetin ja valitsemalla sitten Lisätietoja. Parametrit-osassa näet säännön nimen, ehdot ja säännön toiminnot.

2. Määritä **Valvonta-sivun** **Haku-välilehdessä** seuraavat asetukset:
   - **Päivämäärä- ja aikaalue:** Valitse päivämäärä-/aika-alue Aloitus- ja **Lopetus-ruuduista.** 
   - **Toiminnot:** Valitse **Saapuneet-kansioSta Luo Saapuneet-kansion sääntö Outlook Web App**

3. Kun olet valmis, valitse **Hae**. Toiminnot näkyvät uudella **Valvontahaku-sivulla.**

4. Avaa tietojen pikaikkuna valitsemalla toiminto tuloksista. **Parametrit-osassa** näet säännön nimen, ehdot ja säännön toiminnot.

Lisätietoja on kohdassa [Valvontalokista etsiminen ja yleisimmät tukiongelmat.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
