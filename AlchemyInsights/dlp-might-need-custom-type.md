---
title: DLP voi tarvita mukautettua tyyppiä
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030791"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP voi tarvita mukautettua tyyppiä

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP saattaa edellyttää mukautettua tietotyyppiä**

Tietojen menetyksen estämisen (DLP) käytännön avulla voit tunnistaa ja suojata luottamuksellisia tietoja organisaatiossasi. Joissakin tilanteissa sinun on ehkä luotava  oma mukautettu luottamuksellisten tietojen tyyppi organisaatiosi tietojen suojaamiseksi.

Organisaatiosi on esimerkiksi ehkä tunnistettava ja suojattava työntekijöiden tunnukset tai muut tiedot tietyssä organisaatiosi muodossa. Jos näin on, katso lisätietoja seuraavista artikkeleista.
  
 **Valmiin luottamuksellisen tietotyypin mukauttaminen**
  
Jos sisäinen luottamuksellisten tietojen tyyppi vastaa tarpeitasi muutamalla hienosäädöllä, voit mukauttaa sisäistä [luottamuksellista tietotyyppiä](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Voit esimerkiksi lisätä tai poistaa avainsanoja tai lisätä tai poistaa tukiaineistoa, kuten päivämäärän tai osoitteen.
  
 **Mukautetun luottamuksellisen tietotyypin luominen**
  
Jos sinun on kuitenkin tunnistettava ja suojattava erityyppisiä [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) luottamuksellisia tietoja, voit luoda mukautetun luottamuksellisen tietotyypin Tietoturva- ja & -keskuksen käyttöliittymässä.
  
**Mukautetun luottamuksellisen tietotyypin luominen & yhteensopivuuskeskuksen PowerShellissä**

Jos käyttöliittymässä ei ole kaikkia tarvitsemiasi asetuksia, voit luoda mukautetun luottamuksellisen tietotyypin Tietoturva- & [PowerShellissä.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) Kun aloitat XML-tiedostosta, voit käyttää kaikkia käytettävissä olevia vaihtoehtoja.
