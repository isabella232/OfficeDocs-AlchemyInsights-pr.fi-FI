---
title: SharePoint-sivuston luominen
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786562"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="f0542-102">SharePoint-sivuston luominen</span><span class="sxs-lookup"><span data-stu-id="f0542-102">Create a SharePoint site</span></span>

<span data-ttu-id="f0542-103">SharePoint-hallinta keskuksen [aktiivisten alueiden](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) sivustokohteiden luominen tai hallinta.</span><span class="sxs-lookup"><span data-stu-id="f0542-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="f0542-104">Lisä tietoja on Ohje aiheessa [sivuston hallinta uudessa SharePoint-hallinta keskuksessa](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="f0542-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="f0542-105">Vinkkejä</span><span class="sxs-lookup"><span data-stu-id="f0542-105">Tips:</span></span>

- <span data-ttu-id="f0542-106">Et **voi** luoda sivustoa, jolla on sama URL-osoite olemassa olevalla sivustolla.</span><span class="sxs-lookup"><span data-stu-id="f0542-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="f0542-107">Jos poistit sivuston ja haluat käyttää URL-osoitetta uudelleen, poistettu sivusto on edelleen käytettävissä [Poistetut sivustot](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)-kohdassa.</span><span class="sxs-lookup"><span data-stu-id="f0542-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="f0542-108">Sivusto on poistettava pysyvästi, jotta URL-osoitetta voidaan käyttää uudelleen.</span><span class="sxs-lookup"><span data-stu-id="f0542-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="f0542-109">Jos haluat poistaa sivuston kokonaan PowerShellin avulla, Katso lisä tietoja artikkelista [Remove-SPSite-cmdlet-](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) esimerkki.</span><span class="sxs-lookup"><span data-stu-id="f0542-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="f0542-110">Jotkut käyttäjät eivät ehkä voi luoda sivustoa.</span><span class="sxs-lookup"><span data-stu-id="f0542-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="f0542-111">[Lisä tietoja on kohdassa sivuston luomisen hallinta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="f0542-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="f0542-112">On mahdollista, että sivusto on juuttunut odotettua **kauemmin.**</span><span class="sxs-lookup"><span data-stu-id="f0542-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="f0542-113">Jos sinulla on kulunut yli 24 tuntia siitä, kun olet ensimmäisen kerran nähnyt tämän ongelman, kirjaudu tuki lipulla.</span><span class="sxs-lookup"><span data-stu-id="f0542-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="f0542-114">Monissa tapa uksissa pyrimme jo ratkaisemaan ongelman.</span><span class="sxs-lookup"><span data-stu-id="f0542-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f0542-115">Anna meille vähintään 24 tuntia aikaa ratkaisun suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="f0542-115">Please give us at least 24 hours to complete a solution.</span></span>
