---
title: SharePoint-sivuston luominen
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770852"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="32513-102">SharePoint-sivuston luominen</span><span class="sxs-lookup"><span data-stu-id="32513-102">Create a SharePoint site</span></span>

<span data-ttu-id="32513-103">Luo tai Hallitse sivustoja SharePoint-hallinta keskuksen [aktiivisista sivustoista](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) .</span><span class="sxs-lookup"><span data-stu-id="32513-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="32513-104">Lisä tietoja on kohdassa [sivustojen hallinta uudessa SharePointin hallinta keskuksessa](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="32513-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="32513-105">Vinkkejä:</span><span class="sxs-lookup"><span data-stu-id="32513-105">Tips:</span></span>

- <span data-ttu-id="32513-106">Et **voi** luoda sivustoa, jolla on sama URL-osoite aiemmin luodusta sivustosta.</span><span class="sxs-lookup"><span data-stu-id="32513-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="32513-107">Jos poistit sivuston ja haluat käyttää URL-osoitetta uudelleen, on mahdollista, että poistettu sivusto on edelleen olemassa [Poistetut sivustot](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)-kohdassa.</span><span class="sxs-lookup"><span data-stu-id="32513-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="32513-108">Sivusto on poistettava pysyvästi URL-osoitteen uudelleenkäyttöä varten.</span><span class="sxs-lookup"><span data-stu-id="32513-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="32513-109">Jos haluat poistaa sivuston kokonaan PowerShellin avulla, Katso esimerkki [Poista SPSite-cmdlet-komennosta](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="32513-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="32513-110">Jotkut käyttäjät eivät ehkä voi luoda sivustoa.</span><span class="sxs-lookup"><span data-stu-id="32513-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="32513-111">[Katso sivuston luomisen hallinta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="32513-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="32513-112">On mahdollista, että sivusto näyttää juuttuneen **luomaan** odotettua pidempään.</span><span class="sxs-lookup"><span data-stu-id="32513-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="32513-113">Jos tämän ongelman ensimmäisen näkemis kerran jälkeen on kulunut yli 24 tuntia, kirjaudu tuki lippuun.</span><span class="sxs-lookup"><span data-stu-id="32513-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="32513-114">Monissa tapa uksissa olemme jo tekemässä ratkaisua.</span><span class="sxs-lookup"><span data-stu-id="32513-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="32513-115">Ole hyvä ja anna meille vähintään 24 tuntia aikaa ratkaisun suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="32513-115">Please give us at least 24 hours to complete a solution.</span></span>
