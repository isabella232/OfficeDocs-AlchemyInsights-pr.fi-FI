---
title: Ehdollisen käytön valvominen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702900"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Ehdollisen Exchange-yhteyden valvonta

Ehdolliseen käyttöön kohdistetut käyttäjät saavat ilmoitus Sähkö posti viestin, jos he eivät täytä organisaatiosi käyttö oikeus vaatimuksia. Ratkaisu on suositeltava vähintään yksi seuraavista ratkaisuista:
  
- Jos laitteen oletetaan olevan rekisteröity, kehota käyttäjää siirtymään yritys portaali-sovellukseen ja vahvistamaan, että se näkyy yritys portaalissa. Jos näin ei tapahdu, käyttäjän on rekisteröitävä laite.
    
- Valitse Azure-portaalissa **Intune- \> laitteen yhteensopivuus**. Valitse **näyttö** -kohdassa **laitteen yhteensopivuus**. Tarkastele laitteesi yhteensopivuus raporttia varmistaaksesi, että käyttäjän laite on merkitty yhteensopivaksi. 
    
- Valitse Azure-portaalissa **Intune- \> laitteen yhteensopivuus**. Valitse **hallinta**-kohdassa **käytännöt**. Varmista yhteensopivuus käytäntöjen luettelosta, että profiili on määritetty käyttäjän laitteelle. Jos profiilia ei ole määritetty, Intune ei pysty vahvistamaan laitteen yhteensopivuus tilaa. 
    
- Muokkaa käyttäjän ehdollisen käytön määritystä.
    
1. Azure-portaalissa Siirry **Intune-sivuston \> ehdollisen käytön \> käytäntöihin**
    
2. Valitse käytännöstä luettelosta
    
3. Valitse **käyttäjät ja ryhmät**
    
4. Jos haluat kohdentaa tiettyyn käytäntöön jollekulle, lisää ne **Sisällytä** -luetteloon. Jos haluat varmistaa, että henkilö jätetään pois käytännöstä, Lisää hänet **Jätä pois** -luetteloon. 
    
Lue lisää: [ehdollisen pääsyn valvonta laitteiden valvominen](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

