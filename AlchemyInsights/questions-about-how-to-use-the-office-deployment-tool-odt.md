---
title: Kysymyksiin siitä, miten voit käyttää Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553537"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Kysymyksiin siitä, miten voit käyttää Office Deployment Tool (ODT)

Lataa Office Deployment Tool-työkalua [Microsoft Download Centeristä](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Sen jälkeen tiedoston lataamisessa suorittamalla automaattisesti purkautuva suoritettava tiedosto, joka sisältää Office Deployment Tool suoritustiedoston (setup.exe) ja kokoonpano-tiedosto (configuration.xml).
  
 **Voit jättää tai poistaa Office 365 ProPlus tuotteita asiakastietokoneista:**
  
Kun asennat Office 365 ProPlus, voit jättää pois tiettyjä tuotteita. Voit tehdä toimet asentaa Officen ODT kanssa, mutta sisällyttää kokoonpanomääritystiedoston ExcludeApp-elementin. Esimerkiksi tämän kokoonpanon tiedoston asentaa Office 365 ProPlus tuotteita kuin Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Yleisiä tietoja Office Deployment Tool-työkalua](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

