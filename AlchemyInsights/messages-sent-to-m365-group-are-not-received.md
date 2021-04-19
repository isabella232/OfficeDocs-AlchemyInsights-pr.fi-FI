---
title: Kaikki jäsenet eivät saa Microsoft 365 -ryhmälle lähetettyjä viestejä
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 29adc5a7b8b74280cb3fcd6369dc4fc3a3e8e957
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823784"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="3b6f3-102">Kaikki jäsenet eivät saa Microsoft 365 -ryhmälle lähetettyjä viestejä</span><span class="sxs-lookup"><span data-stu-id="3b6f3-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="3b6f3-103">Varmista, että kaikki ryhmän jäsenet ovat valinneet sähköpostiviestien vastaanottamisen.</span><span class="sxs-lookup"><span data-stu-id="3b6f3-103">Ensure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="3b6f3-104">Katso [Seuraa ryhmää Outlookissa](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="3b6f3-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="3b6f3-105">Voit tarkistaa ryhmän sähköpostiviestit tilanneiden jäsenten tilan suorittamalla seuraavan komennon [EXO PowerShellissä](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true): </span><span class="sxs-lookup"><span data-stu-id="3b6f3-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="3b6f3-106">Määritä kaikki ryhmän jäsenet vastaanottamaan Microsoft 365 -ryhmälle lähetettyjä sähköpostiviestejä Saapuneet-kansioonsa suorittamalla seuraavan EXO PowerShell -komennon: </span><span class="sxs-lookup"><span data-stu-id="3b6f3-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

<span data-ttu-id="3b6f3-107">Esimerkkejä:</span><span class="sxs-lookup"><span data-stu-id="3b6f3-107">For example:</span></span>

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`