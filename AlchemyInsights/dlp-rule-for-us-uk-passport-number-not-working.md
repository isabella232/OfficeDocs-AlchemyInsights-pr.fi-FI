---
title: US/UK Passport -passin numero ei toimi DLP-sääntö
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507295"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Ongelmia DLP - USA / UK passin numerot

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP-ongelmat Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumeroiden kanssa**

Onko sinulla ongelmia, kun **käytät DLP-arkaluonteista** tietotyyppiä O365:ssä, **kun** käytät DLP-arkaluonteista tietotyyppiä O365:ssä? Jos näin on, varmista, että sisältö sisältää tarvittavat tiedot siitä, mitä DLP-käytäntö etsii, kun sitä arvioidaan.
  
Esimerkiksi Yhdysvaltain **ja Yhdistyneen kuningaskunnan passinumerokäytännössä,** jonka luotettavuustaso on 75 %, arvioidaan seuraavat tiedot ja ne on tunnistettava, jotta sääntö käynnistää
  
- **[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Yhdeksän numeroa

- **[Mallineule:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Yhdeksän peräkkäistä numeroa

- **[Tarkistussumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, tarkistussummaa ei ole.

- **[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP-käytäntö on 75% varma siitä, että se on havainnut tällaisia arkaluonteisia tietoja, jos 300 merkin läheisyydessä:

  - Funktio Func_usa_uk_passport etsii kuviota vastaavaa sisältöä.

  - Avainsana Keyword_passport löytyy.

    Esimerkiksi seuraava esimerkki käynnistäisi **Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumerokäytännön:** Yhdysvaltain passin numero 123456789

Lisätietoja siitä, mitä tarvitaan, jotta Yhdysvaltalaisen ja Yhdistyneen kuningaskunnan passinumero voidaan havaita sisällöllesi, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumeroa](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Jos käytät eri sisäänrakennettua arkaluonteista tietotyyppiä, lue seuraavassa artikkelissa tietoja siitä, mitä tarvitaan muuntyyppisille [tyypeille: Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  