---
title: Julkisten kansioiden käytön hallinta Outlookin avulla
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
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816737"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="b78f6-102">Julkisten kansioiden käytön hallinta Outlookin avulla</span><span class="sxs-lookup"><span data-stu-id="b78f6-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="b78f6-103">Voit määrittää, k voivatko käyttäjät käyttää julkisia kansioita Outlookin avulla:</span><span class="sxs-lookup"><span data-stu-id="b78f6-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="b78f6-104">Käytä `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="b78f6-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="b78f6-105">$true: Salli käyttäjien käyttää julkisia kansioita Outlookissa</span><span class="sxs-lookup"><span data-stu-id="b78f6-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="b78f6-106">$false: Estä käyttäjien pääsy Yleisiin kansioihin Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="b78f6-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="b78f6-107">Tämä on oletusarvo.</span><span class="sxs-lookup"><span data-stu-id="b78f6-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="b78f6-108">Huomautus: Tässä menettelyssä voidaan hallita ainoastaan yhteyksiä Outlookin työpöytäversioon Windows-asiakassovellohjelmia varten.</span><span class="sxs-lookup"><span data-stu-id="b78f6-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="b78f6-109">Käyttäjät voivat edelleen käyttää julkisia kansioita OWA:n tai Outlook for Macin avulla.</span><span class="sxs-lookup"><span data-stu-id="b78f6-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="b78f6-110">Lisätietoja on kohdassa [Hallitut yhteydet yleisiin kansioihin Outlookissa.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="b78f6-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
