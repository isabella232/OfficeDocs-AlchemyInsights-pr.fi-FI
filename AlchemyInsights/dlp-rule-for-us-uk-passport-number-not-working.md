---
title: DLP-sääntö YHDYSVALTALLE/UK:N Passport-numerolle ei toimi
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679221"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP-US/UK Passport-numeroiden ongelmat

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP-ongelmat USA:N/Yhdistyneen kuningas kunnan Passport-numeroissa**

Onko sinulla ongelmia **tietojen menetyksen estämisen (DLP)** kanssa, joka ei toimi **Yhdysvalloissa ja Yhdistyneessä kuningas kunnassa olevan Passport-numeron** sisältävässä sisällössä, kun O365-palvelussa käytetään DLP-arkaluonteista tieto tyyppiä? Jos näin on, varmista, että sisältö sisältää tarvittavat tiedot siitä, mitä DLP-käytäntöä etsitään, kun se on laskettu.
  
Esimerkiksi **Yhdysvaltain ja Yhdistyneen kuningas kunnan passin numero** käytännölle, jonka luotettavuus taso on 75%, lasketaan seuraavat ehdot, jotka on määritettävä, jotta sääntö käynnistetään
  
- **[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Yhdeksän numeroa

- **[Malli neule:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Yhdeksän peräkkäistä numeroa

- **[Tarkistus summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, tarkistus summaa ei ole

- **[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP-käytännöllä on 75% varma, että se havaitsee tämän tyyppisiä tietoja, jos se on 300-merkin lähellä:

  - Funktio Func_usa_uk_passport löytää kaavaa vastaavaa sisältöä.

  - Keyword_passport avain sana löytyy.

    Esimerkiksi seuraava esimerkki käynnistäisi **Yhdysvaltojen ja Yhdistyneen kuningas kunnan passin numero** käytäntöä: Yhdysvaltain passin numero 123456789

Lisä tietoja käyttäjän ja Yhdistyneen kuningas kunnan passin numeron havaitsemisesta sisältöä varten on tämän artikkelin seuraavassa osiossa: [mitä luottamukselliset tieto tyypit näyttävät Yhdysvaltojen ja Yhdistyneen kuningas kunnan Passport-numerolle](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Jos käytät erilaista sisäistä arkaluonteista tieto tyyppiä, Katso lisä tietoja muista tieto tyypeistä, jotka ovat tarpeen: [mitä luottamukselliset tieto tyypit](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) etsivät
  