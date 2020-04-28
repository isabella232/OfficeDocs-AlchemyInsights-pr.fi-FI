---
title: Jakaminen ulkoisten käyttäjien kanssa ei toimi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912999"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>SharePoint-sisällön jakamiseen ulkoisten käyttäjien kanssa liittyvien ongelmien korjaaminen

Varmista, että ulkoinen jakaminen on käytössä organisaatiossasi:
  
1. Siirry [Microsoft &amp; 365 -hallintakeskuksen Palvelut-apuohjelmat -sivulle](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ja valitse **Sivustot**.
    
2. Varmista, että asetuksen asetuksena on Käytössä. Jos "Vain nykyiset ulkoiset käyttäjät" on valittuna, varmista, että ulkoinen käyttäjä näkyy Microsoft 365 -hallintakeskuksessa.
    
Varmista, että ulkoinen jakaminen on käytössä sivustossa. Klassista sivustokokoelmaa varten:
  
1. Valitse uuden SharePoint-hallintakeskuksen vasemmanpuoleisesta ruudusta **Sivustot**.
    
2. Valitse sivusto tai sivustot ja valitse valintanauhasta **Jakaminen**.
    
Ryhmäsivustossa, joka kuuluu Microsoft 365 -ryhmään, tai viestintäsivustoon:
  
- Näillä uusilla sivustotyypeillä on sama jakamisasetus kuin organisaation laajuisella asetuksella, ellei organisaation laajuinen asetus salli tiedostojen jakamista linkeillä, jotka eivät edellytä kirjautumista. Tässä tapauksessa sivustot sallivat jakamisen uusien ja olemassa olevien ulkoisten käyttäjien kanssa, jotka kirjautuvat sisään. Jos haluat muuttaa tiettyjen sivustojen asetusta, käytä uutta SharePoint-hallintakeskusta tai PowerShelliä. [Lisätietoja](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Minkä tahansa sivuston ulkoinen jakamisasetus voi olla rajoittavampi kuin koko organisaation asetus, mutta ei sallivampi kuin organisaation laajuinen asetus. 
  

