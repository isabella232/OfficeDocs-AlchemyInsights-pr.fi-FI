---
title: Useat käyttäjät eivät näe apuosia Outlookissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197974"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="0337e-102">Useat käyttäjät eivät näe apuosia Outlookissa</span><span class="sxs-lookup"><span data-stu-id="0337e-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="0337e-103">Jos testaat Outlookin apuohjelmia, eikä mitään näy ensimmäisenä vianmääritysvaiheena, käytä **Get-OrganizationConfig** PowerShell -cmdlet-komentoa _AppsForOfficeEnabled-parametrin_ kyselyyn.</span><span class="sxs-lookup"><span data-stu-id="0337e-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="0337e-104">Jos kysely palauttaa arvon **False**, määritä tämän parametrin arvoksi **Tosi** **Set-OrganizationConfig-cmdlet-nännin** avulla, joten apuohjelmat näkyvät odotetulla tavalla.</span><span class="sxs-lookup"><span data-stu-id="0337e-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="0337e-105">Emme suosittele, että _AppsForOfficeEnabled-parametrin_ arvo on **False**.</span><span class="sxs-lookup"><span data-stu-id="0337e-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="0337e-106">**False-arvo** ohittaa kaikki edellä mainitut hallinta- ja käyttäjärooliasetukset ja estää organisaation käyttäjän aktivoimasta uusia sovelluksia.</span><span class="sxs-lookup"><span data-stu-id="0337e-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="0337e-107">Lisätietoja on [ohjeaiheessa Outlookin apuohjelmia asennettavien ja hallitsevien järjestelmänvalvojien ja käyttäjien määrittäminen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="0337e-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>