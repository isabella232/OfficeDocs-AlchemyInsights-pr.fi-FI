---
title: DLP-sääntö, Meille pankkitilinumero ei toimi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916413"
---
Onko sinulla ongelmia **Tietojen menetyksen ehkäisyyn (DLP)** ei toimi sisällölle, joka sisältää **US pankkitilinumero** käytettäessä DLP luottamuksellisten tietojen tyypin O365 kanssa? Jos näin on, varmista, että sisältö on mitä DLP käytännön etsii kun sen arvioidaan tarvittavat tiedot. 
  
Esimerkiksi **Yhdysvaltalaisen pankkitilinumero** 85 %: n varmuudella määrittää käytännön, seuraavat arvioidaan ja havaittu käynnistää säännön: 
  
- **[Muodossa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 numeroa 
    
- **[Kuvio:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 peräkkäistä numeroa. 
    
- **[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole tarkistussumma 
    
- **[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP-käytäntö on 75 % varma siitä, että se on havainnut arkaluonteisia henkilötietoja Jos läheisyydessä 300 merkkiä sisällä: 
    
  - Regex_usa_bank_account_number säännöllinen lauseke löytää sisältöä, joka vastaa kaavaa
    
  - -Keyword_usa_Bank_Account avainsana on löytynyt.
    
    Esimerkiksi seuraava esimerkki käynnistää **Yhdysvaltojen pankkitilinumero** käytännön: Sekkitili 78344011 
    
Lisätietoja mitä tarvitaan, jotta voidaan havaita sisällön **Yhdysvaltojen pankkitilinumero** , katso tämän artikkelin seuraavassa osassa: [Mitä on herkkä tietotyypit etsiä US pankkitilinumero](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Käyttämällä erilaisia sisäisiä luottamuksellisia tietoja, seuraavasta artikkelista lisätietoja, mitä tarvitaan muissa yhteyksissä: [Etsi mitä luottamuksellisten tietojen tyypit](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

