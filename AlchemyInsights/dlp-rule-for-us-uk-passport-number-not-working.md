---
title: DLP-säännön USA / UK passin numero ei toimi
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
ms.openlocfilehash: 0567e9521507bcc192b187d0e5a8a0658332ff99
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389538"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP - ongelmia US / UK passi numerot

Onko sinulla ongelmia **Tietojen menetyksen ehkäisyyn (DLP)** ei toimi, joka sisältää sisällön kanssa **USA / UK passin numero** käytettäessä DLP luottamuksellisten tietojen tyyppi O365? Jos näin on, varmista, että sisältö on mitä DLP käytännön etsii kun sen arvioidaan tarvittavat tiedot.
  
Esimerkiksi **USA / UK passin numero** 75 %: n varmuudella määritetty käytäntö, seuraavat arvioidaan ja käynnistää sääntö on havaittavissa
  
- **[Muodossa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Yhdeksän numeroa

- **[Kuvio:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Yhdeksän peräkkäistä numeroa

- **[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole tarkistussumma

- **[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP-käytäntö on 75 % varma siitä, että se on havainnut arkaluonteisia henkilötietoja Jos läheisyydessä 300 merkkiä sisällä:

  - Func_usa_uk_passport-funktio etsii mallia vastaavia kohtia.

  - -Keyword_passport avainsana on löytynyt.

    Esimerkiksi seuraava malli käynnistää **USA / UK passin numero** käytännön: Yhdysvaltain passin numero 123456789

Lisätietoja mitä tarvitaan USA / UK passin numero, sisällön tunnistaminen on tämän artikkelin seuraavassa osassa: [Etsi mitä luottamuksellisten tietojen tyypit USA / UK passin numero](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Käyttämällä erilaisia sisäisiä luottamuksellisia tietoja, seuraavasta artikkelista lisätietoja, mitä tarvitaan muissa yhteyksissä: [Etsi mitä luottamuksellisten tietojen tyypit](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  