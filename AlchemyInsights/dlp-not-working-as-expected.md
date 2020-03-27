---
title: DLP ei toimi odotetusti
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977435"
---
# <a name="dlp-not-working-as-expected"></a>DLP ei toimi odotetusti

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat edelleen erittäin saatavilla – lisätietoja on [SharePoint Onlinen tilapäisissä ominaisuusoikaisuissa.](https://aka.ms/ODSPAdjustments)

 **DLP:n määrittäminen**

Onko Office 365:n **DLP(Data Loss Prevention)** -ongelma, joka ei toimi odotetulla tavalla? Jos näin on, varmista, että **DLP-käytäntö** on määritetty oikein ja että tiedot sisältävät sen, mitä **DLP-käytäntö** etsii, kun niitä arvioidaan.
  
DLP-käytäntöjen avulla voit tunnistaa ja suojata organisaation arkaluonteisia tietoja. Voit määrittää DLP-käytännöt [tässä .](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)
  
 **Mitä DLP-käytännöt etsivät**
  
Kun käytät **sisäisiä arkaluonteisia tietotyyppejä** Office 365:n suojaus- ja yhteensopivuuskeskuksessa, DLP-käytännöt etsivät tiettyjä malleja ja elementtejä, kun havaitset nämä arkaluonteiset tyypit.
  
- **Sisäiset arkaluonteiset tietotyypit**

    Lisätietoja sisäisistä arkaluonteisista tyypeistä ja siitä, mitä DLP-käytäntö etsii herkän tyypin havaitsemisessa, on kohdassa: [Mitä arkaluonteisia tietotyyppejä etsitään](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Mukautetut arkaluonteiset tietotyypit**

    Jos yrität luoda mukautettuja arkaluonteisia tietotyyppejä, saat lisätietoja mukautetun arkaluonteisen tyypin luomisesta seuraavasta artikkelista: [Mukautetun arkaluonteisen tietotyypin luominen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**DLP-käytännön testaaminen**

Jos haluat testata tietoja valmiilla tai mukautetulla arkaluonteisella tietotyypillä, käytä **Luokitusten** > **arkaluonteiset tietotyypit**-kohdan **Testaa tyyppi** -vaihtoehtoa. Lisätietoja on kohdassa [Mukautettujen arkaluonteisten tietotyyppien testaaminen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Raportit**
  
- Saat arkaluonteisten tietojen kävijätietoja [DLP-raporttien avulla.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Katso tapahtuman tarkat tiedot [tapahtumaraportin](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)avulla .
