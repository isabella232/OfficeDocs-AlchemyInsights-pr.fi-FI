---
title: Microsoft 365 -ryhmien tervetuloviesti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357537"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="39807-102">Microsoft 365 -ryhmien tervetuloviesti</span><span class="sxs-lookup"><span data-stu-id="39807-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="39807-103">Microsoft 365 -ryhmään liittyvät uudet käyttäjät saavat tervetulosähköpostiviestin, jos UnifiedGroupWelcomeMessageEnabled-ominaisuus on True.</span><span class="sxs-lookup"><span data-stu-id="39807-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="39807-104">Jos haluat poistaa tervetuloviestin käytöstä, käytä seuraavaa [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) -komentoa:</span><span class="sxs-lookup"><span data-stu-id="39807-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
