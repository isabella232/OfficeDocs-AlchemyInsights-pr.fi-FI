---
title: Ulkoisten käyttäjien kanssa ei toimi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 700e6d24e49cf11bf91780895f5a796cc1d8349d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753423"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>SharePoint-sisällön jakaminen ulkoisten käyttäjien ongelmien korjaaminen

Varmista, että ulkoinen jakaminen on otettu käyttöön organisaatiossa:
  
1. Siirry [palvelut &amp; apuohjelmia Microsoft 365 admin keskellä sivun](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), ja valitse **sivustot**.
    
2. Varmista, että asetus on poistettu ”käytössä”. Jos ”vain olemassa olevat Ulkoiset käyttäjät” on valittuna, varmista, että ulkoisen käyttäjän tiedot on lueteltu Microsoft 365 admin Centerissä.
    
Varmista, että ulkoinen jakamisen pois sivuston. Perinteinen sivustokokoelman:
  
1. Valitse **sivustokokoelmat**classic SharePoint-hallintakeskukseen vasemmanpuoleisessa ruudussa.
    
2. Valitse sivusto tai sivustoja ja valitse valintanauhan **jakaminen**.
    
Ryhmäsivusto, joka kuuluu Office 365-ryhmään tai Viestimissivusto:
  
- Tällaisten sivusto on sama jakamisen määrittäminen organisaation laajuisten asetusten paitsi koko organisaation-asetuksen avulla, jakaa tiedostoja, linkkejä, jotka eivät edellytä sisään. Tässä tapauksessa sivustot sallivat uusien ja olemassa olevien ulkoisten käyttäjille, jotka kirjautua sisään jakaminen. Voit muuttaa asetusta tietyissä sivustoissa, käyttämällä uuden SharePoint-hallintakeskukseen (esikatselu)- tai PowerShell. [Lue lisää](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Kaikki sivuston ulkoinen jakaminen asetus voi olla rajoittavampi kuin organisaation laajuinen asetus, mutta ei kuitenkaan enempää kuin organisaation laajuinen asetus sallivien. 
  

