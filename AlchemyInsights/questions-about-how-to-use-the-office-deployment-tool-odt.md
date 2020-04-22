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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="43ddd-102">Kysymyksiä Officen käyttöönottotyökalun (ODT) käyttämisestä</span><span class="sxs-lookup"><span data-stu-id="43ddd-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="43ddd-103">Lataa Officen käyttöönottotyökalu [Microsoft Download Centeristä](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="43ddd-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="43ddd-104">Kun olet ladannut tiedoston, suorita itsepurkautuva suoritettava tiedosto, joka sisältää Office Deployment Tool -työkalun suoritustyökalun (setup.exe) ja mallimääritystiedoston (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="43ddd-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="43ddd-105">**Microsoft 365 Apps for enterprise -tuotteiden poissulkeminen asiakastietokoneista:**</span><span class="sxs-lookup"><span data-stu-id="43ddd-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="43ddd-106">Kun asennat Microsoft 365 Apps for Enterprise -sovellusta, voit sulkea pois tiettyjä tuotteita.</span><span class="sxs-lookup"><span data-stu-id="43ddd-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="43ddd-107">Voit tehdä tämän noudattamalla ohjeita Officen odt-yhteyden avulla, mutta sisällytä ExcludeApp-elementti määritystiedostoon.</span><span class="sxs-lookup"><span data-stu-id="43ddd-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="43ddd-108">Tämä määritystiedosto asentaa esimerkiksi kaikki Microsoft 365 Apps for enterprise -tuotteet Publisheria lukuun ottamatta:</span><span class="sxs-lookup"><span data-stu-id="43ddd-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="43ddd-109">Officen käyttöönottotyökalun yleiskatsaus</span><span class="sxs-lookup"><span data-stu-id="43ddd-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

