---
title: 0x8004de40 OneDriven käynnistämisen virhesanoma
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813649"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="5aed8-102">0x8004de40 OneDriven käynnistämisen virhesanoma</span><span class="sxs-lookup"><span data-stu-id="5aed8-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="5aed8-103">Jos saat virheilmoituksen **0x8004de40** kirjauduttaessa OneDriveen, käynnistä tietokone uudelleen, kun olet yhteydessä työ- tai koulutoimialueeseen.</span><span class="sxs-lookup"><span data-stu-id="5aed8-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="5aed8-104">Jos saat tämän virheen uudelleenkäynnistyksen jälkeen, kokeile tätä, kun olet muodostanut yhteyden työ- tai koulutoimialueeseen:</span><span class="sxs-lookup"><span data-stu-id="5aed8-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="5aed8-105">Valitse Käynnistä ja kirjoita  **hakuruutuun cmd** tai komentokehote, napsauta komentokehotesovellusta hiiren kakkospainikkeella ja valitse **Suorita järjestelmänvalvojana**.</span><span class="sxs-lookup"><span data-stu-id="5aed8-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="5aed8-106">Jos sinua pyydetään antamaan järjestelmänvalvojan salasana tai vahvistus, kirjoita salasana tai valitse **Salli**.</span><span class="sxs-lookup"><span data-stu-id="5aed8-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="5aed8-107">Kirjoita Komentokehote-ikkunassa **dsregcmd /leave**  ja odota, että komento on valmis.</span><span class="sxs-lookup"><span data-stu-id="5aed8-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="5aed8-108">Kirjoita **sitten dsregcmd /join** ja odota, että komento on valmis.</span><span class="sxs-lookup"><span data-stu-id="5aed8-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="5aed8-109">Käynnistä tietokone uudelleen.</span><span class="sxs-lookup"><span data-stu-id="5aed8-109">Reboot your computer.</span></span>
