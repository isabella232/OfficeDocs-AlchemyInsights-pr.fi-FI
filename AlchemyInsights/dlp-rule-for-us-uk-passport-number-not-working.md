---
title: Yhdysvaltain/Yhdistyneen kuningaskunnan passien numeron DLP-sääntö ei toimi
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004943"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Ongelmia DLP:n kanssa – Yhdysvaltain/Yhdistyneen kuningaskunnan passien numerot

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP-ongelmat Yhdysvaltain/Yhdistyneen kuningaskunnan passien numeroissa**

Onko sinulla ongelmia tietojen menetyksen estämisen **(DLP)** kanssa, joka ei toimi **Yhdysvaltain/Yhdistyneen** kuningaskunnan passinumeron sisältävän sisällön kanssa, kun käytät DLP-luottamuksellista tietotyyppiä O365:ssä? Jos näin on, varmista, että sisältösi sisältää tarvittavat tiedot siitä, mitä DLP-käytäntö etsii, kun sitä arvioidaan.
  
Jos esimerkiksi Yhdysvaltain/Yhdistyneen kuningaskunnan kansalaisten passien numerokäytäntö on määritetty 75 prosentin luottamustasolle, arvioidaan seuraavat seikat, ja ne on tunnistettava, jotta sääntö voi käynnistää 
  
- **[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Yhdeksän numeroa

- **[Kaava:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Yhdeksän peräkkäistä numeroa

- **[Tarkistussumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, tarkistussummaa ei ole

- **[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP-käytäntö on 75-prosenttisesti varma siitä, että se on havainnut luottamuksellisia tietoja, jos 300 merkin sisällä:

  - Funktio Func_usa_uk_passport löytää kaavaa vastaavaa sisältöä.

  - Hakusana kohteesta Keyword_passport löytyy.

    Esimerkiksi Yhdysvaltain/Yhdistyneen kuningaskunnan passien numerokäytäntö käynnisti seuraavan otoksen: Yhdysvaltain passien 123456789 

Lisätietoja siitä, mitä sisällössäsi tunnistettavan Yhdysvaltain/Yhdistyneen kuningaskunnan passien numeron on oltava, on tämän artikkelin seuraavassa [osiossa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) Mitä Yhdysvaltain/ Yhdistyneen kuningaskunnan passien numero luottamukselliset tietotyypit näyttävät?
  
Jos käytössäsi on erilainen sisäinen luottamuksellisten tietojen tyyppi, katso seuraavasta artikkelista tietoja siitä, mitä muuntyyppiset tiedot tarvitaan: Mitä Luottamukselliset tietotyypit [-kohta näyttää](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  