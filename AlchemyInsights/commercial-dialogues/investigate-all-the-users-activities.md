---
title: Kaikkien käyttäjien toimintojen tutkiminen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332340"
---
# <a name="investigate-all-the-users-activities"></a>Kaikkien käyttäjien toimintojen tutkiminen

Voit tehdä tämän näin:

1. Tee jokin seuraavista:
   - Valitse Microsoft 365 -yhteensopivuuskeskus <https://compliance.microsoft.com> -palvelussa **Ratkaisujen** \> **valvonta.** Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://compliance.microsoft.com/auditlogsearch> -
   - Valitse Microsoft 365 Defender <https://security.microsoft.com> -portaalissa **Valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://security.microsoft.com/auditlogsearch> -

    **Huomautus:** Jos näet ilmoituksen, että sinun on ottaa ominaisuus käyttöön, ota se käyttöön nyt. Jos ominaisuus ei ole käytössä, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.

2. Määritä **Valvonta-sivun** **Haku-välilehdessä** seuraavat asetukset:
   - **Päivämäärä- ja aikaalue:** Valitse päivämäärä-/aika-alue Aloitus- ja **Lopetus-ruuduista.** 
   - **Toiminnot:** Jos olet kiinnostunut tietystä aktiviteetista, valitse se luettelosta; Muussa tapauksessa oletusarvo Näytä kaikkien **toimintojen tulokset palauttaa** kaikki toiminnot.
   - **Käyttäjät:** Voit palauttaa kaikkien käyttäjien tulokset hyväksymällä tyhjän oletusarvon tai kirjoittamalla yhden tai useamman käyttäjän.

3. Kun olet valmis, valitse **Hae**. Toiminnot näkyvät uudella **Valvontahaku-sivulla.** Näet IP-osoitteen , **Käyttäjän** **ja** **aktiviteetin** nimen.

4. Lataa tulokset valitsemalla Vie **Lataa** \> **kaikki tulokset**.

5. Avaa tietojen pikaikkuna valitsemalla toiminto tuloksista.

Lisätietoja on kohdassa [Valvontalokista etsiminen ja yleisimmät tukiongelmat.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
