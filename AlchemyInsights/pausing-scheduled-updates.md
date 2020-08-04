---
title: Ajoitettujen päivitysten keskeyttäminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555105"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="effe4-102">Ajoitettujen päivitysten keskeyttäminen</span><span class="sxs-lookup"><span data-stu-id="effe4-102">Pausing scheduled updates</span></span>

<span data-ttu-id="effe4-103">Kun taukokomento annetaan, laitteet käsittelevät komentoa vasta, kun he seuraavan kerran kuittaavat sisään Intuneen.</span><span class="sxs-lookup"><span data-stu-id="effe4-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="effe4-104">Tämän vuoksi laitteissasi voi olla:</span><span class="sxs-lookup"><span data-stu-id="effe4-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="effe4-105">Ajoitetut päivitykset asennettiin ennen sisäänkirjautumisen aloittamista.</span><span class="sxs-lookup"><span data-stu-id="effe4-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="effe4-106">On sammutettu, kun sait taukokomennon.</span><span class="sxs-lookup"><span data-stu-id="effe4-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="effe4-107">Tässä tapauksessa, kun laitteet olivat päällä, ne ovat saattaneet ladata ja asentaa ajoitetut päivitykset ennen sisäänkirjautumista.</span><span class="sxs-lookup"><span data-stu-id="effe4-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>