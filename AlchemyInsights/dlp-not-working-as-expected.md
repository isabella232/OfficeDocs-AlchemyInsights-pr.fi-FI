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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932619"
---
# <a name="dlp-not-working-as-expected"></a>DLP ei toimi odotetusti

**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan. Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut. Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.

Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan. Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina. Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.

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
