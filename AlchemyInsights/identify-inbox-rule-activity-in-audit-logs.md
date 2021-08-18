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
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331120"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Saapuneet-kansion säännön toiminnan tunnistaminen valvontalokeja varten

Voit tarkastella Saapuneet-kansion sääntöjen tapahtumia Microsoft 365 -yhteensopivuuskeskus valvontalokihaun avulla (Saapuneet-kansion sääntöjen luominen, muokkaaminen ja poistaminen).

1. Tee jokin seuraavista toimista:
   - Valitse Microsoft 365 -yhteensopivuuskeskus <https://compliance.microsoft.com> -palvelussa **Ratkaisujen** \> **valvonta.** Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://compliance.microsoft.com/auditlogsearch> -
   - Valitse Microsoft 365 Defender <https://security.microsoft.com> -portaalissa **Valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://security.microsoft.com/auditlogsearch> -

2. Määritä **Valvonta-sivun** **Haku-välilehdessä** seuraavat asetukset:
   - **Päivämäärä- ja aikaalue:** Valitse päivämäärä-/aika-alue Aloitus- ja **Lopetus-ruuduista.** 
   - **Toiminnot:** Valitse vähintään yksi seuraavista arvoista:
     - **Uusi Saapuneet-kansio Saapuneet-kansion säännön luominen Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Saapuneet-kansion sääntöjen päivittäminen Outlook asiakasohjelmasta**

3. Kun olet valmis, valitse **Hae**. Toiminnot näkyvät uudella **Valvontahaku-sivulla.**

4. Avaa tietojen pikaikkuna valitsemalla toiminto tuloksista. Tiedot Saapuneet-kansion sääntöasetuksista näkyvät **Parametrit-kentässä.**

Lisätietoja on kohdassa Käyttäjän [Luoman Saapuneet-kansion säännön selvittäminen.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
