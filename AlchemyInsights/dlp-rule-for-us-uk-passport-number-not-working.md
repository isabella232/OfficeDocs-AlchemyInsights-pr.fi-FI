---
title: DLP sääntö YHDYSVALTAIN / UK Passport Number ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931259"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Ongelmia DLP - USA / Iso-Britannia passin numerot

**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan. Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut. Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.

Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan. Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina. Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.

**DLP-ongelmat Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumeroiden kanssa**

Onko sinulla ongelmia **Data Loss Prevention (DLP)** ei toimi sisältöä, joka sisältää Yhdysvaltain ja Yhdistyneen **kuningaskunnan passin numero,** kun käytät DLP arkaluonteisia tietoja tyyppi O365? Jos näin on, varmista, että sisältösi sisältää tarvittavat tiedot siitä, mitä DLP-käytäntö etsii, kun sitä arvioidaan.
  
Esimerkiksi Yhdysvaltain **ja Yhdistyneen kuningaskunnan passin numerokäytännössä,** jonka luotettavuustaso on 75 %, arvioidaan seuraavat tiedot, ja ne on tunnistettava, jotta sääntö voi käynnistää
  
- **[Muoto:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Yhdeksän numeroa

- **[Mallineule:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Yhdeksän peräkkäistä numeroa

- **[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole Checksumia.

- **[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP-käytäntö on 75 %: n varma siitä, että se on havainnut tämäntyyppisiä arkaluonteisia tietoja, jos 300 merkin etäisyydellä:

  - Toiminto Func_usa_uk_passport etsii kaavaa vastaavaa sisältöä.

  - Keyword_passport avainsana löytyy.

    Esimerkiksi seuraava esimerkki käynnistäisi **Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumerokäytännön:** Yhdysvaltain passin numero 123456789

Lisätietoja siitä, mitä tarvitaan, jotta Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumero voidaan havaita sisällöllesi, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät YHDYSVALTAIN ja Yhdistyneen kuningaskunnan passin numeroa](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Toisen sisäisen arkaluonteisen tietotyypin avulla on seuraavassa artikkelissa tietoja siitä, mitä muille tyypeille tarvitaan: [Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  