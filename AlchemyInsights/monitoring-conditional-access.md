---
title: Ehdollisen käyttöoikeuden valvonta
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538739"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Ehdollisen käyttöoikeuden Exchange seuranta

Kohdennetut ja ehdollisen käyttöoikeuden käyttäjät saavat sähköposti-ilmoitus, jos ne eivät täytä vaatimuksia organisaation. käyttö. Ratkaisemiseksi, suosittelemme vähintään yksi seuraavista toimista:
  
- Laite on rekisteröitynyt, siirry yritysportaalin yritys app ja varmista, että käyttäjä antaa neuvoja toteutuvan tulee yrityksen portaaliin. Jos näin ei ole, käyttäjä pitäisi rekisteröidä laitteen.
    
- Siirry portaalin Azure **Intune \> laitteen yhteensopivuuden**. Valitse **näytön** **laitteen vaatimustenmukaisuus**. Voit tarkastella laitteen yhteensopivuus raportin, varmista, että laitteen käyttäjän on merkitty niin paljon. 
    
- Siirry portaalin Azure **Intune \> laitteen yhteensopivuuden**. Valitse **Hallitse** **käytäntöjä**. Yhteensopivuuskäytäntöihin luettelossa Tarkista, että profiili on määritetty käyttäjän laitteeseen. Jos ei ole profiilin on määritetty, Intune ei voi Vahvista laitteen yhteensopivuus tila. 
    
- Muokkaa käyttäjän ehdollisen käyttöoikeuden varauksen.
    
1. Siirry portaalin Azure **Intune \> ehdollisen käyttöoikeuden \> käytännöt**
    
2. Valitse käytäntö luettelosta
    
3. Valitse **käyttäjät ja ryhmät**
    
4. Joku on tiettyjä käytännön kohteeksi lisätä ne **luettelossa** . Sen varmistamiseksi, että henkilö on pois käytännöstä, lisää ne **pois** luettelosta. 
    
Lue lisää: [miten näyttö ehdollisen käyttöoikeuden laitteet](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

