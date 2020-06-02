---
title: DLP-sääntö, jos SSN ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507367"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-ongelmat sosiaaliturvatunnusten kanssa

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP-ongelmat SSN:ssä**

Onko sinulla ongelmia, kun **tietoja katoamisen estämisessä (DLP)** ei ole käytössä sisältöä, joka sisältää **SSN:n (SSN),** kun käytät microsoft 365:n arkaluonteista tietotyyppiä? Jos näin on, varmista, että sisältö sisältää tarvittavat tiedot siitä, mitä DLP-käytäntö etsii. 
  
Esimerkiksi SSN-käytännössä, jonka luotettavuustaso on 85 %, arvioidaan seuraavat tiedot, jotka on tunnistettava, jotta sääntö käynnistyisi:
  
- **[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 numeroa, jotka voivat olla muotoiltu tai muotoilematon kuvio

- **[Mallineule:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neljä toimintoa etsiä SSNs neljä eri malleja:

  - Func_ssn etsii SSN-nit, joiden ennen 2011 -muotoista muotoilua on muotoiltu viivoilla tai välilyönneillä (ddd-dd-dddd OR ddd ddddd)

  - Func_unformatted_ssn etsii SSN-nit, joiden ennen vuotta 2011 on vahva muotoilu ja jotka eivät ole muotoiltu yhdeksäksi peräkkäiseksi numeroksi (ddddddddd)

  - Func_randomized_formatted_ssn etsii vuoden 2011 jälkeisiä SSN-nistoja, jotka on muotoiltu vikoilla tai välilyönneillä (ddd-dd-dddd OR ddd ddddd)

  - Func_randomized_unformatted_ssn etsii vuoden 2011 jälkeisiä SSN-numeroita, jotka ovat muotoilemattomia yhdeksäksi peräkkäiseksi numeroksi (dddddddd)

- **[Tarkistussumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ei, tarkistussummaa ei ole.

- **[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP-käytäntö on 85% varma siitä, että se on havainnut tällaisia arkaluonteisia tietoja, jos 300 merkin läheisyydessä:

  - [Funktio Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) etsii kuviota vastaavaa sisältöä.

  - Avainsana [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) löytyy. Esimerkkejä avainsanoista ovat: *Sosiaaliturva, Sosiaaliturva#, Soc Sec, SSN* . Esimerkiksi seuraava esimerkki käynnistäisi DLP SSN -käytännön: **SSN: 489-36-8350**
  
Lisätietoja siitä, mitä ssn-tekniikat ovat velvollisia havaitsemaan sisältöäsi varten, on seuraavassa tämän artikkelin osassa: [Mitä arkaluonteiset tietotyypit etsivät SSN-tyyppejä](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Jos käytät eri sisäänrakennettua arkaluonteista tietotyyppiä, lue seuraavassa artikkelissa tietoja siitä, mitä tarvitaan muuntyyppisille [tyypeille: Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  