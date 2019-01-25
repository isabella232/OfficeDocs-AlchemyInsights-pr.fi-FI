---
title: Ulkoisten käyttäjien kanssa ei toimi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29467542"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>SharePoint-sisällön jakaminen ulkoisten käyttäjien ongelmien korjaaminen

Varmista, että ulkoinen jakaminen on otettu käyttöön organisaatiossa:
  
1. Siirry [palvelut &amp; -apuohjelmat Office 365: n hallinnan keskellä sivun](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), ja valitse **sivustot**.
    
2. Varmista, että asetus on poistettu ”käytössä”. Jos ”vain olemassa olevat Ulkoiset käyttäjät” on valittuna, varmista, että ulkoinen käyttäjä on mainittu Office 365-hallintakeskukseen.
    
Varmista, että ulkoinen jakamisen pois sivuston. Perinteinen sivustokokoelman:
  
1. Valitse **sivustokokoelmat**classic SharePoint-hallintakeskukseen vasemmanpuoleisessa ruudussa.
    
2. Valitse sivusto tai sivustoja ja valitse valintanauhan **jakaminen**.
    
Ryhmäsivusto, joka kuuluu Office 365-ryhmään tai Viestimissivusto:
  
- Tällaisten sivusto on sama jakamisen määrittäminen organisaation laajuisten asetusten paitsi koko organisaation-asetuksen avulla, jakaa tiedostoja, linkkejä, jotka eivät edellytä sisään. Tässä tapauksessa sivustot sallivat uusien ja olemassa olevien ulkoisten käyttäjille, jotka kirjautua sisään jakaminen. Voit muuttaa asetusta tietyissä sivustoissa, käyttämällä uuden SharePoint-hallintakeskukseen (esikatselu)- tai PowerShell. [Lue lisää](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Kaikki sivuston ulkoinen jakaminen asetus voi olla rajoittavampi kuin organisaation laajuinen asetus, mutta ei kuitenkaan enempää kuin organisaation laajuinen asetus sallivien. 
  

