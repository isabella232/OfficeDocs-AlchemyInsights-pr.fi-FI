---
title: DLP ei toimi oikein
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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679690"
---
# <a name="dlp-not-working-as-expected"></a>DLP ei toimi oikein

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

 **DLP:N määrittäminen**

Onko sinulla ongelmia **tietojen menetyksen estämisen (DLP)** kanssa Office 365 ei toimi oikein? Jos näin on, varmista, että **DLP-käytäntönne** on määritetty oikein ja että tiedot sisältävät sen, mitä **DLP-käytäntöä** etsitään, kun sitä arvioidaan.
  
DLP-käytäntöjen avulla voit tunnistaa ja suojata organisaation luottamukselliset tiedot. Jos haluat määrittää DLP-käytännöt, käytä [näitä tietoja.](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)
  
 **Mitä DLP-käytännöt etsivät**
  
Kun käytät tieto turva-ja yhteensopivuus keskuksissa olevia **sisäisiä tieto tyyppejä** , DLP-käytännöt etsivät tiettyjä kuvioita ja tietoja tunnistamalla nämä arkaluonteiset tyypit.
  
- **Sisäiset luottamukselliset tieto tyypit**

    Lisä tietoja sisäisistä luottamuksellisista tyypeistä ja siitä, mitä DLP-käytäntöä etsitään arkaluonteisen tyypin havaitsemiseksi, on kohdassa: [mitä arkaluonteiset tieto tyypit](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)etsivät.

- **Mukautetut luottamukselliset tieto tyypit**

    Jos yrität luoda mukautettuja tieto tyyppejä, käytä seuraavaa artikkelin tietoja mukautetun luottamuksellisen tyypin luomisesta: [mukautetun tieto tyypin](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)luominen.

**DLP-käytäntöjen testaaminen**

Jos haluat testata tietoja sisäisellä tai mukautetulla arkaluonteisella tieto tyypillä, käytä **testi tyyppi** -vaihto ehtoa **luokittelujen**  >  **luottamukselliset tieto tyypit**-kohdassa. Lisä tietoja on kohdassa [mukautettujen luottamuksellisten tieto tyyppien testaaminen](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Raportit**
  
- Nouda luottamukselliset tietojen tiedot [DLP-raporttien avulla.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Tarkastele tapahtuman yksityiskohtaisia tietoja [häiriö raportin](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)avulla.
