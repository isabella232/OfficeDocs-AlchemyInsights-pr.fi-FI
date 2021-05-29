---
title: Mikroviiveet tai rajoittaminen Exchange Online PowerShellissä
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702123"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="4d110-102">Mikroviiveet tai rajoittaminen Exchange Online PowerShellissä</span><span class="sxs-lookup"><span data-stu-id="4d110-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="4d110-103">Kun suoritat Exchange Onlinessa komentosarjoja ja cmdlet-komentoja, saatat huomata viiveitä tai nähdä Mikroviive käytetty -varoituksen.</span><span class="sxs-lookup"><span data-stu-id="4d110-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="4d110-104">Tässä on muutamia ehdotuksia, miten voit ratkaista ongelman:</span><span class="sxs-lookup"><span data-stu-id="4d110-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="4d110-105">Suorita vianmääritys, niin voit rentoutua vuokraajan PowerShellin throtling-käytännöistä.</span><span class="sxs-lookup"><span data-stu-id="4d110-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="4d110-106">Tämä ratkaisu ratkaisee ongelman useimmin.</span><span class="sxs-lookup"><span data-stu-id="4d110-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="4d110-107">Jos ongelma ei ratkea vieläkään, [käytä Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)-moduulia, joka sisältää REST-ohjelmointirajapintaan perustuvat CMDlet-komennot ja jotka toimivat huomattavasti tehokkaammin.</span><span class="sxs-lookup"><span data-stu-id="4d110-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="4d110-108">Tämä voi olla hyvä ratkaisu monille usein käytettäville Get-CMDlet-komennoille.</span><span class="sxs-lookup"><span data-stu-id="4d110-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="4d110-109">Jos sinun on käytettävä CMDlet-komentoja, joita ei sisällytetä v2-moduuliin, katso [PowerShellin cmdlet-komentojen](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)käyttö suurille käyttäjille Office 365:ssä, jossa käsitellään PowerShellin rajoitusrajoitusten Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="4d110-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
