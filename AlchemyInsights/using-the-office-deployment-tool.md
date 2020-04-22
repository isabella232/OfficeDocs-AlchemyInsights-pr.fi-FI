---
title: Officen käyttöönottotyökalun käyttäminen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726245"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="6b6b9-102">Officen käyttöönottotyökalun (ODT) käyttäminen</span><span class="sxs-lookup"><span data-stu-id="6b6b9-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="6b6b9-103">Office 365 -version käyttöönotto on office-käyttöönottotyökalua (ODT) käyttämällä.</span><span class="sxs-lookup"><span data-stu-id="6b6b9-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="6b6b9-104">Officen käyttöönottotyökalu (setup.exe) suoritetaan komentoriviltä, ja sen avulla määritetään xml-määritystiedoston avulla, mitä asetuksia Officen käyttöönotossa käytetään.</span><span class="sxs-lookup"><span data-stu-id="6b6b9-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="6b6b9-105">Lataa Officedeployment Tool -työkalun uusin versio [Microsoft Download Centeristä](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="6b6b9-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="6b6b9-106">Valitse käyttöönottoasetukset ja luo xml-määritystiedosto [Officecustomization Tool (OCT) -työkalun](https://config.office.com) avulla.</span><span class="sxs-lookup"><span data-stu-id="6b6b9-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="6b6b9-107">Vie määritystiedosto ja sijoita se paikallisesti samaan kansioon, jossa setup.exe sijaitsee.</span><span class="sxs-lookup"><span data-stu-id="6b6b9-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="6b6b9-108">**Huomautus:** Officen asennusongelmia ilmenee yleensä virheellisesti määritettyjen tai väärin muotoiltujen määritystiedostojen vuoksi.</span><span class="sxs-lookup"><span data-stu-id="6b6b9-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="6b6b9-109">Tällaisten ongelmien välttämiseksi on suositeltavaa luoda määritystiedosto Officen mukautustyökalun avulla.</span><span class="sxs-lookup"><span data-stu-id="6b6b9-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="6b6b9-110">Voit myös tuoda aiemmin luotuja määritystiedostoja Officen mukautustyökaluun.</span><span class="sxs-lookup"><span data-stu-id="6b6b9-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="6b6b9-111">Siirry laajennetusta komentorivistä sijaintiin, jossa setup.exe sijaitsee, ja suorita Officedeployment Tool lataustilassa ja määritä juuri tallentamasi määritystiedosto.</span><span class="sxs-lookup"><span data-stu-id="6b6b9-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="6b6b9-112">Tässä esimerkissä määritystiedoston nimi on Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="6b6b9-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="6b6b9-113">Suorita Officen käyttöönottotyökalu määritystilassa ja määritä määritystiedosto.</span><span class="sxs-lookup"><span data-stu-id="6b6b9-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="6b6b9-114">**Huomautus:** Sinun on suoritettava tämä vaihe asiakastietokoneesta, johon haluat asentaa Officen, ja sinulla on oltava paikallisen järjestelmänvalvojan oikeudet kyseiseen tietokoneeseen.</span><span class="sxs-lookup"><span data-stu-id="6b6b9-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="6b6b9-115">Lisätietoja Officedeployment Tool -työkalun käyttämisestä Microsoft 365 Apps for enterprise -käyttöönottoskenaarioissa on artikkelissa [Officen käyttöönottotyökalun yleiskatsaus](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="6b6b9-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="6b6b9-116">Lisätietoja Officen mukautustyökalun käyttämisestä on artikkelissa [Officen mukautustyökalun yleiskatsaus](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="6b6b9-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
