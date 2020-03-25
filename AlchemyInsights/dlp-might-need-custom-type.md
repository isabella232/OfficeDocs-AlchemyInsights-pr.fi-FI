---
title: DLP saattaa tarvita mukautetun tyypin
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932655"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP saattaa tarvita mukautetun tyypin

**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan. Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut. Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.

Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan. Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina. Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.

**DLP voi vaatia mukautetun tietotyypin**

DLP (Data Loss Prevention) -käytännön avulla voit tunnistaa ja suojata organisaation arkaluonteisia tietoja. Joissakin tilanteissa sinun on ehkä luotava oma **mukautettu** tietotyyppi organisaatiosi tietojen suojaamiseksi.

Organisaatiosi on esimerkiksi ehkä tunnistettava ja suojattava työntekijätunnusten tai muiden tietojen tunnistamisessa organisaatiosi tietyssä muodossa. Jos näin on, katso lisätietoja seuraavista artikkeleista.
  
 **Sisäisen arkaluonteisen tietotyypin mukauttaminen**
  
Jos sisäänrakennettu arkaluonteinen tietotyyppi vastaisi tarpeitasi muutamalla sävyllä, voit [mukauttaa sisäisen arkaluonteisen tietotyypin](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Voit esimerkiksi lisätä tai poistaa avainsanoja tai lisätä tai poistaa todisteita, kuten päivämäärän tai osoitteen.
  
 **Mukautetun arkaluonteisen tietotyypin luominen**
  
Jos sinun on kuitenkin tunnistettava ja suojattava erityyppiset arkaluonteiset tiedot kokonaan, voit [luoda mukautetun arkaluonteisen tietotyypin](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) Suojaus& Yhteensopivuuskeskuksen käyttöliittymässä.
  
**Mukautetun arkaluonteisen tietotyypin luominen Tietoturva& Compliance Center PowerShellissä**

Jos käyttöliittymässä ei ole kaikkia tarvitsemiasi asetuksia, voit [luoda mukautetun arkaluonteisen tietotyypin Tietoturva-& Yhteensopivuuskeskus PowerShellissä](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Aloittamalla XML-tiedostosta voit käyttää kaikkia käytettävissä olevia vaihtoehtoja.
