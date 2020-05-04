---
title: Mikroviiveet tai rajoittaminen Exchange Online PowerShellissä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947832"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="36806-102">Mikroviiveet tai rajoittaminen Exchange Online PowerShellissä</span><span class="sxs-lookup"><span data-stu-id="36806-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="36806-103">Kun suoritat Exchange Onlinessa komentosarjoja ja cmdlet-komentoja, saatat huomata viiveitä tai nähdä Mikroviive käytetty -varoituksen.</span><span class="sxs-lookup"><span data-stu-id="36806-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="36806-104">Seuraavassa on kaksi tähän liittyvää ehdotusta:</span><span class="sxs-lookup"><span data-stu-id="36806-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="36806-105">Sinun kannattaa ehkä kokeilla [Exchange Online v2 PowerShell -moduulia](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), joka sisältää REST-ohjelmointirajapintaan perustuvia, paljon paremmin toimivia CMDlet-komentoja.</span><span class="sxs-lookup"><span data-stu-id="36806-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="36806-106">Tämä voi olla hyvä ratkaisu monille usein käytettäville Get-CMDlet-komennoille.</span><span class="sxs-lookup"><span data-stu-id="36806-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="36806-107">Jos haluat käyttää CMDlet-komentoja, joita v2-moduuli ei kata vielä, tutustu artikkeliin [PowerShell cmdlet -komentojen suorittaminen suurille käyttäjämäärille Office 365:ssä](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), jossa kerrotaan, miten odotetut PowerShellin rajoitukset voidaan kiertää Exchange Onlinessa.</span><span class="sxs-lookup"><span data-stu-id="36806-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
