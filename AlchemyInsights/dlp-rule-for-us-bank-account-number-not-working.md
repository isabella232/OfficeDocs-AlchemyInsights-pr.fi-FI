---
title: Yhdysvaltain pankkitilinumeron DLP-sääntö ei toimi
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
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005015"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-ongelmat YHDYSVALTOJEN pankkitilinumeroissa

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP-ongelmat YHDYSVALTOJEN pankkitilinumeroissa**

Onko sinulla ongelmia tietojen menetyksen estämisen **(DLP)** kanssa, joka ei toimi Yhdysvaltojen pankkitilinumeron sisältävän sisällön kanssa, kun käytät DLP-luottamuksellista tietotyyppiä O365:ssä?  Jos näin on, varmista, että sisältösi sisältää tarvittavat tiedot siitä, mitä DLP-käytäntö etsii, kun sitä arvioidaan.
  
Jos esimerkiksi US **Bank Account Number** -käytäntö on määritetty 85 prosentin luottamustasolla, seuraavat tiedot arvioidaan, ja ne on tunnistettava, jotta sääntö voi käynnistää:
  
- **[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8–17 numeroa

- **[Kuvio:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8–17 peräkkäistä numeroa.

- **[Tarkistussumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, tarkistussummaa ei ole

- **[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP-käytäntö on 75-prosenttisesti varma siitä, että se on havainnut luottamuksellisia tietoja, jos 300 merkin sisällä:

  - Säännöllinen lauseke Regex_usa_bank_account_number löytää kaavaa vastaavaa sisältöä

  - Hakusana kohteesta Keyword_usa_Bank_Account löytyy.

    Esimerkiksi seuraava esimerkki käynnisti US Bank **Account Number** -käytännön: Checking Account 78344011

Lisätietoja siitä, mitä sisällössäsi **tunnistettavan YHDYSVALTOJEN** pankkitilinumeron vaatimukset ovat, on tämän artikkelin seuraavassa osiossa: Mitä luottamukselliset tietotyypit näyttävät US Bank Account Number [-tunnuksella?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Jos käytössäsi on erilainen sisäinen luottamuksellisten tietojen tyyppi, katso seuraavasta artikkelista tietoja siitä, mitä muuntyyppiset tiedot tarvitaan: Mitä Luottamukselliset tietotyypit [-kohta näyttää](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  