---
title: SharePoint-sivuston luominen
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802963"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="2715c-102">SharePoint-sivuston luominen</span><span class="sxs-lookup"><span data-stu-id="2715c-102">Create a SharePoint site</span></span>

<span data-ttu-id="2715c-103">Voit tarkastella tietoja SharePoint-sivuston luomisen seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="2715c-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="2715c-104">[Uusi SharePoint-hallintakeskukseen sivustojen hallinta](https://docs.microsoft.com/sharepoint/manage-site-creation): sivuston luonnin asetukset, kuten luoda perinteisen sivuston tai ryhmien sivusto, joka ei sisällä Office 365-ryhmän tietoja.</span><span class="sxs-lookup"><span data-stu-id="2715c-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="2715c-105">[Luo SharePoint-ryhmäsivuston](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Opi luomaan ryhmäsivustossa.</span><span class="sxs-lookup"><span data-stu-id="2715c-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="2715c-106">[Luo SharePoint Online-sivuston tietoliikenne](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Opi luomaan communications-sivustoon.</span><span class="sxs-lookup"><span data-stu-id="2715c-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="2715c-107">[Uusi SharePoint-hallintakeskukseen sivustojen hallinta](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Opi luoda perinteisen sivuston tai ryhmäsivuston, joka ei sisällä Office 365-ryhmä.</span><span class="sxs-lookup"><span data-stu-id="2715c-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Vinkkejä]
> - <span data-ttu-id="2715c-109">Et voi luoda sivuston aiemmin luotuun sivustoon samaa URL-Osoitetta.</span><span class="sxs-lookup"><span data-stu-id="2715c-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="2715c-110">Poistettu sivuston ja haluavat käyttää URL-Osoitetta uudelleen, jos on mahdollista poistettu sivustosta on **poistettu sivustojen**alle.</span><span class="sxs-lookup"><span data-stu-id="2715c-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="2715c-111">Voit hallita poistetaan Katso sivustot, [poistaa sivuston](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="2715c-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="2715c-112">PowerShellin sivuston poistaminen kokonaan, on esimerkki [Poista SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet-komennolla.</span><span class="sxs-lookup"><span data-stu-id="2715c-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="2715c-113">Jotkin käyttäjät eivät välttämättä pysty luomaan sivuston.</span><span class="sxs-lookup"><span data-stu-id="2715c-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="2715c-114">[Hallitse sivuston luominen SharePoint Online-](https://docs.microsoft.com/sharepoint/manage-site-creation)kohdassa.</span><span class="sxs-lookup"><span data-stu-id="2715c-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="2715c-115">On mahdollista, sivusto näkyy odotettua kauemmin **luominen** on jumissa.</span><span class="sxs-lookup"><span data-stu-id="2715c-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="2715c-116">Jos on kulunut yli 24 tuntia näit tämän ongelman, kirjaudu support ticket.</span><span class="sxs-lookup"><span data-stu-id="2715c-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="2715c-117">Monissa tapauksissa olemme jo käsittelet ratkaisua.</span><span class="sxs-lookup"><span data-stu-id="2715c-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="2715c-118">Antakaa meille vähintään 24 tuntia ratkaisua.</span><span class="sxs-lookup"><span data-stu-id="2715c-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="2715c-119">Jos haluat luoda uuden työryhmäsivuston, joka ei sisällä Office 365-ryhmässä</span><span class="sxs-lookup"><span data-stu-id="2715c-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


