---
title: Kysymyksiä Office Käyttöönottotyökalun (ODT) käytöstä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959680"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Kysymyksiä Office Käyttöönottotyökalun (ODT) käytöstä

Lataa Office käyttöönottotyökalu Microsoft [Download Centeristä.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Kun olet ladanut tiedoston, suorita suoritettava suoritettava tiedosto, joka sisältää suoritettavan Office Deployment Tool (setup.exe) -työkalun ja mallimääritystiedoston (configuration.xml).
  
 **Jos haluat poistaa Microsoft 365 -sovellukset suuryrityksille asiakastietokoneista:**
  
Kun asennat Microsoft 365 -sovellukset suuryrityksille, voit jättää tietyt tuotteet pois. Noudata ohjeita, kun asennat Office ODT:n mukana, mutta sisällytä ExcludeApp-elementti määritystiedostoon. Esimerkiksi tämä määritystiedosto asentaa kaikki muut Microsoft 365 -sovellukset suuryrityksille paitsi Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Yleistä Office käyttöönottotyökalusta](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

