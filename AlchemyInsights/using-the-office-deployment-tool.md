---
title: Office Deployment-työkalun avulla
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287163"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="3044d-102">Office Deployment Tool (ODT-työkalun) avulla</span><span class="sxs-lookup"><span data-stu-id="3044d-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="3044d-p101">Office Deployment Tool (ODT) avulla voit ottaa käyttöön Office-version Office 365: ssä. Office Deployment Tool-työkalua (setup.exe) suoritetaan komentoriviltä, ja selvittää, mitä asetuksia, voit ottaa käyttöön Office XML-määritystiedoston avulla.</span><span class="sxs-lookup"><span data-stu-id="3044d-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="3044d-105">Lataa uusin versio Office Deployment Tool-työkalua [Microsoft Download Centeristä](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="3044d-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="3044d-p102">Luo XML-määritystiedosto ja valitse käyttöönoton asetukset [Office Customization Tool (OCT)](https://config.office.com) avulla. Määritystiedoston vieminen ja sijoittaa sen paikallisesti samaan kansioon, jossa asuu setup.exe.</span><span class="sxs-lookup"><span data-stu-id="3044d-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="3044d-p103">**Huomautus:** Office-asennuksen ongelmista esiintyy yleisesti asianmukaisesti, sen kokoonpano on väärä tai malformatted määritystiedostoja. Tällaisten ongelmien välttämiseksi on suositeltavaa, että käytät Officen mukauttamistyökalun määritystiedoston luominen. Voit myös tuoda aiemmin luotuja määritystiedostoja Officen mukauttamistyökalun.</span><span class="sxs-lookup"><span data-stu-id="3044d-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="3044d-p104">Siirry sijaintiin, jossa asuu setup.exe järjestelmänvalvojan oikeuksin suoritettava komentorivi ja suorita Office Deployment Tool-työkalua download tilassa ja määrittää tiedoston juuri tallennettu. Tässä esimerkissä tiedoston nimi on Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="3044d-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="3044d-113">Suorita Office Deployment Tool-työkalua ja määritä tila määrittää määritystiedoston.</span><span class="sxs-lookup"><span data-stu-id="3044d-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="3044d-114">**Huomautus:** Tämä vaihe on suoritettava asiakastietokoneesta, johon haluat asentaa Officen ja sinulla on oltava paikallisen järjestelmänvalvojan oikeudet tietokoneeseen.</span><span class="sxs-lookup"><span data-stu-id="3044d-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="3044d-p105">Saat lisätietoja Office Deployment Tool-työkalua käyttämällä Office 365 ProPlus käyttöönottoprosessissa on [Yleiskatsaus Office Deployment Tool-työkalua](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Lisätietoja Officen mukauttamistyökalun käyttämisestä on ohjeaiheessa [Officen mukauttamistyökalun yleiskatsaus](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="3044d-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

