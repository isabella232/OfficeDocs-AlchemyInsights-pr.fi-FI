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
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371765"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="037ac-102">Kysymyksiin siitä, miten voit käyttää Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="037ac-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="037ac-103">Lataa Office Deployment Tool-työkalua [Microsoft Download Centeristä](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="037ac-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="037ac-104">Sen jälkeen tiedoston lataamisessa suorittamalla automaattisesti purkautuva suoritettava tiedosto, joka sisältää Office Deployment Tool suoritustiedoston (setup.exe) ja kokoonpano-tiedosto (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="037ac-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="037ac-105">**Voit jättää tai poistaa Office 365 ProPlus tuotteita asiakastietokoneista:**</span><span class="sxs-lookup"><span data-stu-id="037ac-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="037ac-106">Kun asennat Office 365 ProPlus, voit jättää pois tiettyjä tuotteita.</span><span class="sxs-lookup"><span data-stu-id="037ac-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="037ac-107">Voit tehdä toimet asentaa Officen ODT kanssa, mutta sisällyttää kokoonpanomääritystiedoston ExcludeApp-elementin.</span><span class="sxs-lookup"><span data-stu-id="037ac-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="037ac-108">Esimerkiksi tämän kokoonpanon tiedoston asentaa Office 365 ProPlus tuotteita kuin Publisher:</span><span class="sxs-lookup"><span data-stu-id="037ac-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="037ac-109">Yleisiä tietoja Office Deployment Tool-työkalua</span><span class="sxs-lookup"><span data-stu-id="037ac-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

