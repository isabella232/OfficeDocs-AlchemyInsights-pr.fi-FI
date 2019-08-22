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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525056"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="cab1f-102">Korjaa virhe 0x8004de40 OneDrive</span><span class="sxs-lookup"><span data-stu-id="cab1f-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="cab1f-103">Jos näyttöön tulee virhesanoma 0x8004de40 OneDrive kanssa:</span><span class="sxs-lookup"><span data-stu-id="cab1f-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="cab1f-104">Uudelleenkäynnistystä tietokonetta yhdistettynä Acitve Directory-toimialueeseen.</span><span class="sxs-lookup"><span data-stu-id="cab1f-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="cab1f-105">Jos uudelleenkäynnistys ei korjaa ongelmaa, eroa ja liittyä Azure AD: stä laitteeseen.</span><span class="sxs-lookup"><span data-stu-id="cab1f-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="cab1f-106">**Huomautus**: näiden vaiheiden aikana on oltava yrityksen verkossa.</span><span class="sxs-lookup"><span data-stu-id="cab1f-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="cab1f-107">Älä suorita nämä vaiheet, kun et pysty muodostamaan yhteyttä yrityksen infrastruktuurin (esimerkiksi matkoilla).</span><span class="sxs-lookup"><span data-stu-id="cab1f-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="cab1f-108">Avaa järjestelmänvalvojan oikeuksin suoritettava komentokehote.</span><span class="sxs-lookup"><span data-stu-id="cab1f-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="cab1f-109">Avaa järjestelmänvalvojan oikeuksin suoritettava komentokehote, napsauta - **Käynnistä-painiketta**hiiren kakkospainikkeella **Komentorivi**ja valitsemalla **Suorita järjestelmänvalvojana**.</span><span class="sxs-lookup"><span data-stu-id="cab1f-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="cab1f-110">Kirjoita *dsregcmd /leave* ja paina **Enter**-näppäintä.</span><span class="sxs-lookup"><span data-stu-id="cab1f-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="cab1f-111">Kun asennus on valmis, kirjoita *dsregcmd /join* ja paina **Enter**.</span><span class="sxs-lookup"><span data-stu-id="cab1f-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="cab1f-112">Kun olet valmis, sulje komentokehote.</span><span class="sxs-lookup"><span data-stu-id="cab1f-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="cab1f-113">Käynnistä tietokone uudelleen ja kirjaudu järjestelmään OneDrive.</span><span class="sxs-lookup"><span data-stu-id="cab1f-113">Reboot the computer, and log into OneDrive.</span></span>