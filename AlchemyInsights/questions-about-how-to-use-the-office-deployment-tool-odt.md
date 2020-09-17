---
title: Officen käyttöönotto työkalun (ODT) käyttöä koskevia kysymyksiä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774888"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Officen käyttöönotto työkalun (ODT) käyttöä koskevia kysymyksiä

Lataa Officen käyttöönotto työkalu [Microsoft Download Centeristä](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Kun olet ladannut tiedoston, suorita itse purkautuva suoritettava tiedosto, joka sisältää Officen käyttöönotto työkalun suoritettavan tiedoston (setup.exe) ja esimerkki määritys tiedoston (configuration.xml).
  
 **Jos haluat sulkea pois tai poistaa Microsoft 365-sovelluksia yritys tuotteista asiakas tieto koneista:**
  
Kun asennat yritys käyttöön tarkoitettuja Microsoft 365-sovelluksia, voit jättää tietyt tuotteet pois. Jos haluat tehdä näin, noudata ohjeita, jotka koskevat Officen asentamista ODT-ohjelman avulla, mutta Sisällytä ExcludeApp-elementti määritys tiedostoon. Tämä määritys tiedosto asentaa esimerkiksi kaikki yritys tuotteita koskevat Microsoft 365-sovellukset, paitsi Publisherin:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Yleistä Officen käyttöönotto työkalusta](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

