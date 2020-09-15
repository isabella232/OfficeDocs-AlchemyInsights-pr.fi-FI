---
title: DLP-sääntö luotto kortin numerolle ei toimi
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
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679438"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-ongelmat luotto kortti numeroilla

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP-ongelmat luotto kortti numeroilla**

Onko sinulla ongelmia **tietojen menetyksen estämisen (DLP)** kanssa, jos sisältö, joka sisältää **luotto kortin numeron** , ei toimi O365? Jos näin on, varmista, että sisältö sisältää tarvittavat tiedot, joiden avulla voit käynnistää DLP-käytäntöä, kun se lasketaan. Esimerkiksi **luotto kortti käytännölle** , jonka luotettavuus taso on 85%, on määritettävä seuraavat tiedot ja niiden on oltava havaittu, jotta sääntö käynnistetään:
  
- **[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 numeroa, jotka voidaan muotoilla tai muotoilemattomana (dddddddddddddddd), ja niiden on läpäistävä Luhn-testi.

- **[Malli neule:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Erittäin monimutkainen ja vankka malli, joka havaitsee eri puolilta maailmaa perä isin olevat kortit, mukaan lukien Visa, MasterCard, Discover Card, JCB, American Express, lahja kortit ja Diner-kortit.

- **[Tarkistus summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Kyllä, Luhn-tarkistus summa

- **[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP-käytännöllä on 85% varma, että se havaitsee tämän tyyppisiä tietoja, jos se on 300-merkin lähellä:

  - Funktio Func_credit_card löytää kaavaa vastaavaa sisältöä.

  - Jokin seuraavista on tosi:

  - Keyword_cc_verification avain sana löytyy.

  - Keyword_cc_name avain sana löytyy

  - Funktio Func_expiration_date löytää päivä määrän oikeassa päivämäärä muodossa.

  - Tarkistus summa kulkee

    Esimerkiksi seuraava esimerkki käynnistäisi DLP-luotto kortin numero käytäntöä:

  - Visa: 4485 3647 3952 7352
  
  - Vanhentuu: 2/2009

Lisä tietoja sisällöstä, jota tarvitaan **luotto kortin numeron** havaitsemisesta, on tämän artikkelin seuraavassa osiossa: [mitä luottamukselliset tieto tyypit näyttävät luotto kortti](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number) numeroksi
  
Jos käytät erilaista sisäistä arkaluonteista tieto tyyppiä, Katso lisä tietoja muista tieto tyypeistä, jotka ovat tarpeen: [mitä luottamukselliset tieto tyypit](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) etsivät
  