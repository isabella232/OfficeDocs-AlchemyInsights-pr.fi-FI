---
title: DLP-säännön USA / UK passin numero ei toimi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29467720"
---
Onko sinulla ongelmia **Tietojen menetyksen ehkäisyyn (DLP)** ei toimi, joka sisältää sisällön kanssa **USA / UK passin numero** käytettäessä DLP luottamuksellisten tietojen tyyppi O365? Jos näin on, varmista, että sisältö on mitä DLP käytännön etsii kun sen arvioidaan tarvittavat tiedot. 
  
Esimerkiksi **USA / UK passin numero** 75 %: n varmuudella määritetty käytäntö, seuraavat arvioidaan ja käynnistää sääntö on havaittavissa 
  
- **[Muodossa:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Yhdeksän numeroa 
    
- **[Kuvio:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Yhdeksän peräkkäistä numeroa 
    
- **[Tarkistussumma:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole tarkistussumma 
    
- **[Määritelmä:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP-käytäntö on 75 % varma siitä, että se on havainnut arkaluonteisia henkilötietoja Jos läheisyydessä 300 merkkiä sisällä: 
    
  - Func_usa_uk_passport-funktio etsii mallia vastaavia kohtia.
    
  - -Keyword_passport avainsana on löytynyt.
    
    Esimerkiksi seuraava malli käynnistää **USA / UK passin numero** käytännön: Yhdysvaltain passin numero 123456789 
    
Lisätietoja mitä tarvitaan USA / UK passin numero, sisällön tunnistaminen on tämän artikkelin seuraavassa osassa: [Etsi mitä luottamuksellisten tietojen tyypit USA / UK passin numero](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Käyttämällä erilaisia sisäisiä luottamuksellisia tietoja, seuraavasta artikkelista lisätietoja, mitä tarvitaan muissa yhteyksissä: [Etsi mitä luottamuksellisten tietojen tyypit](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

