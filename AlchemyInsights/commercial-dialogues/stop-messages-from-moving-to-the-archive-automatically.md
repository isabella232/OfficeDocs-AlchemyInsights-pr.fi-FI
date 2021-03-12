---
title: Viestien automaattinen siirtäminen arkistoon
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746333"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="b4bb4-102">Viestien automaattinen siirtäminen arkistoon</span><span class="sxs-lookup"><span data-stu-id="b4bb4-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="b4bb4-103">Jos käytät säilytyskäytäntöä, voit muuttaa tämän käytännön säilytysikää niin, että viestit eivät arkistoi automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="b4bb4-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="b4bb4-104">Toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="b4bb4-104">Here's how:</span></span>

1. <span data-ttu-id="b4bb4-105">Valitse [Exchange-hallintakeskuksessa](https://go.microsoft.com/fwlink/?linkid=2059104)yhteensopivuuden **hallinnan**  >  **säilytystunnisteet.**</span><span class="sxs-lookup"><span data-stu-id="b4bb4-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="b4bb4-106">Etsi Siirrä arkistoon -säilytystunniste.</span><span class="sxs-lookup"><span data-stu-id="b4bb4-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="b4bb4-107">Muuta säilytystunnisteessa säilytysaika (arkistointijakso)  ei koskaan, jos haluat estää säilytyskäytännön automaattisesti arkistoimasta kohteita.</span><span class="sxs-lookup"><span data-stu-id="b4bb4-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="b4bb4-108">Tämä muuttaa kaikkien niiden postilaatikoiden arkistoasetusta, joissa on käytössä tämä säilytystunniste.</span><span class="sxs-lookup"><span data-stu-id="b4bb4-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
