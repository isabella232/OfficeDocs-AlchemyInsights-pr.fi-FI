---
title: DLP-sääntö luottokortin numerolle ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507403"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-ongelmat luottokorttien numeroiden kanssa

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP-ongelmat luottokorttien numeroiden kanssa**

Onko sinulla ongelmia **tietojen menetyksen estämisessä (DLP)** ei toimi sisällössä, joka sisältää **luottokortin numeron,** kun käytät DLP-arkaluonteista tietotyyppiä O365:ssä? Jos näin on, varmista, että sisältö sisältää tarvittavat tiedot, jotta DLP-käytäntö käynnistetään, kun sitä arvioidaan. Esimerkiksi **luottokorttikäytännössä,** jonka luotettavuustaso on 85 %, arvioidaan seuraavat tiedot, jotka on tunnistettava, jotta sääntö käynnistyisi:
  
- **[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 numeroa, jotka voidaan muotoilla tai alustamatta (dddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd

- **[Mallineule:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Erittäin monimutkainen ja vankka kuvio, joka havaitsee kortteja kaikista tärkeimmistä tuotemerkeistä maailmanlaajuisesti, mukaan lukien Visa, MasterCard, Discover Card, JCB, American Express, lahjakortit ja diner-kortit.

- **[Tarkistussumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Kyllä, Luhnin tarkistussumma.

- **[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP-käytäntö on 85% varma siitä, että se on havainnut tällaisia arkaluonteisia tietoja, jos 300 merkin läheisyydessä:

  - Funktio, Func_credit_card etsii kuviota vastaavaa sisältöä.

  - Jokin seuraavista on totta:

  - Avainsana Keyword_cc_verification löytyy.

  - Avainsana Keyword_cc_name löytyy

  - Funktio, Func_expiration_date etsii päivämäärän oikeassa päivämäärämuodossa.

  - Tarkistussumma kulkee

    Esimerkiksi seuraava esimerkki käynnistäisi DLP-luottokortin numerokäytännön:

  - Viisumi: 4485 3647 3952 7352
  
  - Päättyy: 2/2009

Lisätietoja siitä, mitä tarvitaan, jotta **luottokorttinumero** voidaan havaita sisällöllesi, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät luottokorttia#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Jos käytät eri sisäänrakennettua arkaluonteista tietotyyppiä, lue seuraavassa artikkelissa tietoja siitä, mitä tarvitaan muuntyyppisille [tyypeille: Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  