---
title: Ehdollisen käytön valvonta
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713715"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Ehdollisen käytön valvonta Exchangessa

Ehdolliseen käyttöön kohdistetut käyttäjät saavat sähköposti-ilmoituksen, jos he eivät täytä organisaatiosi käyttövaatimuksia. Ratkaisua suositellaan vähintään yhtä seuraavista ratkaisuista:
  
- Jos laitteen oletetaan olevan rekisteröitynyt, kehota käyttäjää menemään Yritysportaali-sovellukseen ja varmistamaan, että se näkyy yritysportaalissa. Jos näin ei ole, käyttäjän on rekisteröitava laite.
    
- Siirry Azure-portaalissa **Kohtaan \> Intune Device compliance**. Valitse **Näyttö-kohdassa** **Laitteen yhteensopivuus**. Tarkista laitteen yhteensopivuusraportista, että käyttäjän laite on merkitty yhteensopivaksi. 
    
- Siirry Azure-portaalissa **Kohtaan \> Intune Device compliance**. Valitse **Hallinta**-kohdassa **Käytännöt**. Varmista yhteensopivuuskäytäntöjen luettelosta, että käyttäjän laitteelle on määritetty profiili. Jos profiilia ei ole määritetty, Intune ei voi vahvistaa laitteen vaatimustenmukaisuuden tilaa. 
    
- Muokkaa käyttäjän ehdollisen käytön määritystä.
    
1. Siirry Azure-portaalissa **Intune-ehdollisen \> käytön \> käytäntöihin**
    
2. Käytännön valitseminen luettelosta
    
3. Valitse **Käyttäjät ja ryhmät.**
    
4. Jos haluat kohdistaa tietyn käytännön johonkin, lisää hänet **Sisällytä-luetteloon.** Voit varmistaa, että henkilö jätetään pois käytännöstä, lisäämällä hänet **Pois-luetteloon.** 
    
Lue lisää: [Ehdollisen käytön laitteiden valvonta](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

