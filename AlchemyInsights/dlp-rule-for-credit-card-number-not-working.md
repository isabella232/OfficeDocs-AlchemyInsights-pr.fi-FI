---
title: DLP-sääntö, luottokorttinumero ei toimi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919077"
---
Onko sinulla ongelmia kanssa **Tietojen menetyksen ehkäisyyn (DLP)** , jossa **Luottokortin numeroa** käytettäessä DLP luottamuksellisten tietojen tyyppi O365 sisällölle ei toimi? Jos näin on, varmista, että sisältösi on antamaan tarvittavia tietoja DLP-käytäntö, kun sitä arvioidaan. Esimerkiksi **luottokortin käytäntö** määritetty 85 %: n varmuudella, seuraavat arvioidaan ja havaittu käynnistää säännön: 
  
- **[Muoto:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 numeroa, joka on muotoiltu tai Muotoilematon (dddddddddddddddd) ja on läpäistävä testi Luhn. 
    
- **[Kuvio:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Erittäin monimutkaisia ja vakaan kuvio, joka havaitsee kaikki suuret tuotemerkkejä kaikkialla maailmassa, kuten Visa, Mastercard, löytää kortin, JCB, American Express, lahjakortteja ja diner korttien maiden kortteja. 
    
- **[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Kyllä, Luhn tarkistussumma 
    
- **[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP-käytäntö on 85 % varma siitä, että se on havainnut arkaluonteisia henkilötietoja Jos läheisyydessä 300 merkkiä sisällä: 
    
  - Func_credit_card-funktio etsii mallia vastaavia kohtia.
    
  - Jokin seuraavista pitää paikkansa: 
    
  - -Keyword_cc_verification avainsana on löytynyt.
    
  - Avainsana-Keyword_cc_name löytyy
    
  - Func_expiration_date-funktio etsii päivämäärä oikean päivämäärän muodossa.
    
  - Tarkistussumma osumia
    
    Esimerkiksi seuraava esimerkki aiheuttaa käytännön DLP luottokortin numero:
    
  - Viisumi: 4485 3647 3952 7352 
    
  - Voimassaoloaika päättyy: 2/2009
    
Lisätietoja mitä tarvitaan, jotta voidaan havaita sisällön **Luottokorttinumero** , katso tämän artikkelin seuraavassa osassa: [Mitä on herkkä tietotyypit etsii luottokortin #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Käyttämällä erilaisia sisäisiä luottamuksellisia tietoja, seuraavasta artikkelista lisätietoja, mitä tarvitaan muissa yhteyksissä: [Etsi mitä luottamuksellisten tietojen tyypit](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

