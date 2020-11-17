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
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086153"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Officen käyttöönotto työkalun (ODT) käyttöä koskevia kysymyksiä

Lataa Officen käyttöönotto työkalu [Microsoft Download Centeristä](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Kun olet ladannut tiedoston, suorita itse purkautuva suoritettava tiedosto, joka sisältää Officen käyttöönotto työkalun suoritettavan tiedoston (setupodt.exe) ja esimerkki määritys tiedoston (configuration.xml).
  
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
  

