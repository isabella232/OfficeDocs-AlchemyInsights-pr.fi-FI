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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882632"
---
# <a name="find-events-performed-on-inbox-rules"></a>Saapuneet-kansion sääntöjen tapahtumien etsiminen

Kun Saapuneet-kansion sääntöjä luodaan, muutetaan tai poistetaan, tapahtumat tallennetaan valvontalokiin. Voit tarkastella niitä näin:

1. Tee jokin seuraavista:
   - Valitse Microsoft 365 -yhteensopivuuskeskus <https://compliance.microsoft.com> :ssä Ratkaisujen  \> **valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://compliance.microsoft.com/auditlogsearch> -
   - Valitse Microsoft 365 Defender -portaalissa <https://security.microsoft.com> **Valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://security.microsoft.com/auditlogsearch> -

    > [!NOTE]
    > Jos huomaat, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt. Jos tämä toiminto ei ole käytössä, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.

2. Määritä **Valvonta-sivun** **Haku-välilehdessä** seuraavat asetukset:
   - **Päivämäärä- ja aikaalue:** Valitse päivämäärä-/aika-alue Aloitus- ja **Lopetus-ruuduista.** 
   - **Toiminnot:** Valitse **Uusi Saapuneet-kansioRule Luo Saapuneet-kansion sääntö Outlook Web App**

3. Kun olet valmis, valitse **Hae**. Toiminnot näkyvät uudella **Valvontahaku-sivulla.**

4. Avaa tietojen pikaikkuna valitsemalla toiminto tuloksista. **Parametrit-osassa** näet säännön nimen, ehdot ja säännön toiminnot.

Lisätietoja on kohdassa [Valvontalokista etsiminen ja yleisimmät tukiongelmat.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
