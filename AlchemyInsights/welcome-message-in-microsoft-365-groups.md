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
# <a name="welcome-message-in-microsoft-365-groups"></a>Microsoft 365 -ryhmien tervetuloviesti

Microsoft 365 -ryhmään liittyvät uudet käyttäjät saavat tervetulosähköpostiviestin, jos UnifiedGroupWelcomeMessageEnabled-ominaisuus on True.

Jos haluat poistaa tervetuloviestin käytöstä, käytä seuraavaa [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) -komentoa:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
