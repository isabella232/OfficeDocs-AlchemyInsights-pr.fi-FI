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
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895176"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Ota selvää, kuka on määrittänyt edelleenlähetystä postilaatikossa ja miten

Jos postilaatikossa on määritetty ulkoinen edelleenlähetys, toiminta valvotaan osana **Set-Mailbox-cmdlet-komentoa.** Voit etsiä toiminnon valvontalokista näin:

1. Tee jokin seuraavista:
   - Valitse Microsoft 365 -yhteensopivuuskeskus <https://compliance.microsoft.com> -palvelussa Ratkaisujen  \> **valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://compliance.microsoft.com/auditlogsearch> -
   - Valitse Microsoft 365 Defender <https://security.microsoft.com> -hallintaportaalissa **Valvonta**. Jos haluat siirtyä suoraan **Valvonta-sivulle,** käytä <https://security.microsoft.com/auditlogsearch> -

   > [!NOTE]
   > Jos huomaat, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt. Jos tämä toiminto ei ole käytössä, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.

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
