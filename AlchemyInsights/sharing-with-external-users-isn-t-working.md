---
title: Jakaminen ulkopuolisten käyttäjien kanssa ei toimi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691572"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>SharePoint-sisällön jakamiseen ulkoisiin käyttäjiin liittyvien ongelmien korjaaminen

Varmista, että ulkoinen jakaminen on otettu käyttöön organisaatiossa:
  
1. Siirry [ &amp; Microsoft 365-hallinta keskuksen palvelut-apuohjelmat-sivulle](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ja valitse **sivustot**.
    
2. Varmista, että asetus on käytössä. Jos vain olemassa olevat ulkoiset käyttäjät-kohta on valittuna, varmista, että ulkoinen käyttäjä on lueteltu Microsoft 365-hallinta keskuksessa.
    
Varmista, että ulkoinen jakaminen on otettu käyttöön sivustossa. Perinteinen sivustokokoelma:
  
1. Valitse uusi SharePoint-hallinta keskus-kohdan vasemmanpuoleisessa ruudussa **sivustot**.
    
2. Valitse sivusto tai sivustot ja valitse sitten valinta nauhassa **jakaminen**.
    
Ryhmäsivusto, joka kuuluu Microsoft 365-ryhmään tai viestintäsivustoon:
  
- Näillä uusilla sivustotyypeillä on sama jakamis asetus koko organisaation leveää asetusta varten, ellei koko organisaation laajuinen asetus salli tiedostojen jakamista linkeillä, jotka eivät edellytä sisäänkirjautumista. Tässä tapa uksessa sivustot sallivat jakamisen uusilla ja olemassa oleville ulkoisille käyttäjille, jotka kirjautuvat sisään. Jos haluat muuttaa tiettyjen sivuston asetuksia, käytä uutta SharePoint-hallinta keskusta tai PowerShelliä. [Lisätietoja](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Minkä tahansa sivuston ulkoinen jakamis asetus voi olla organisaatiolaajuista asetusta rajoittavampi, mutta ei koko organisaatiota leveää asetusta suurempi. 
  

