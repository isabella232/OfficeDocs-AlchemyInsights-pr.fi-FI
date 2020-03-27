---
title: DLP sääntö YHDYSVALTAIN / UK Passport Number ei toimi
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
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977103"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Ongelmia DLP - USA / Iso-Britannia passin numerot

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat edelleen erittäin saatavilla – lisätietoja on [SharePoint Onlinen tilapäisissä ominaisuusoikaisuissa.](https://aka.ms/ODSPAdjustments)

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
  