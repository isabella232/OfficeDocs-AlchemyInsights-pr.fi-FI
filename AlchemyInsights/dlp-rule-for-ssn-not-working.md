---
title: SSN-ei toimi DLP-sääntö
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 7242bf2b101b45fec0fe00ab33fa6db150004ee5
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657356"
---
Onko sinulla ongelmia kanssa **Tietojen menetyksen ehkäisyyn (DLP)** sisällön sisältävän **Henkilötunnus (SSN)** luottamuksellisten tietojen tyyppiä käytettäessä Office 365: ssä ei toimi? Jos näin on, varmista, että sisältösi on DLP-käytäntö on selvittämiseen tarvittavia tietoja. 
  
Esimerkiksi määritetty 85 %: n varmuudella SSN-käytäntö, seuraavat arvioidaan ja havaittu käynnistää säännön:
  
- **[Muoto:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 numeroa, joka voi olla muotoiltuna tai muotoilemattomana kuvio 
    
- **[Kuvio:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neljä Funktiot Etsi SSNs neljä eri kuviot: 
    
  - Func_ssn löytää SSNs ja pre-2011 vahva muotoilu, jotka on muotoiltu väliviivoja tai välilyöntejä (ddd-pp-dddd tai ddd pp dddd)
    
  - Func_unformatted_ssn löytää SSNs ja pre-2011 vahva muotoilu, joka on alustettu yhdeksän peräkkäistä merkkiä (ddddddddd)
    
  - Func_randomized_formatted_ssn löytää post-2011 SSNs, jotka on muotoiltu väliviivoja tai välilyöntejä (ddd-pp-dddd tai ddd pp dddd)
    
  - Func_randomized_unformatted_ssn löytää post-2011 SSNs, joka on alustettu yhdeksän peräkkäistä merkkiä (ddddddddd)
    
- **[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ei, ei ole tarkistussumma 
    
- **[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP-käytäntö on 85 % varma siitä, että se on havainnut arkaluonteisia henkilötietoja Jos läheisyydessä 300 merkkiä sisällä: 
    
  - [Func_ssn-funktio](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) etsii kuviota vastaava sisältö. 
    
  - - [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) avainsana on löytynyt. Sisältää esimerkkejä avainsanat: *sosiaaliturva, sosiaaliturvan #, Soc s, SSN* . Esimerkiksi seuraava esimerkki käynnistää käytännön DLP SSN: **SSN: 489-36-8350**
    
Katso lisätietoja mitä tarvitaan sisällön tunnistaminen SSNs on tämän artikkelin seuraavassa osassa: [Mitä on herkkä tietotyypit etsiä SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Käyttämällä erilaisia sisäisiä luottamuksellisia tietoja, seuraavasta artikkelista lisätietoja, mitä tarvitaan muissa yhteyksissä: [Etsi mitä luottamuksellisten tietojen tyypit](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

