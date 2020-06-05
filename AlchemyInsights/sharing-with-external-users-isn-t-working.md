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
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582772"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>SharePoint-sisällön jakamiseen ulkoisten käyttäjien kanssa liittyvien ongelmien korjaaminen

Varmista, että ulkoinen jakaminen on otettu käyttöön organisaatiossa:
  
1. Siirry [Microsoft &amp; 365 -hallintakeskuksen Palvelut-apuohjelmat-sivulle](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ja valitse **Sivustot**.
    
2. Varmista, että asetuksen asetus on Käytössä. Jos "Vain aiemmin luodut ulkoiset käyttäjät" on valittuna, varmista, että ulkoinen käyttäjä on Microsoft 365 -hallintakeskuksessa.
    
Varmista, että ulkoinen jakaminen on käytössä sivustossa. Klassinen sivustokokoelma:
  
1. Valitse uudessa SharePoint-hallintakeskuksessa vasemmanpuoleisesta ruudusta **sivustot**.
    
2. Valitse sivusto tai sivustot ja valitse valintanauhasta **Jakaminen**.
    
Jos ryhmäsivusto kuuluu Microsoft 365 -ryhmään tai viestintäsivustoon:
  
- Näillä uusilla sivustotyypeillä on sama jakamisasetus kuin organisaation laajuisella asetuksella, ellei organisaation laajuinen asetus salli tiedostojen jakamista linkeillä, jotka eivät edellytä kirjautumista. Tässä tapauksessa sivustot sallivat jakamisen uusien ja olemassa olevien ulkoisten käyttäjien kanssa, jotka kirjautuvat sisään. Jos haluat muuttaa tiettyjen sivustojen asetusta, käytä uutta SharePoint-hallintakeskusta tai PowerShelliä. [Lisätietoja](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Minkä tahansa sivuston ulkoinen jakamisasetus voi olla rajoittavampi kuin organisaation laajuinen asetus, mutta ei sallivampi kuin organisaation laajuinen asetus. 
  

