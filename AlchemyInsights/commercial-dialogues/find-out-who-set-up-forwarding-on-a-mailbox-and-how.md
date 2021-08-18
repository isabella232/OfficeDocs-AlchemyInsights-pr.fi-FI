---
title: Ota selvää, kuka on määrittänyt edelleenlähetystä postilaatikossa ja miten
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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317805"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Ota selvää, kuka on määrittänyt edelleenlähetystä postilaatikossa ja miten

Jos postilaatikossa on määritetty ulkoinen edelleenlähetys, toiminta valvotaan osana **Set-Mailbox-cmdlet-komentoa.** Voit etsiä toiminnon valvontalokista näin:

1. Tee jokin seuraavista:
   - Valitse Microsoft 365 -yhteensopivuuskeskus <https://compliance.microsoft.com> -palvelussa **Ratkaisujen** \> **valvonta.** Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://compliance.microsoft.com/auditlogsearch> -
   - Valitse Microsoft 365 Defender <https://security.microsoft.com> -portaalissa **Valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://security.microsoft.com/auditlogsearch> -

   **Huomautus:** Jos näet ilmoituksen, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt. Jos tämä toiminto ei ole käytössä, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.

2. Varmista **Valvonta-sivulla,** että **Haku-välilehti** on valittuna, ja määritä sitten seuraavat asetukset:
   - Valitse päivämäärä- ja aikaalue Aloitus- ja **Loppu-ruuduissa.** 
   - Tarkista, että Toiminnot-ruudussa **on Näytä kaikkien toimintojen tulokset**. 

3. Kun olet valmis, valitse **Hae**. Toiminnot näkyvät uudella **Valvontahaku-sivulla.**

4. Lajittele tulokset valitsemalla **hakutuloksista** Toiminta-sarake ja etsi sitten **Set-Mailbox -merkinnät.**

5. Avaa tietojen pikaikkuna valitsemalla toiminto tuloksista. Tarkista kunkin valvontatietueen tiedot ja selvitä, liittyykö toiminto sähköpostin edelleenlähetystän:
   - **ObjectId:** Muokatun postilaatikon aliasarvo.
   - **Parametrit:** _ForwardingSmtpAddress osoittaa_ kohdesähköpostiosoitteen.
   - **UserId:** Käyttäjä, joka määritti sähköpostin edelleenlähetystä postilaatikossa **ObjectId-kentässä.**

Lisätietoja on kohdassa [Postilaatikon sähköpostin edelleenlähetysten määritysten selvittäminen.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
