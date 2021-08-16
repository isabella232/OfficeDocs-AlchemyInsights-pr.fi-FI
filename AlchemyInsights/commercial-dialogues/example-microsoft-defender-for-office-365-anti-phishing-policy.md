---
title: Esimerkki Microsoft Defender for Office 365 tietojenkalastelun torjuntakäytännöstä
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035003"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Esimerkki Microsoft Defender for Office 365 tietojenkalastelun torjuntakäytännöstä

Nämä asetukset mahdollistavat käytännön nimeltä Toimialue *ja toimitusjohtaja.* Tämä käytäntö tarjoaa sekä käyttäjän että toimialueen tekeytymisen, ja sen jälkeen käytäntöä sovelletaan kaikkiin sähköpostiviesteihin, jotka käyttäjät vastaanotetaan toimialueella. Lisää ensin seuraavat tiedot käytännön luomiseen:

- **Nimi:** Toimialueen ja **toimitusjohtajan kuvaus:** Varmistaa, että toimitusjohtaja ja toimialueesi eivät tekeyy tekeytymään.
  **Käytössä:** Valitse **Vastaanottajan toimialue on**. Valitse **Mikä tahansa näistä** **-kohdassa Valitse** ja valitse sitten toimialue. Valitse **+ Lisää**. Valitse luettelossa toimialueen nimen vieressä olevaa valintaruutua (esimerkiksi contoso.com *)* ja valitse sitten **Lisää**. Valitse **Valmis**.
- Kun käytäntö on luotu, voit hienosäätää sitä seuraavilla asetuksilla:
  - **Käyttäjien lisääminen suojattavaksi:** Lisää tässä esimerkissä toimitusjohtajan sähköpostiosoite vähintään.
  - **Suojaa lisäämällä toimialueita:** Lisää organisaatiotoimialue, joka sisältää toimitusjohtajan toimiston.
  - **Valitse toiminnot:** **Jos** sähköpostin lähettänyt tekeytynyt käyttäjä , valitse Ohjaa viesti toiseen sähköpostiosoitteeseen ja kirjoita sitten suojauksenvalvojan sähköpostiosoite (esimerkiksi *securityadmin@contoso.com).* Jos **sähköpostin lähettänyt toimialue on tekeytynyt,** valitse Aseta viesti **karanteeniin**.
  - **Postilaatikkotiedot:** Tämä asetus on valittuna oletusarvoisesti, kun luot uuden tietojenkalastelun torjuntakäytännön. Jätä tämä asetus **käytössä,** niin saat parhaan tuloksen.
  - **Luotettujen lähettäjien ja toimialueiden lisääminen:** Älä tässä esimerkissä määritä ohitusta.
- Kun olet tarkistanut asetukset, valitse **Luo tämä käytäntö tai** **Tallenna**.

Lisätietoja on kohdassa Tietojen [kalastelun estokäytännöt Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
