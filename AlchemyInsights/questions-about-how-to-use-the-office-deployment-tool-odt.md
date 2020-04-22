---
title: Kysymyksiä Officen käyttöönottotyökalun (ODT) käyttämisestä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698055"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Kysymyksiä Officen käyttöönottotyökalun (ODT) käyttämisestä

Lataa Officen käyttöönottotyökalu [Microsoft Download Centeristä](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Kun olet ladannut tiedoston, suorita itsepurkautuva suoritettava tiedosto, joka sisältää Office Deployment Tool -työkalun suoritustyökalun (setup.exe) ja mallimääritystiedoston (configuration.xml).
  
 **Microsoft 365 Apps for enterprise -tuotteiden poissulkeminen asiakastietokoneista:**
  
Kun asennat Microsoft 365 Apps for Enterprise -sovellusta, voit sulkea pois tiettyjä tuotteita. Voit tehdä tämän noudattamalla ohjeita Officen odt-yhteyden avulla, mutta sisällytä ExcludeApp-elementti määritystiedostoon. Tämä määritystiedosto asentaa esimerkiksi kaikki Microsoft 365 Apps for enterprise -tuotteet Publisheria lukuun ottamatta:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Officen käyttöönottotyökalun yleiskatsaus](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

