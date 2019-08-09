---
title: SharePoint-sivuston luominen
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ad1a77b69d2d453dbd3daa304759238b329f96ba
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269913"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="a37dc-102">SharePoint-sivuston luominen</span><span class="sxs-lookup"><span data-stu-id="a37dc-102">Create a SharePoint site</span></span>

<span data-ttu-id="a37dc-103">Voit tarkastella tietoja SharePoint-sivuston luomisen seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="a37dc-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="a37dc-104">[Uusi SharePoint-hallintakeskukseen sivustojen hallinta](https://docs.microsoft.com/sharepoint/manage-site-creation): sivuston luonnin asetukset, kuten luoda perinteisen sivuston tai ryhmien sivusto, joka ei sisällä Office 365-ryhmän tietoja.</span><span class="sxs-lookup"><span data-stu-id="a37dc-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="a37dc-105">[Luo SharePoint-ryhmäsivuston](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Opi luomaan ryhmäsivustossa.</span><span class="sxs-lookup"><span data-stu-id="a37dc-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="a37dc-106">[Luo SharePoint Online-sivuston tietoliikenne](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Opi luomaan communications-sivustoon.</span><span class="sxs-lookup"><span data-stu-id="a37dc-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="a37dc-107">[Uusi SharePoint-hallintakeskukseen sivustojen hallinta](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Opi luoda perinteisen sivuston tai ryhmäsivuston, joka ei sisällä Office 365-ryhmä.</span><span class="sxs-lookup"><span data-stu-id="a37dc-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Vinkkejä]
> - <span data-ttu-id="a37dc-109">Et voi luoda sivuston aiemmin luotuun sivustoon samaa URL-Osoitetta.</span><span class="sxs-lookup"><span data-stu-id="a37dc-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="a37dc-110">Poistettu sivuston ja haluavat käyttää URL-Osoitetta uudelleen, jos on mahdollista poistettu sivustosta on **poistettu sivustojen**alle.</span><span class="sxs-lookup"><span data-stu-id="a37dc-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="a37dc-111">Voit hallita poistetaan Katso sivustot, [poistaa sivuston](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="a37dc-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="a37dc-112">PowerShellin sivuston poistaminen kokonaan, on esimerkki [Poista SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet-komennolla.</span><span class="sxs-lookup"><span data-stu-id="a37dc-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="a37dc-113">Jotkin käyttäjät eivät välttämättä pysty luomaan sivuston.</span><span class="sxs-lookup"><span data-stu-id="a37dc-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="a37dc-114">[Hallitse sivuston luominen SharePoint Online-](https://docs.microsoft.com/sharepoint/manage-site-creation)kohdassa.</span><span class="sxs-lookup"><span data-stu-id="a37dc-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="a37dc-115">On mahdollista, sivusto näkyy odotettua kauemmin **luominen** on jumissa.</span><span class="sxs-lookup"><span data-stu-id="a37dc-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="a37dc-116">Jos on kulunut yli 24 tuntia näit tämän ongelman, kirjaudu support ticket.</span><span class="sxs-lookup"><span data-stu-id="a37dc-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="a37dc-117">Monissa tapauksissa olemme jo käsittelet ratkaisua.</span><span class="sxs-lookup"><span data-stu-id="a37dc-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="a37dc-118">Antakaa meille vähintään 24 tuntia ratkaisua.</span><span class="sxs-lookup"><span data-stu-id="a37dc-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="a37dc-119">Jos haluat luoda uuden työryhmäsivuston, joka ei sisällä Office 365-ryhmässä</span><span class="sxs-lookup"><span data-stu-id="a37dc-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


