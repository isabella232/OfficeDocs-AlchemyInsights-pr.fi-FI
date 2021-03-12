---
title: DLP ei toimi odotetulla tavalla
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707807"
---
# <a name="dlp-not-working-as-expected"></a>DLP ei toimi odotetulla tavalla

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

 **DLP:n määrittäminen**

Onko Office 365:n tietojen menetyksen estämisessä **(DLP)** ongelmia, jotka eivät toimi odotetulla tavalla? Jos on, varmista, että **DLP-käytäntö** on määritetty oikein ja että tietosi sisältävät sen, mitä **DLP-käytäntö** etsii, kun sitä arvioidaan.
  
DLP-käytännöt mahdollistavat luottamuksellisten tietojen tunnistamisen ja suojaamisen organisaatiossasi. Jos haluat määrittää DLP-käytäntöjä, käytä näitä [tietoja.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Mitä DLP-käytännöt näyttävät**
  
Kun tietoturva- ja yhteensopivuuskeskuksissa käytetään sisäänrakennettuja luottamuksellisia tietotyyppejä, **DLP-käytännöt** etsivät tiettyjä kaavoja ja elementtejä tunnistaessaan näitä luottamuksellisia tyyppejä.
  
- **Sisäänrakennettu luottamuksellisten tietojen tyypit**

    Tietoja valmiista luottamuksellisista tyypeistä ja siitä, mitä DLP-käytäntö etsii tunnistaessaan Luottamukselliset-tyypin, on seuraavassa kohdassa: Mitä luottamukselliset tietotyypit [etsivät.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Mukautetut luottamukselliset tietotyypit**

    Jos yrität luoda mukautettuja luottamuksellisia tietotyyppejä, saat seuraavan artikkelin avulla lisätietoja mukautetun luottamuksellisen tietotyypin luosta: Mukautetun [luottamuksellisen tietotyypin luominen.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**DLP-käytännön testaaminen**

Voit testata tietoja valmiilla tai mukautetuilla luottamuksellisilla  tietotyypeillä Käyttämällä Testityyppi-vaihtoehtoa Luokitukset   >  **luottamukselliset tietotyypit -kohdassa.** Lisätietoja on kohdassa Mukautettujen [luottamuksellisten tietotyyppien testaaminen.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Raportit**
  
- DLP-raporttien avulla saat [luottamuksellisia tietoja.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Voit tarkastella tapahtuman yksityiskohtaisia tietoja [tapahtumaraportin avulla.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
