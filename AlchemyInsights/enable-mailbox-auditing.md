---
title: Ota käyttöön posti laatikon valvonta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736250"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="d8559-102">Ota käyttöön posti laatikon valvonta</span><span class="sxs-lookup"><span data-stu-id="d8559-102">Enable mailbox auditing</span></span>

<span data-ttu-id="d8559-103">Jos haluat ottaa posti laatikon valvonnan käyttöön joko yksittäisessä tai koko organisaatiossa, seuraavat cmdlet-komennot on suoritettava Etävirralla:</span><span class="sxs-lookup"><span data-stu-id="d8559-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="d8559-104">**Yksittäinen käyttäjä**</span><span class="sxs-lookup"><span data-stu-id="d8559-104">**Single User**</span></span>
  
<span data-ttu-id="d8559-105">Set-posti laatikko-identiteetti "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="d8559-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="d8559-106">**Organisaatio**</span><span class="sxs-lookup"><span data-stu-id="d8559-106">**Organization**</span></span>
  
<span data-ttu-id="d8559-107">Get-posti laatikko-ResultSize Unlimited-suodatin {Vastaanottaenttypedetails-EQ "Userposti laatikko"} | Aseta-posti laatikko-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="d8559-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="d8559-108">Opi lisää</span><span class="sxs-lookup"><span data-stu-id="d8559-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

