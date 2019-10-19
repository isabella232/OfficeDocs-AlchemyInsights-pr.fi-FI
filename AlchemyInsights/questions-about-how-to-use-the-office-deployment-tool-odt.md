---
title: Kysymyksiä Officen käyttöönotto työkalun (ODT) käyttämisestä
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553537"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="20c0d-102">Kysymyksiä Officen käyttöönotto työkalun (ODT) käyttämisestä</span><span class="sxs-lookup"><span data-stu-id="20c0d-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="20c0d-103">Lataa Officen käyttöönotto työkalu [Microsoft Download Centeristä](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="20c0d-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="20c0d-104">Kun olet ladannut tiedoston, suorita automaattisesti purkautuva ohjelma tiedosto, joka sisältää Officen käyttöönotto työkalun suoritettavan tiedoston (Setup. exe) ja malli määritys tiedoston (Configuration. xml).</span><span class="sxs-lookup"><span data-stu-id="20c0d-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="20c0d-105">**Voit sulkea Office 365 ProPlus-tuotteet pois asiakas tieto koneista ja poistaa ne:**</span><span class="sxs-lookup"><span data-stu-id="20c0d-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="20c0d-106">Kun asennat Office 365 ProPlusin, voit sulkea pois tiettyjä tuotteita.</span><span class="sxs-lookup"><span data-stu-id="20c0d-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="20c0d-107">Voit tehdä tämän noudattamalla Officen asennus ohjeita ODT:N kanssa, mutta Sisällytä siihen myös Poisdeapp-elementti määritys tiedostossa.</span><span class="sxs-lookup"><span data-stu-id="20c0d-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="20c0d-108">Tämä kokoonpano tiedosto asentaa esimerkiksi kaikki Office 365 ProPlus-tuotteet Publisheria lukuun ottamatta:</span><span class="sxs-lookup"><span data-stu-id="20c0d-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="20c0d-109">Officen käyttöönotto työkalun yleiskatsaus</span><span class="sxs-lookup"><span data-stu-id="20c0d-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

