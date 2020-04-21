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
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="3ee73-102">SharePoint-sivuston luominen</span><span class="sxs-lookup"><span data-stu-id="3ee73-102">Create a SharePoint site</span></span>

<span data-ttu-id="3ee73-103">Luo tai hallitse SharePoint-hallintakeskuksen [aktiivisten sivustojen](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) sivustoja.</span><span class="sxs-lookup"><span data-stu-id="3ee73-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="3ee73-104">Lisätietoja on [ohjeaiheessa Uuden SharePoint-hallintakeskuksen sivustojen hallinta](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="3ee73-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="3ee73-105">Vinkkejä:</span><span class="sxs-lookup"><span data-stu-id="3ee73-105">Tips:</span></span>

- <span data-ttu-id="3ee73-106">Sivustoa, jolla on sama URL-osoite aiemmin luodussa sivustossa, **ei voi** luoda.</span><span class="sxs-lookup"><span data-stu-id="3ee73-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="3ee73-107">Jos olet poistanut sivuston ja haluat käyttää URL-osoitetta uudelleen, poistettu sivusto on mahdollisesti edelleen [Olemassa Poistetut sivustot](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)-kohdassa.</span><span class="sxs-lookup"><span data-stu-id="3ee73-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="3ee73-108">Sivusto on poistettava pysyvästi, jotta URL-osoitetta voidaan käyttää uudelleen.</span><span class="sxs-lookup"><span data-stu-id="3ee73-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="3ee73-109">Jos haluat poistaa Powershell-sivuston kokonaan, katso [Poista-SPSite-cmdlet-esimerkki.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="3ee73-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="3ee73-110">Jotkin käyttäjät eivät ehkä pysty luomaan sivustoa.</span><span class="sxs-lookup"><span data-stu-id="3ee73-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="3ee73-111">[Lisätietoja on ohjeaiheessa Sivuston luomisen hallinta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="3ee73-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="3ee73-112">On mahdollista, että sivusto näkyy jumissa **luominen** odotettua kauemmin.</span><span class="sxs-lookup"><span data-stu-id="3ee73-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="3ee73-113">Jos tämän ongelman ensimmäisestä näkemästäsi on kulunut yli 24 tuntia, kirjaudu tukilipusta.</span><span class="sxs-lookup"><span data-stu-id="3ee73-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="3ee73-114">Monissa tapauksissa olemme jo työstänyt ratkaisua.</span><span class="sxs-lookup"><span data-stu-id="3ee73-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="3ee73-115">Anna meille vähintään 24 tuntia ratkaisun viimeistelemiseksi.</span><span class="sxs-lookup"><span data-stu-id="3ee73-115">Please give us at least 24 hours to complete a solution.</span></span>
