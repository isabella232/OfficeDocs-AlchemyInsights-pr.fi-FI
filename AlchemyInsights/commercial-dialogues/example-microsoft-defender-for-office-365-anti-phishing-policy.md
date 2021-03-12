---
title: Esimerkki Microsoft Defender for Office 365:n tietojenkalastelun estokäytännöstä
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746852"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Esimerkki Microsoft Defender for Office 365:n tietojenkalastelun estokäytännöstä

Nämä asetukset mahdollistavat käytännön nimeltä Toimialue *ja toimitusjohtaja.* Tämä käytäntö tarjoaa sekä käyttäjä- että toimialuesuojauksen tekeytymisviestiltä, ja sen jälkeen käytäntöä sovelletaan kaikkiin sähköpostiviesteihin, jotka käyttäjät ovat vastaanottaneet toimialueella. Luo ensin käytäntö lisäämällä seuraavat tiedot:

- **Nimi:** Toimialueen ja **toimitusjohtajan kuvaus:** Varmistaa, että toimitusjohtaja ja toimialueesi eivät tekeyty.
  **Käytössä:** Valitse **vastaanottajan toimialue on**. Valitse **jokin näistä** ja **valitse** sitten toimialue. Valitse **+ Lisää.** Valitse luettelossa toimialueen nimen vieressä olevaa valintaruutua (esimerkiksi *contoso.com)* ja valitse **sitten Lisää.** Valitse **Valmis.**
- Kun käytäntö on luotu, voit hienosäätää käytäntöä seuraavilla asetuksilla:
  - **Käyttäjien lisääminen suojattavaksi:** Lisää tässä esimerkissä vähintään toimitusjohtajan sähköpostiosoite.
  - **Suojaa lisäämällä toimialueita:** Lisää organisaatiotoimialue, joka sisältää toimitusjohtajan toimiston.
  - **Toimintojen valinta:** **Jos** sähköpostin on lähettänyt tekeytynyt käyttäjä, valitse Ohjaa viesti toiseen sähköpostiosoitteeseen ja kirjoita sitten suojauksenvalvojan sähköpostiosoite (esimerkiksi *securityadmin@contoso.com).*  Jos **sähköpostin lähettää tekeytynyt toimialue,** valitse **Aseta viesti karanteeniin.**
  - **Postilaatikkotiedot:** Tämä asetus on valittuna oletusarvoisesti, kun luot uuden tietojenkalastelukäytännön. Jätä tämä asetus **käyttöön,** niin saat parhaan tuloksen.
  - **Luotettujen lähettäjien ja toimialueiden lisääminen:** Älä määritä tässä esimerkissä ohitusta.
- Kun olet tarkistanut asetukset, valitse Luo **tämä käytäntö tai** **Tallenna.**

Lisätietoja on Microsoft [365:n](https://go.microsoft.com/fwlink/?linkid=2092235)tietojenkalastelun torjunnan käytännöt -kohdassa.
