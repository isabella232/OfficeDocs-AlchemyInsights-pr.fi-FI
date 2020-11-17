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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="dad85-102">Officen käyttöönotto työkalun (ODT) käyttöä koskevia kysymyksiä</span><span class="sxs-lookup"><span data-stu-id="dad85-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="dad85-103">Lataa Officen käyttöönotto työkalu [Microsoft Download Centeristä](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="dad85-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="dad85-104">Kun olet ladannut tiedoston, suorita itse purkautuva suoritettava tiedosto, joka sisältää Officen käyttöönotto työkalun suoritettavan tiedoston (setupodt.exe) ja esimerkki määritys tiedoston (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="dad85-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="dad85-105">**Jos haluat sulkea pois tai poistaa Microsoft 365-sovelluksia yritys tuotteista asiakas tieto koneista:**</span><span class="sxs-lookup"><span data-stu-id="dad85-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="dad85-106">Kun asennat yritys käyttöön tarkoitettuja Microsoft 365-sovelluksia, voit jättää tietyt tuotteet pois.</span><span class="sxs-lookup"><span data-stu-id="dad85-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="dad85-107">Jos haluat tehdä näin, noudata ohjeita, jotka koskevat Officen asentamista ODT-ohjelman avulla, mutta Sisällytä ExcludeApp-elementti määritys tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="dad85-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="dad85-108">Tämä määritys tiedosto asentaa esimerkiksi kaikki yritys tuotteita koskevat Microsoft 365-sovellukset, paitsi Publisherin:</span><span class="sxs-lookup"><span data-stu-id="dad85-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="dad85-109">Yleistä Officen käyttöönotto työkalusta</span><span class="sxs-lookup"><span data-stu-id="dad85-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

