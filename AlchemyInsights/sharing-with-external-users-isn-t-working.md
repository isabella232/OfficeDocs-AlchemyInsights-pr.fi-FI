---
title: Jakaminen ulkoisten käyttäjien kanssa ei toimi
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
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502228"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>SharePoint-sisältöä ulkoisten käyttäjien kanssa jakavan ongelman korjaaminen

Varmista, että ulkoinen jakaminen on käytössä organisaatiossa:
  
1. Siirry [ &amp; Palvelut-apuohjelmat-sivulle Microsoft 365-hallinta keskuksessa](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ja valitse **sivustot**.
    
2. Varmista, että asetus on käytössä. Jos valittuna on "vain nykyiset ulkoiset käyttäjät", varmista, että ulkoinen käyttäjä näkyy Microsoft 365-hallinta keskuksessa.
    
Varmista, että ulkoinen jakaminen on käytössä sivustolla. Klassiseen sivustokokoelmaan:
  
1. Valitse uudessa SharePointin hallinta keskuksessa vasemmassa ruudussa **sivustot**.
    
2. Valitse sivusto tai sivustot ja valitse sitten valinta nauhassa **jakaminen**.
    
Office 365-ryhmään kuuluva ryhmäsivusto tai tieto liikenne sivusto:
  
- Näillä uusilla sivustotyypeilla on sama jakamis asetus kuin organisaatiolla-asetuksella, ellei organisaation laajuinen asetus sallii tiedostojen jakamista sellaisten linkkien avulla, jotka eivät vaadi kirjautumista. Tässä tapa uksessa sivustot sallivat jakamisen uusille ja olemassa oleville ulkoisille käyttäjille, jotka kirjautumiseen. Jos haluat muuttaa tiettyjen sivustojen asetuksia, käytä uutta SharePointin hallinta keskusta tai PowerShelliä. [Lue lisää](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Ulkoisen jakamisen asetus missä tahansa sivustossa voi olla rajoittavampi kuin koko organisaatiota koskeva asetus, mutta ei enemmän salliva kuin organisaation laajuinen asetus. 
  

