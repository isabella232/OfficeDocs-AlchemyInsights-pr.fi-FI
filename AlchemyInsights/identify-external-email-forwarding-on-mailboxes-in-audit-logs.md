---
title: Ulkoisen sähköpostin edelleenlähetysten tunnistaminen postilaatikoissa valvontalokeihin
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331156"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ulkoisen sähköpostin edelleenlähetysmäärityksen tunnistaminen postilaatikoissa

Kun Microsoft 365 määrittää postilaatikon ulkoisen sähköpostin edelleenlähetystä, toiminta valvotaan osana **Set-Mailbox-cmdlet-komentoa.** Näet toiminnon valvontalokihaun avulla. Voit tehdä sen näin.

1. Tee jokin seuraavista toimista:
   - Valitse Microsoft 365 -yhteensopivuuskeskus <https://compliance.microsoft.com> -palvelussa **Ratkaisujen** \> **valvonta.** Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://compliance.microsoft.com/auditlogsearch> -
   - Valitse Microsoft 365 Defender <https://security.microsoft.com> -portaalissa **Valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://sip.security.microsoft.com/auditlogsearch> -

2. Varmista **Valvonta-sivulla,** että **Haku-välilehti** on valittuna, ja määritä sitten seuraavat asetukset:
   - Valitse päivämäärä- ja aikaalue Aloitus- ja **Loppu-ruuduissa.** 
   - Tarkista, että Toiminnot-ruudussa **on Näytä kaikkien toimintojen tulokset**. 

3. Kun olet valmis, valitse **Hae**. Toiminnot näkyvät uudella **Valvontahaku-sivulla.**

4. Valitse tuloksissa **Suodata tulokset** ja kirjoita **Toimintasuodatin-ruutuun Set-Mailbox.**

5. Valitse valvontatietue tuloksista. Valitse **Tiedot-pikaikkunassa** **Lisätietoja**. Sinun on tarkastettava kunkin valvontatietueen tiedot sen määrittämiseksi, liittyykö toiminto sähköpostin edelleenlähetystän.

   - **ObjectId:** Muokatun postilaatikon aliasarvo.
   - **Parametrit:** _ForwardingSmtpAddress osoittaa_ kohdesähköpostiosoitteen.
   - **UserId:** Käyttäjä, joka määritti sähköpostin edelleenlähetystä postilaatikossa **ObjectId-kentässä.**

Lisätietoja on kohdassa [Postilaatikon sähköpostin edelleenlähetysten määritysten selvittäminen.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
