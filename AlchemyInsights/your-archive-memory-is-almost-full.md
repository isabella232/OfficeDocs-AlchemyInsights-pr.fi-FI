---
title: Arkistopostilaatikkosi on lähes täynnä
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974278"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="4f3a7-102">Arkistopostilaatikkosi on lähes täynnä</span><span class="sxs-lookup"><span data-stu-id="4f3a7-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="4f3a7-103">Jos käyttäjä saa varoituksen; **Arkistopostilaatikkosi on lähes** täynnä tai sinun on lisättävä arkistopostilaatikon kokoa, seuraavassa on joitain vinkkejä:</span><span class="sxs-lookup"><span data-stu-id="4f3a7-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="4f3a7-104">Jos käyttäjälle on määritetty Exchange Online -palvelupaketti 1, päivitä **Exchange Online -palvelupaketti 2** -käyttöoikeuteen ja suurenna kokoa 50 Gt:stä 100 Gt:ksi.</span><span class="sxs-lookup"><span data-stu-id="4f3a7-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="4f3a7-105">Jos käyttäjälle on jo määritetty jompikumpi seuraavista: Exchange Online -palvelupaketti **2** tai Exchange Online -palvelupaketti 1 ja Exchange Online Archiving -lisäosa, ota automaattinen arkistointi käyttöön alla olevia ohjeita noudattamalla:.</span><span class="sxs-lookup"><span data-stu-id="4f3a7-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="4f3a7-106">[Muodosta yhteys Exchange Online PowerShelliin.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="4f3a7-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="4f3a7-107">Suorita käyttäjälle seuraava komento:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="4f3a7-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="4f3a7-108">Varmista, että komento on otettu käyttöön käyttäjälle, toimimalla seuraavasti:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="4f3a7-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="4f3a7-109">Lisätietoja on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="4f3a7-109">For more information see:</span></span>

- [<span data-ttu-id="4f3a7-110"> Rajoittamattoman arkistoinnin ottaminen käyttöön – järjestelmänvalvojan ohje – Microsoft 365 :n | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="4f3a7-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="4f3a7-111">Exchange Onlinen rajoitukset – palvelukuvaukset | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="4f3a7-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="4f3a7-112">Toiseen liiketoimintasuunnitelmaan päivittäminen | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="4f3a7-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

