---
title: 0x8004de40-Virhe käynnistettäessä OneDrivea
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823047"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="04604-102">0x8004de40-Virhe käynnistettäessä OneDrivea</span><span class="sxs-lookup"><span data-stu-id="04604-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="04604-103">Jos näyttöön tulee virhe **0x8004de40,** kun kirja Udut sisään OneDriveen, Käynnistä tieto kone uudelleen, kun olet muodostanut yhteyden työpaikan tai oppi laitoksen toimi alueeseen.</span><span class="sxs-lookup"><span data-stu-id="04604-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="04604-104">Jos saat tämän virheen uudelleenkäynnistyksen jälkeen, kokeile tätä, kun olet muodostanut yhteyden työpaikan tai oppi laitoksen toimi alueeseen:</span><span class="sxs-lookup"><span data-stu-id="04604-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="04604-105">Napsauta Käynnistä-painiketta ja kirjoita haku ruutuun **cmd** tai **komento kehote**  , napsauta komento kehote-sovellusta hiiren kakkos painikkeella ja valitse  **Suorita järjestelmänvalvojana** .</span><span class="sxs-lookup"><span data-stu-id="04604-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="04604-106">Jos sinua pyydetään antamaan järjestelmänvalvojan sala sana tai vahvistamaan toiminto, kirjoita sala sana tai valitse **Salli** .</span><span class="sxs-lookup"><span data-stu-id="04604-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="04604-107">Kirjoita komento kehote ikkunaan **dsregcmd/Leave**  ja odota, kunnes komento on valmis.</span><span class="sxs-lookup"><span data-stu-id="04604-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="04604-108">Kirjoita sitten **dsregcmd/Join** ja odota, kunnes komento on valmis.</span><span class="sxs-lookup"><span data-stu-id="04604-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="04604-109">Käynnistä tieto kone uudelleen.</span><span class="sxs-lookup"><span data-stu-id="04604-109">Reboot your computer.</span></span>
