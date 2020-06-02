---
title: Palauta poistetut kohteet cmdlet-otoksella
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493026"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="2b903-102">Palauta poistetut kohteet cmdlet-otoksella</span><span class="sxs-lookup"><span data-stu-id="2b903-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="2b903-103">[Get-RecoverableItems-cmdlet-toiminnolla](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) voit tarkastella postilaatikoiden poistettuja kohteita.</span><span class="sxs-lookup"><span data-stu-id="2b903-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="2b903-104">Kun olet löytänyt poistetut kohteet, palauta ne [Restore-RecoverableItems-cmdlet-toiminnolla.](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="2b903-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="2b903-105">Katso täydelliset tiedot [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="2b903-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="2b903-106">Postilaatikon tuonnin vientirooli on määritettävä, ennen kuin voit suorittaa tämän cmdlet-otoksen.</span><span class="sxs-lookup"><span data-stu-id="2b903-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="2b903-107">Lisätietoja on kohdassa [Get-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="2b903-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
