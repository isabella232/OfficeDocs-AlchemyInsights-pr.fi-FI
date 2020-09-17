---
title: Officen käyttöönotto työkalun käyttäminen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794908"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="98b90-102">Officen käyttöönotto työkalun (ODT) käyttäminen</span><span class="sxs-lookup"><span data-stu-id="98b90-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="98b90-103">Käytät Officen käyttöönotto työkalua (ODT) Office 365-versioiden käyttöönottoon.</span><span class="sxs-lookup"><span data-stu-id="98b90-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="98b90-104">Officen käyttöönotto työkalu (setup.exe) suoritetaan komento riviltä, ja sen avulla määritetään, mitkä asetukset otetaan käyttöön Officen käyttöönoton yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="98b90-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="98b90-105">Lataa Officen käyttöönotto työkalun uusin versio [Microsoft Download Centeristä](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="98b90-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="98b90-106">Voit valita käyttöönoton asetukset ja luoda määrityksen XML-tiedoston [Officen mukautus työkalun (OCT)](https://config.office.com) avulla.</span><span class="sxs-lookup"><span data-stu-id="98b90-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="98b90-107">Vie määritys tiedosto ja sijoita se paikallisesti samaan kansioon, jossa setup.exe sijaitsee.</span><span class="sxs-lookup"><span data-stu-id="98b90-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="98b90-108">**Huomautus:** Officen asennus ongelmat tapahtuvat yleensä väärin käytettyjen määritys tiedostojen vuoksi.</span><span class="sxs-lookup"><span data-stu-id="98b90-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="98b90-109">Jos haluat välttää tällaiset ongelmat, suosittelemme, että luot määritys tiedoston Officen mukautus työkalun avulla.</span><span class="sxs-lookup"><span data-stu-id="98b90-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="98b90-110">Voit myös tuoda aiemmin luotuja määritys tiedostoja Officen mukautus työkaluun.</span><span class="sxs-lookup"><span data-stu-id="98b90-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="98b90-111">Siirry laajennetussa komento kehotteessa sijaintiin, jossa setup.exe sijaitsee, ja suorita Officen käyttöönotto työkalu lataus tilassa ja määritä juuri tallentamasi määritys tiedosto.</span><span class="sxs-lookup"><span data-stu-id="98b90-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="98b90-112">Tässä esimerkissä määritys tiedoston nimi on Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="98b90-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setup.exe /download Configuration.xml```

<span data-ttu-id="98b90-113">4. Suorita Officen käyttöönotto työkalu Määritä-tilassa ja määritä määritys tiedosto.</span><span class="sxs-lookup"><span data-stu-id="98b90-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setup.exe /configure Configuration.xml```

<span data-ttu-id="98b90-114">**Huomautus:** Sinun on suoritettava tämä vaihe asiakas tieto koneesta, johon haluat asentaa Officen, ja sinulla on oltava paikallisen Järjestelmänvalvoja-oikeudet kyseisessä tieto koneessa.</span><span class="sxs-lookup"><span data-stu-id="98b90-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="98b90-115">Lisä tietoja Officen käyttöönotto työkalun käyttämisestä Microsoft 365-sovelluksissa yritys käyttöönoton skenaarioissa on artikkelissa [yleistä Office-käyttöönotto työkalusta](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="98b90-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="98b90-116">Lisä tietoja Officen mukautus työkalun käyttämisestä on Ohje aiheessa [Officen mukautus työkalun yleiskatsaus](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="98b90-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
