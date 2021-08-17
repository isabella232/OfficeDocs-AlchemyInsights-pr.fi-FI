---
title: Jakaminen ulkoisten käyttäjien kanssa ei toimi
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
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304366"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Sisällön jakamiseen ulkoisten SharePoint ongelmien ratkaiseminen

Varmista, että ulkoinen jakaminen on otettu käyttöön organisaatiossasi:
  
1. Siirry [ &amp; Palvelut-apuohjelmat-sivulle](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)Microsoft 365 -hallintakeskus ja **valitse Sivustot**.
    
2. Varmista, että asetuksena on Käytössä. Jos Vain aiemmin luodut ulkoiset käyttäjät on valittuna, varmista, että ulkoinen käyttäjä näkyy Microsoft 365 -hallintakeskus.
    
Varmista, että ulkoinen jakaminen on otettu käyttöön sivustossa. Jos sivustokokoelma on perinteinen:
  
1. Valitse SharePoint hallintakeskuksen vasemmanpuoleisessa **ruudussa Sivustot**.
    
2. Valitse sivusto tai sivustot ja valitse sitten valintanauhassa **Jakaminen**.
    
Ryhmäsivuston, joka kuuluu Microsoft 365 tai viestintäsivustoon:
  
- Näillä uusilla sivustotyypeillä on sama jakamisasetus kuin koko organisaatiolla, ellei koko organisaation laajuisessa asetus salli tiedostojen jakamista linkeissä, jotka eivät vaadi kirjautumista sisään. Tässä tapauksessa sivustot sallivat jakamisen uusien ja aiemmin luotujen ulkoisten käyttäjien kanssa, jotka kirjautuvat sisään. Jos haluat muuttaa tiettyjen sivustojen asetuksia, käytä uutta hallintakeskusta SharePoint PowerShelliä. [Lisätietoja](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Huomautus:** Minkä tahansa sivuston ulkoisen jakamisen asetus voi olla rajoittavampi kuin koko organisaation laajuinen asetus, mutta enintään organisaation laajuinen asetus. 
  

