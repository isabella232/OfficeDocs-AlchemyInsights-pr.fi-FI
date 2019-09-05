---
title: Korjaa 0x8004de40-virhe OneDrivessa
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755845"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="91709-102">Korjaa 0x8004de40-virhe OneDrivessa</span><span class="sxs-lookup"><span data-stu-id="91709-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="91709-103">Jos näyttöön tulee virhe 0x8004de40 OneDrivessa:</span><span class="sxs-lookup"><span data-stu-id="91709-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="91709-104">Käynnistä haavoittuvuuden sisältävät tieto kone uudelleen, kun olet muodostanut yhteyden Acitve-hakemisto toimi alueeseen.</span><span class="sxs-lookup"><span data-stu-id="91709-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="91709-105">Jos uudelleenkäynnistys ei korjaa ongelmaa, avaa laitteen liitos ja liitä se uudelleen Azure ADISTA.</span><span class="sxs-lookup"><span data-stu-id="91709-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="91709-106">**Huomautus**: sinun pitäisi olla yrityksen verkossa, kun suoritat näitä vaiheita.</span><span class="sxs-lookup"><span data-stu-id="91709-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="91709-107">Älä tee näitä vaiheita, kun et pysty muodostamaan yhteyttä yrityksen infrastruktuuriin (esimerkiksi matkoilla).</span><span class="sxs-lookup"><span data-stu-id="91709-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="91709-108">Avaa laajennettu komento kehote.</span><span class="sxs-lookup"><span data-stu-id="91709-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="91709-109">Voit avata järjestelmänvalvojan oikeuksin suoritettavan komento kehotteen valitsemalla- **Käynnistä**, napsauttamalla hiiren kakkos painikkeella **komento kehote**-kohtaa ja valitsemalla sitten **Suorita järjestelmänvalvojana**.</span><span class="sxs-lookup"><span data-stu-id="91709-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="91709-110">Kirjoita *dsregcmd/Leave* ja paina **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="91709-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="91709-111">Kun olet valmis, kirjoita *dsregcmd/Join* ja paina **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="91709-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="91709-112">Kun olet valmis, sulje komento kehote.</span><span class="sxs-lookup"><span data-stu-id="91709-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="91709-113">Käynnistä tieto kone uudelleen ja Kirjaudu sisään OneDriveen.</span><span class="sxs-lookup"><span data-stu-id="91709-113">Reboot the computer, and log into OneDrive.</span></span>