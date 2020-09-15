---
title: DLP-sääntö ei toimi SSN-palvelussa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679366"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-ongelmat Sosiaaliturvanumeroissa

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP-ongelmat SSN:llä**

Onko sinulla ongelmia **tietojen menetyksen estämisen (DLP)** kanssa, joka ei toimi, jos sisältö sisältää **SOSIAALITURVANUMERON (SSN)** , kun Microsoft 365-palvelussa käytetään arkaluonteista tieto tyyppiä? Varmista, että sisältö sisältää tarvittavat tiedot siitä, mitä DLP-käytäntöä etsitään. 
  
Esimerkiksi SSN-käytännölle, jonka luotettavuus taso on 85%, lasketaan seuraavat ja on havaittu, että sääntö käynnistetään:
  
- **[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 numeroa, jotka voivat olla muotoiltuna tai muotoilemattomana kuviona

- **[Malli neule:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neljä funktiota näyttävät SSN:t neljässä eri kuvioissa:

  - Func_ssn löytää SSNS:n, jossa on ennen 2011 vahvaa muotoilua, joka on muotoiltu katko viivoilla tai väli lyönneillä (DDD-DD-dddd tai TDD DD dddd)

  - Func_unformatted_ssn löytää SSN-version, jossa on ennen 2011 vahvaa muotoilua, jonka muotoilu on yhdeksän peräkkäistä numeroa (ddddddddd)

  - Func_randomized_formatted_ssn löytää post-2011 SSN-merkit, jotka on muotoutunut viivoilla tai väli lyönneillä (DDD-DD-dddd tai TDD DD dddd)

  - Func_randomized_unformatted_ssn hakee post-2011-SSN-tunnukset, jotka ovat muotoilemattomia yhdeksässä peräkkäisessä numerona (ddddddddd)

- **[Tarkistus summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ei, tarkistus summaa ei ole

- **[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP-käytännöllä on 85% varma, että se havaitsee tämän tyyppisiä tietoja, jos se on 300-merkin lähellä:

  - [Funktio Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) löytää kaavaa vastaavaa sisältöä.

  - [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) avain sana löytyy. Esimerkkejä avain sanoista ovat:  *sosiaaliturva, sosiaaliturva #, SOC SEC, SSN*  . Esimerkiksi seuraava esimerkki käynnistäisi DLP SSN-käytäntöä: **SSN: 489-36-8350**
  
Jos haluat lisä tietoja siitä, mitä SSN:ltä edellytetään sisällölle, Lue tämän artikkelin seuraava osio: [mitä luottamukselliset tieto tyypit etsivät SSN:stä](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Jos käytät erilaista sisäistä arkaluonteista tieto tyyppiä, Katso lisä tietoja muista tieto tyypeistä, jotka ovat tarpeen: [mitä luottamukselliset tieto tyypit](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) etsivät
  