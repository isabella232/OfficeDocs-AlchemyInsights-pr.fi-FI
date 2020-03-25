---
title: Luottokortin numeron DLP-sääntö ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932440"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-ongelmat luottokorttien numeroissa

**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan. Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut. Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.

Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan. Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina. Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.

**DLP-ongelmat luottokorttien numeroissa**

Onko sinulla ongelmia **DLP (Data Loss Prevention) -toiminnon kanssa,** joka ei toimi **luottokortin numeron** sisältävän sisällön kanssa, kun käytät DLP-arkaluonteista tietotyyppiä O365:ssä? Jos näin on, varmista, että sisältösi sisältää tarvittavat tiedot DLP-käytännön käynnistämiseen, kun sitä arvioidaan. Esimerkiksi **luottokorttikäytännössä,** jonka luotettavuustaso on 85 %, arvioidaan seuraavat tiedot, ja ne on tunnistettava, jotta sääntö käynnistyy:
  
- **[Muoto:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 numeroa, jotka voidaan muotoilla tai muotoilematon (ddddddddddddddddddddddddddddddd.

- **[Mallineule:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Erittäin monimutkainen ja vankka kuvio, joka havaitsee kortit kaikilta maailman suurilta brändeiltä, mukaan lukien Visa, MasterCard, Discover Card, JCB, American Express, lahjakortit ja diner-kortit.

- **[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Kyllä, Luhnin tarkistussumma

- **[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP-käytäntö on 85 %: n varma siitä, että se on havainnut tämäntyyppisiä arkaluonteisia tietoja, jos 300 merkin etäisyydellä:

  - Funktio Func_credit_card etsii kaavaa vastaavaa sisältöä.

  - Jokin seuraavista on totta:

  - Keyword_cc_verification avainsana löytyy.

  - Keyword_cc_name avainsana löytyy

  - Funktio Func_expiration_date löytää päivämäärän oikeassa päivämäärämuodossa.

  - Tarkistussumma kulkee

    Esimerkiksi seuraava esimerkki käynnistidänsä DLP-luottokortin numerokäytännön:

  - Viisumi: 4485 3647 3952 7352
  
  - Päättyy: 2/2009

Lisätietoja siitä, mitä vaaditaan, jotta **luottokorttinumero** voidaan havaita sisällöllesi, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät luottokorttia#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Toisen sisäisen arkaluonteisen tietotyypin avulla on seuraavassa artikkelissa tietoja siitä, mitä muille tyypeille tarvitaan: [Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  