---
title: DLP saattaa tarvita mukautetun tyypin
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704486"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP saattaa tarvita mukautetun tyypin

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP voi vaatia mukautetun tietotyypin**

DLP (Data Loss Prevention) -käytännön avulla voit tunnistaa ja suojata organisaation arkaluonteisia tietoja. Joissakin tilanteissa sinun on ehkä luotava oma **mukautettu** tietotyyppi organisaatiosi tietojen suojaamiseksi.

Organisaatiosi on esimerkiksi ehkä tunnistettava ja suojattava työntekijätunnusten tai muiden tietojen tunnistamisessa organisaatiosi tietyssä muodossa. Jos näin on, katso lisätietoja seuraavista artikkeleista.
  
 **Sisäisen arkaluonteisen tietotyypin mukauttaminen**
  
Jos sisäänrakennettu arkaluonteinen tietotyyppi vastaisi tarpeitasi muutamalla sävyllä, voit [mukauttaa sisäisen arkaluonteisen tietotyypin](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Voit esimerkiksi lisätä tai poistaa avainsanoja tai lisätä tai poistaa todisteita, kuten päivämäärän tai osoitteen.
  
 **Mukautetun arkaluonteisen tietotyypin luominen**
  
Jos sinun on kuitenkin tunnistettava ja suojattava erityyppiset arkaluonteiset tiedot kokonaan, voit [luoda mukautetun arkaluonteisen tietotyypin](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) Suojaus& Yhteensopivuuskeskuksen käyttöliittymässä.
  
**Mukautetun arkaluonteisen tietotyypin luominen Tietoturva& Compliance Center PowerShellissä**

Jos käyttöliittymässä ei ole kaikkia tarvitsemiasi asetuksia, voit [luoda mukautetun arkaluonteisen tietotyypin Tietoturva-& Yhteensopivuuskeskus PowerShellissä](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Aloittamalla XML-tiedostosta voit käyttää kaikkia käytettävissä olevia vaihtoehtoja.
