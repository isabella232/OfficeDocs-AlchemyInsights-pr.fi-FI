---
title: DLP sääntö SSN ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932518"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-ongelmat sosiaaliturvanumeroissa

**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan. Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut. Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.

Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan. Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina. Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.

**DLP-ongelmat ssns**

Onko sinulla ongelmia **dlp(Data Loss Prevention) -toiminnon kanssa,** joka ei toimi **sosiaaliturvatunnuksen (SSN)** sisältävän sisällön kanssa, kun käytät arkaluonteista tietotyyppiä Office 365:ssä? Jos näin on, varmista, että sisältö sinetaan tarvittavat tiedot siitä, mitä DLP-käytäntö etsii. 
  
Esimerkiksi SSN-käytännölle, jonka luotettavuustaso on 85 %, arvioidaan seuraavat tiedot, ja ne on tunnistettava, jotta sääntö käynnistyy:
  
- **[Muoto:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 numeroa, jotka voivat olla muotoiltutai muotoilematon kuvio

- **[Mallineule:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neljä toimintoa etsii ssns neljässä eri malleja:

  - Func_ssn etsii ssn-nijät, joiden muotoilu on ennen vuoden 2011 vahvaa ja jotka on muotoiltu viivoilla tai välilyönneillä (ddd-dd-dddd OR ddd dd ddddd)

  - Func_unformatted_ssn löytää ssn-nijät, joiden vahva muotoilu on ennen vuotta 2011 ja joita ei ole muotoiltu yhdeksäksi peräkkäiseksi numeroksi (dddddddd)

  - Func_randomized_formatted_ssn etsii vuoden 2011 jälkeisiä ssn-naatteja, jotka on muotoiltu viivoilla tai välilyönneillä (ddd-dd-ddd OR ddd dd ddddd)

  - Func_randomized_unformatted_ssn löytää vuoden 2011 jälkeiset ssnit, joita ei ole muotoiltu yhdeksäksi peräkkäiseksi numeroksi (dddddddd)

- **[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ei, ei ole Checksumia.

- **[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP-käytäntö on 85 %: n varma siitä, että se on havainnut tämäntyyppisiä arkaluonteisia tietoja, jos 300 merkin etäisyydellä:

  - Toiminto [Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) etsii kaavaa vastaavaa sisältöä.

  - [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) avainsana löytyy. Avainsanoja ovat esimerkiksi *sosiaaliturva, sosiaaliturva#, Soc Sec ,SSN* . Esimerkiksi seuraava esimerkki käynnistäisi DLP SSN -käytännön: **SSN: 489-36-8350**
  
Lisätietoja siitä, mitä sisällön ssn-nimiselle tunnistettaviksi tarvitaan, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät ssn-verkkoja](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Toisen sisäisen arkaluonteisen tietotyypin avulla on seuraavassa artikkelissa tietoja siitä, mitä muille tyypeille tarvitaan: [Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  