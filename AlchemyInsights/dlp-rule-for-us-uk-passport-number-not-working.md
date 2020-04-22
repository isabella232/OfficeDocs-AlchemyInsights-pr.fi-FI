---
title: DLP sääntö YHDYSVALTAIN / UK Passport Number ei toimi
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
ms.openlocfilehash: 9d9615eccd1e245bf4ca32742bfc64321dd7a8cf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714983"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Ongelmia DLP - USA / Iso-Britannia passin numerot

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP-ongelmat Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumeroiden kanssa**

Onko sinulla ongelmia **Data Loss Prevention (DLP)** ei toimi sisältöä, joka sisältää Yhdysvaltain ja Yhdistyneen **kuningaskunnan passin numero,** kun käytät DLP arkaluonteisia tietoja tyyppi O365? Jos näin on, varmista, että sisältösi sisältää tarvittavat tiedot siitä, mitä DLP-käytäntö etsii, kun sitä arvioidaan.
  
Esimerkiksi Yhdysvaltain **ja Yhdistyneen kuningaskunnan passin numerokäytännössä,** jonka luotettavuustaso on 75 %, arvioidaan seuraavat tiedot, ja ne on tunnistettava, jotta sääntö voi käynnistää
  
- **[Muoto:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Yhdeksän numeroa

- **[Mallineule:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Yhdeksän peräkkäistä numeroa

- **[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole Checksumia.

- **[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP-käytäntö on 75 %: n varma siitä, että se on havainnut tämäntyyppisiä arkaluonteisia tietoja, jos 300 merkin etäisyydellä:

  - Toiminto Func_usa_uk_passport etsii kaavaa vastaavaa sisältöä.

  - Keyword_passport avainsana löytyy.

    Esimerkiksi seuraava esimerkki käynnistäisi **Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumerokäytännön:** Yhdysvaltain passin numero 123456789

Lisätietoja siitä, mitä tarvitaan, jotta Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumero voidaan havaita sisällöllesi, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät YHDYSVALTAIN ja Yhdistyneen kuningaskunnan passin numeroa](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Toisen sisäisen arkaluonteisen tietotyypin avulla on seuraavassa artikkelissa tietoja siitä, mitä muille tyypeille tarvitaan: [Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  