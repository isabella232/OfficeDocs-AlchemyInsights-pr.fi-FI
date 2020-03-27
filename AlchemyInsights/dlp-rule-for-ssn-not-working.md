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
ms.openlocfilehash: 4ec0df9d4954a8c65f0c34188d285dd8cf44a4f2
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977303"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-ongelmat sosiaaliturvanumeroissa

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat edelleen erittäin saatavilla – lisätietoja on [SharePoint Onlinen tilapäisissä ominaisuusoikaisuissa.](https://aka.ms/ODSPAdjustments)

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
  