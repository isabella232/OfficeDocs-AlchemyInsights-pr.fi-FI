---
title: Korjaa 0x8004de40-virhe OneDrivessa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745127"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="f2b84-102">Korjaa 0x8004de40-virhe OneDrivessa</span><span class="sxs-lookup"><span data-stu-id="f2b84-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="f2b84-103">Jos näyttöön tulee 0x8004de40-virhe OneDrivessa:</span><span class="sxs-lookup"><span data-stu-id="f2b84-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="f2b84-104">Käynnistä haavoittuvuuden sisältävä tieto kone uudelleen, kun se on yhdistetty Acitve-hakemisto domainiin.</span><span class="sxs-lookup"><span data-stu-id="f2b84-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="f2b84-105">Jos uudelleenkäynnistys ei korjaa ongelmaa, Yhdistä laite Azure AD:stä ja liity siihen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="f2b84-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="f2b84-106">**Huomautus**: sinun pitäisi olla yritys verkossasi, kun suoritat näitä vaiheita.</span><span class="sxs-lookup"><span data-stu-id="f2b84-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="f2b84-107">Älä suorita näitä vaiheita, jos et voi muodostaa yhteyttä yrityksen infrastruktuuriin (esimerkiksi matkoilla).</span><span class="sxs-lookup"><span data-stu-id="f2b84-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="f2b84-108">Avaa järjestelmänvalvojan oikeuksin suoritettava komento kehote.</span><span class="sxs-lookup"><span data-stu-id="f2b84-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="f2b84-109">Avaa järjestelmänvalvojan oikeuksin suoritettava komento kehote napsauttamalla- **Käynnistä**, napsauttamalla hiiren kakkos painikkeella **komento kehote**ja valitsemalla sitten **Suorita järjestelmänvalvojana**.</span><span class="sxs-lookup"><span data-stu-id="f2b84-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="f2b84-110">Kirjoita *dsregcmd/Leave* ja paina **ENTER**-näppäintä.</span><span class="sxs-lookup"><span data-stu-id="f2b84-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="f2b84-111">Kun olet valmis, kirjoita *dsregcmd/Join* ja paina **ENTER**-näppäintä.</span><span class="sxs-lookup"><span data-stu-id="f2b84-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="f2b84-112">Kun olet valmis, sulje komento kehote.</span><span class="sxs-lookup"><span data-stu-id="f2b84-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="f2b84-113">Käynnistä tieto kone uudelleen ja Kirjaudu sisään OneDriveen.</span><span class="sxs-lookup"><span data-stu-id="f2b84-113">Reboot the computer, and log into OneDrive.</span></span>