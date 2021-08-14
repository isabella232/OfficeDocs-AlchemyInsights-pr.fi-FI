---
title: SSN:n DLP-sääntö ei toimi
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
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004979"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-ongelmat sosiaaliturvatunnuksen kanssa

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP-ongelmat SSN:ssä**

Onko sinulla ongelmia tietojen menetyksen estämisen **(DLP)** kanssa, joka ei toimi sosiaaliturvatunnusta **sisältävässä** sisällössä, kun käytät luottamuksellisten tietojen tyyppiä Microsoft 365? Jos näin on, varmista, että sisältösi sisältää tarvittavat tiedot DLP-käytännön etsimistä varten. 
  
Jos esimerkiksi SSN-käytäntö on määritetty 85 %:n luottamustasolla, arvioidaan seuraava, ja se on tunnistettava, jotta sääntö käynnistää:
  
- **[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 numeroa, jotka voivat olla muotoillun tai muotoilemattoman kuvion mukaisesti

- **[Kaava:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neljä funktiota etsi SSN-kaavoja neljässä eri kaavassa:

  - Func_ssn löytää vuotta 2011 edeltävät vahvat muotoilut, jotka on muotoiltu viivoilla tai välilyönneillä (ddd-dd-dddd TAI ddd dd dddd)

  - Func_unformatted_ssn löytää vuotta 2011 edeltävät vahvat muotoilut, joiden muotoilua ei ole muotoiltu yhdeksäksi peräkkäiseksi numeroksi (ddddddddd)

  - Func_randomized_formatted_ssn etsii vuoden 2011 jälkeiset SSN-tiedot, jotka on muotoiltu viivoilla tai välilyönneillä (ddd-dd-dddd TAI ddd dd dddd)

  - Func_randomized_unformatted_ssn etsii vuoden 2011 jälkeiset SSN-tiedot, joita ei ole muotoiltu yhdeksäksi peräkkäiseksi numeroksi (ddddddddd)

- **[Tarkistussumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ei, tarkistussummaa ei ole

- **[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP-käytäntö on 85-prosenttisesti varma siitä, että se on havainnut luottamuksellisia tietoja, jos 300 merkin sisällä:

  - Funktio [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) löytää kaavaa vastaavaa sisältöä.

  - Hakusana kohteesta [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) löytyy. Avainsanojen esimerkkejä ovat: *Sosiaaliturva, Sosiaaliturva#, Soc Sec, SSN.* Esimerkiksi seuraava esimerkki käynnisti DLP:n SSN-käytännön: **SSN: 489-36-8350**
  
Lisätietoja siitä, mitä sisällössäsi tunnistetaan SSN:t, on tämän artikkelin seuraavassa osiossa: Mitä luottamukselliset tietotyypit näyttävät [SSN-tyypeillä?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Jos käytössäsi on erilainen sisäinen luottamuksellisten tietojen tyyppi, katso seuraavasta artikkelista tietoja siitä, mitä muuntyyppiset tiedot tarvitaan: Mitä Luottamukselliset tietotyypit [-kohta näyttää](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  