---
title: Korjaa 0x8004de40-virhe OneDrivessa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716025"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="4b5cd-102">Korjaa 0x8004de40-virhe OneDrivessa</span><span class="sxs-lookup"><span data-stu-id="4b5cd-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="4b5cd-103">Jos saat 0x8004de40-virheen OneDrivessa:</span><span class="sxs-lookup"><span data-stu-id="4b5cd-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="4b5cd-104">Käynnistä haavoittuvuuden sisältävä tietokone uudelleen, kun se on yhteydessä Acitve Directory -toimialueeseen.</span><span class="sxs-lookup"><span data-stu-id="4b5cd-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="4b5cd-105">Jos uudelleenkäynnistys ei korjaa ongelmaa, poista liittyminen ja liity laitteeseesi uudelleen Azure AD:stä.</span><span class="sxs-lookup"><span data-stu-id="4b5cd-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="4b5cd-106">**Huomautus:** Sinun pitäisi olla yrityksen verkossa, kun suoritat näitä vaiheita.</span><span class="sxs-lookup"><span data-stu-id="4b5cd-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="4b5cd-107">Älä tee näitä vaiheita, kun et pysty muodostamaan yhteyttä yrityksen infrastruktuuriin (esimerkiksi matkoilla).</span><span class="sxs-lookup"><span data-stu-id="4b5cd-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="4b5cd-108">Avaa laajennettu komentokehote.</span><span class="sxs-lookup"><span data-stu-id="4b5cd-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="4b5cd-109">Voit avata komentorivin valitsemalla - **Käynnistä**, napsauttamalla **komentoriviä**hiiren kakkospainikkeella ja valitsemalla sitten **Suorita järjestelmänvalvojana**.</span><span class="sxs-lookup"><span data-stu-id="4b5cd-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="4b5cd-110">Kirjoita *dsregcmd /leave* ja paina **Enter**.</span><span class="sxs-lookup"><span data-stu-id="4b5cd-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="4b5cd-111">Kun olet valmis, kirjoita *dsregcmd /join* ja paina **Enter**.</span><span class="sxs-lookup"><span data-stu-id="4b5cd-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="4b5cd-112">Kun olet valmis, sulje komentokehote.</span><span class="sxs-lookup"><span data-stu-id="4b5cd-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="4b5cd-113">Käynnistä tietokone uudelleen ja kirjaudu OneDriveen.</span><span class="sxs-lookup"><span data-stu-id="4b5cd-113">Reboot the computer, and log into OneDrive.</span></span>