---
title: Ehdollisen käyttöoikeuden valvonta
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287507"
---
# <a name="monitoring-conditional-access"></a>Ehdollisen käyttöoikeuden valvonta

Kohdennetut ja ehdollisen käyttöoikeuden käyttäjät saavat sähköposti-ilmoitus, jos ne eivät täytä vaatimuksia organisaation. käyttö. Ratkaisemiseksi, suosittelemme vähintään yksi seuraavista toimista:
  
- Laite on rekisteröitynyt, siirry yritysportaalin yritys app ja varmista, että käyttäjä antaa neuvoja toteutuvan tulee yrityksen portaaliin. Jos näin ei ole, käyttäjä pitäisi rekisteröidä laitteen.
    
- Siirry portaalin Azure **Intune \> laitteen yhteensopivuuden**. Valitse **näytön** **laitteen vaatimustenmukaisuus**. Voit tarkastella laitteen yhteensopivuus raportin, varmista, että laitteen käyttäjän on merkitty niin paljon. 
    
- Siirry portaalin Azure **Intune \> laitteen yhteensopivuuden**. Valitse **Hallitse** **käytäntöjä**. Yhteensopivuuskäytäntöihin luettelossa Tarkista, että profiili on määritetty käyttäjän laitteeseen. Jos ei ole profiilin on määritetty, Intune ei voi Vahvista laitteen yhteensopivuus tila. 
    
- Muokkaa käyttäjän ehdollisen käyttöoikeuden varauksen.
    
1. Siirry portaalin Azure **Intune \> ehdollisen käyttöoikeuden \> käytännöt**
    
2. Valitse käytäntö luettelosta
    
3. Valitse **käyttäjät ja ryhmät**
    
4. Joku on tiettyjä käytännön kohteeksi lisätä ne **luettelossa** . Sen varmistamiseksi, että henkilö on pois käytännöstä, lisää ne **pois** luettelosta. 
    
Lue lisää: [miten näyttö ehdollisen käyttöoikeuden laitteet](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)
  

