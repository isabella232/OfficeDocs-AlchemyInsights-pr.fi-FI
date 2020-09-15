---
title: DLP-sääntö USA:N pankki tilin numerolle ei toimi
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679293"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-ongelmat USA:N pankki tili numeroissa

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP-ongelmat USA:N pankki tili numeroissa**

Onko sinulla ongelmia **tietojen menetyksen estämisen (DLP)** kanssa, joka ei toimi **Yhdysvaltojen pankki tilin numeron** sisältävässä sisällössä, kun O365-palvelussa käytetään DLP-arkaluonteista tieto tyyppiä? Jos näin on, varmista, että sisältö sisältää tarvittavat tiedot siitä, mitä DLP-käytäntöä etsitään, kun se on laskettu.
  
Esimerkiksi **Yhdysvaltain pankki tilin numero** -käytännölle, jonka luotettavuus taso on 85%, lasketaan seuraavat tiedot ja ne on havaitava, jotta sääntö käynnistetään:
  
- **[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17-numerot

- **[Malli:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 peräkkäistä numeroa.

- **[Tarkistus summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, tarkistus summaa ei ole

- **[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP-käytännöllä on 75% varma, että se havaitsee tämän tyyppisiä tietoja, jos se on 300-merkin lähellä:

  - Säännöllinen lauseke Regex_usa_bank_account_number löytää kaavaa vastaavaa sisältöä.

  - Keyword_usa_Bank_Account avain sana löytyy.

    Esimerkiksi seuraava esimerkki käynnistäisi **USA:n pankki tilin numero** käytäntöä: tarkistetaan tiliä 78344011

Lisä tietoja siitä, mitä tarvitaan **USA:n pankki tilin numeron** havaitsemisesta sisältöä varten, on tämän artikkelin seuraavassa osiossa: [mitä luottamukselliset tieto tyypit näyttävät USA:n pankki tili numerolle](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) ?
  
Jos käytät erilaista sisäistä arkaluonteista tieto tyyppiä, Katso lisä tietoja muista tieto tyypeistä, jotka ovat tarpeen: [mitä luottamukselliset tieto tyypit](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) etsivät
  