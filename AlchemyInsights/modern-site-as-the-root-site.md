---
title: Kuin pääsivusto nykyaikaisia sivusto
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057703"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="de011-102">Kuin pääsivusto nykyaikaisia sivusto</span><span class="sxs-lookup"><span data-stu-id="de011-102">Modern site as root site</span></span>

<span data-ttu-id="de011-103">[Target-Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) asiakkaat voivat nyt saada niiden SharePoint-vuokralaisen classic pääsivusto, nykyaikaisen viestinnän sivuston kokemus.</span><span class="sxs-lookup"><span data-stu-id="de011-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="de011-104">Tämä ominaisuus voidaan ottaa käyttöön suorittamalla yksinkertainen PowerShell-cmdlet-komennolla.</span><span class="sxs-lookup"><span data-stu-id="de011-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="de011-105">PowerShell-command(s) onnistuneen toteuttamisen pääsivusto on uusi viestintä-sivuston kotisivun.</span><span class="sxs-lookup"><span data-stu-id="de011-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="de011-106">Lisätietoja PowerShellin cmdlet-komennolla ja ominaisuus vaatimukset ovat käytettävissä artikkelin [Ota-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="de011-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="de011-107">Olemme olla vähitellen liikkuvan, tämä off oletusarvoisesti aikaisin toukokuussa 2019, kohdistettu versio asiakkaille ja ulos koonnissa on käytettävissä maailmanlaajuisesti 2019 kesäkuun loppuun mennessä.</span><span class="sxs-lookup"><span data-stu-id="de011-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="de011-108">Lisätietoja [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for muita uusia ominaisuuksia on Moderni edelleen.</span><span class="sxs-lookup"><span data-stu-id="de011-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="de011-109">**Tärkeää**: Älä poista perinteinen pääsivusto luoda Nykyaikainen Viestimissivusto.</span><span class="sxs-lookup"><span data-stu-id="de011-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="de011-110">Microsoft ei tue.</span><span class="sxs-lookup"><span data-stu-id="de011-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="de011-111">Ensisijaisen säilön poistaminen tekee kaikki SharePoint-sivustot organisaation kaikkien käyttäjien käytettävissä ennen kuin palauttaa sivuston tai luoda uuden sivuston samaan URL-osoitteeseen.</span><span class="sxs-lookup"><span data-stu-id="de011-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 