---
title: Postilaatikon valvonnan käyttöönottaaminen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429480"
---
# <a name="turn-on-mailbox-auditing"></a><span data-ttu-id="c7aee-102">Postilaatikon valvonnan käyttöönottaaminen</span><span class="sxs-lookup"><span data-stu-id="c7aee-102">Turn on mailbox auditing</span></span>

<span data-ttu-id="c7aee-103">Jos haluat ottaa postilaatikon valvonnan käyttöön yksittäiselle käyttäjälle tai koko organisaatiolle, suorita seuraavat cmdlet-komennot Etä-PowerShellistä:</span><span class="sxs-lookup"><span data-stu-id="c7aee-103">To turn on mailbox auditing for a single user or an entire organization, run the following cmdlets from Remote PowerShell:</span></span>

- <span data-ttu-id="c7aee-104">**Yksittäinen** käyttäjä: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="c7aee-104">**Single user**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
- <span data-ttu-id="c7aee-105">**Organisaatio:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled-$true</span><span class="sxs-lookup"><span data-stu-id="c7aee-105">**Organization**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>

<span data-ttu-id="c7aee-106">Lisätietoja on ohjeaiheessa [Postilaatikon valvonnan hallinta.](https://go.microsoft.com/fwlink/?linkid=2103668)</span><span class="sxs-lookup"><span data-stu-id="c7aee-106">To learn more, see [Manage mailbox auditing](https://go.microsoft.com/fwlink/?linkid=2103668).</span></span>