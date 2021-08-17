---
title: Saapuneet-kansion säännön toiminnan tunnistaminen valvontalokeja varten
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891292"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Saapuneet-kansion säännön toiminnan tunnistaminen valvontalokeja varten

Voit tarkastella Saapuneet-Microsoft 365 -yhteensopivuuskeskus (Saapuneet-kansion sääntöjen luomista, muokkaamista ja poistamista) käyttämällä valvontalokihakua.

1. Tee jokin seuraavista toimista:
   - Valitse Microsoft 365 -yhteensopivuuskeskus <https://compliance.microsoft.com> :ssä Ratkaisujen  \> **valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://compliance.microsoft.com/auditlogsearch> -
   - Valitse Microsoft 365 Defender -portaalissa <https://security.microsoft.com> **Valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://security.microsoft.com/auditlogsearch> -

2. Määritä **Valvonta-sivun** **Haku-välilehdessä** seuraavat asetukset:
   - **Päivämäärä- ja aikaalue:** Valitse päivämäärä-/aika-alue Aloitus- ja **Lopetus-ruuduista.** 
   - **Toiminnot:** Valitse vähintään yksi seuraavista arvoista:
     - **Uusi Saapuneet-kansio Saapuneet-kansion säännön luominen Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Saapuneet-kansion sääntöjen päivittäminen Outlook asiakasohjelmasta**

3. Kun olet valmis, valitse **Hae**. Toiminnot näkyvät uudella **Valvontahaku-sivulla.**

4. Avaa tietojen pikaikkuna valitsemalla toiminto tuloksista. Tiedot Saapuneet-kansion sääntöasetuksista näkyvät **Parametrit-kentässä.**

Lisätietoja on kohdassa Käyttäjän [Luoman Saapuneet-kansion säännön selvittäminen.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
