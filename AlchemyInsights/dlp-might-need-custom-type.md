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
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507511"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP saattaa tarvita mukautetun tyypin

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP saattaa edellyttää mukautettua tietotyyppiä**

DLP (Data Loss Prevention) -käytännön avulla voit tunnistaa ja suojata organisaation arkaluonteiset tiedot. Joissakin tilanteissa sinun on ehkä luotava oma **mukautettu** arkaluonteinen tietotyyppi, jotta voit suojata organisaatiosi tiedot.

Organisaatiosi on ehkä esimerkiksi tunnistettava ja suojattava työntekijätunnukset tai muut tiedot organisaatiollesi tietyssä muodossa. Jos näin on, katso lisätietoja seuraavista artikkeleista.
  
 **Valmiin arkaluonteisen tietotyypin mukauttaminen**
  
Jos sisäänrakennettu arkaluonteinen tietotyyppi vastaisi tarpeitasi muutamalla hienosäädöllä, voit [mukauttaa sisäänrakennettua arkaluonteista tietotyyppiä](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Voit esimerkiksi lisätä tai poistaa avainsanoja tai lisätä tai poistaa todisteita, kuten päivämäärän tai osoitteen.
  
 **Mukautetun arkaluonteisen tietotyypin luominen**
  
Jos sinun on kuitenkin tunnistettava ja suojattava erityyppiset arkaluonteiset tiedot kokonaan, voit [luoda mukautetun arkaluonteisen tietotyypin](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) Tietoturva-& Compliance Centerin käyttöliittymään.
  
**Mukautetun arkaluonteisen tietotyypin luominen Security & Compliance Center PowerShellissä**

Lopuksi, jos käyttöliittymässä ei ole kaikkia tarvitsemiasi asetuksia, voit [luoda mukautetun arkaluonteisen tietotyypin Security & Compliance Center PowerShell -toiminnolla.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) Aloittamalla XML-tiedostosta voit käyttää kaikkia käytettävissä olevia vaihtoehtoja.
