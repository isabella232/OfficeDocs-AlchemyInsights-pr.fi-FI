---
title: Korjaa virhe 0x8004de40 OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133974"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="927ba-102">Korjaa virhe 0x8004de40 OneDrive</span><span class="sxs-lookup"><span data-stu-id="927ba-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="927ba-103">Jos näyttöön tulee virhesanoma 0x8004de40 OneDrive kanssa:</span><span class="sxs-lookup"><span data-stu-id="927ba-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="927ba-104">Uudelleenkäynnistystä tietokonetta yhdistettynä Acitve Directory-toimialueeseen.</span><span class="sxs-lookup"><span data-stu-id="927ba-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="927ba-105">Jos uudelleenkäynnistys ei korjaa ongelmaa, eroa ja liittyä Azure AD: stä laitteeseen.</span><span class="sxs-lookup"><span data-stu-id="927ba-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="927ba-106">**Huomautus**: näiden vaiheiden aikana on oltava yrityksen verkossa.</span><span class="sxs-lookup"><span data-stu-id="927ba-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="927ba-107">Älä suorita nämä vaiheet, kun et pysty muodostamaan yhteyttä yrityksen infrastruktuurin (esimerkiksi matkoilla).</span><span class="sxs-lookup"><span data-stu-id="927ba-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="927ba-108">Avaa järjestelmänvalvojan oikeuksin suoritettava komentokehote.</span><span class="sxs-lookup"><span data-stu-id="927ba-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="927ba-109">Avaa järjestelmänvalvojan oikeuksin suoritettava komentokehote, napsauta - **Käynnistä-painiketta**hiiren kakkospainikkeella **Komentorivi**ja valitsemalla **Suorita järjestelmänvalvojana**.</span><span class="sxs-lookup"><span data-stu-id="927ba-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="927ba-110">Kirjoita *dsregcmd /leave* ja paina **Enter**-näppäintä.</span><span class="sxs-lookup"><span data-stu-id="927ba-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="927ba-111">Kun asennus on valmis, kirjoita *dsregcmd /join* ja paina **Enter**.</span><span class="sxs-lookup"><span data-stu-id="927ba-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="927ba-112">Kun olet valmis, sulje komentokehote.</span><span class="sxs-lookup"><span data-stu-id="927ba-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="927ba-113">Käynnistä tietokone uudelleen ja kirjaudu järjestelmään OneDrive.</span><span class="sxs-lookup"><span data-stu-id="927ba-113">Reboot the computer, and log into OneDrive.</span></span>