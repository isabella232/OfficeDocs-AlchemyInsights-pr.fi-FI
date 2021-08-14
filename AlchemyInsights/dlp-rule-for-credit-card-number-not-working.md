---
title: Luottokorttinumeron DLP-sääntö ei toimi
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005087"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-ongelmat luottokorttinumeroissa

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP-ongelmat luottokorttinumeroissa**

Onko sinulla ongelmia tietojen menetyksen estämisen **(DLP)** kanssa, joka ei toimi luottokortin numeron sisältävässä sisällössä, kun käytät DLP:n luottamuksellista tietotyyppiä O365:ssä?  Jos näin on, varmista, että sisältösi sisältää tarvittavat tiedot, jotta DLP-käytäntö voidaan käynnistää, kun se arvioidaan. Jos esimerkiksi luottokorttikäytäntö on määritetty 85 prosentin luottamustasolla, seuraavat tiedot arvioidaan, ja ne on tunnistettava, jotta sääntö käynnistää: 
  
- **[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 numeroa, jotka voidaan muotoilla tai joita ei voi muotoilla (dddddd) ja joiden on läpäistävä Luhn-testi.

- **[Kaava:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Erittäin monimutkainen ja tehokas kaava, joka havaitsee kaikkien tärkeimpien merkkien kortteja ympäri maailmaa, mukaan lukien Visa, MasterCard, Discover Card, JCB, American Express, lahjakortit ja diner-kortit.

- **[Tarkistussumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Kyllä, Luhnin tarkistussumma

- **[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP-käytäntö on 85-prosenttisesti varma siitä, että se on havainnut luottamuksellisia tietoja, jos 300 merkin sisällä:

  - Funktio Func_credit_card löytää kaavaa vastaavaa sisältöä.

  - Jokin seuraavista pitää paikkansa:

  - Hakusana kohteesta Keyword_cc_verification löytyy.

  - Hakusana kohteesta Keyword_cc_name löytyy

  - Funktio Func_expiration_date löytää päivämäärän oikeassa päivämäärämuodossa.

  - Tarkistussumma on ohitettu

    Esimerkiksi seuraava esimerkki käynnisti DLP-luottokorttinumerokäytännön:

  - Visa: 4485 3647 3952 7352
  
  - Päättyy: 2.2.2009

Lisätietoja siitä, mitä sisältö  edellyttää luottokorttinumeron havaitsemiseen, on tämän artikkelin seuraavassa osiossa: Mitä Luottamukselliset tietotyypit näyttävät [luottokortilta#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Jos käytössäsi on erilainen sisäinen luottamuksellisten tietojen tyyppi, katso seuraavasta artikkelista tietoja siitä, mitä muuntyyppiset tiedot tarvitaan: Mitä Luottamukselliset tietotyypit [-kohta näyttää](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  