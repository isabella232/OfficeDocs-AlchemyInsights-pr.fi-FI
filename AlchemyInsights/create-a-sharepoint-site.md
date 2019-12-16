---
title: SharePoint-sivuston luominen
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 2611c3ed9cfe78c82c9b123ea26b6fe8f951b458
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049874"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="2a884-102">SharePoint-sivuston luominen</span><span class="sxs-lookup"><span data-stu-id="2a884-102">Create a SharePoint site</span></span>

<span data-ttu-id="2a884-103">Voit tarkastella SharePoint-sivuston luomista koskevia tietoja seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="2a884-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="2a884-104">[Hallitse sivustoja uudessa SharePointin hallinta keskuksessa](https://docs.microsoft.com/sharepoint/manage-site-creation): tietoja sivuston luonti vaihtoehdoista, kuten siitä, miten luodaan perinteinen sivusto tai teams-sivusto, joka ei sisällä Office 365-ryhmää.</span><span class="sxs-lookup"><span data-stu-id="2a884-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="2a884-105">[Ryhmäsivuston luominen SharePointissa](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Opi luomaan Ryhmäsivusto.</span><span class="sxs-lookup"><span data-stu-id="2a884-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="2a884-106">[Viestintä sivuston luominen SharePoint Onlinessa](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Opi luomaan viestintä sivusto.</span><span class="sxs-lookup"><span data-stu-id="2a884-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="2a884-107">[Hallitse sivustoja uudessa SharePointin hallinta keskuksessa](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Opi luomaan perinteinen sivusto tai ryhmäsivusto, joka ei sisällä Office 365-ryhmää.</span><span class="sxs-lookup"><span data-stu-id="2a884-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
<span data-ttu-id="2a884-108">**Vihjeitä:**</span><span class="sxs-lookup"><span data-stu-id="2a884-108">**Tips:**</span></span>
- <span data-ttu-id="2a884-109">Et voi luoda sivustoa, jolla on sama URL-osoite aiemmin luodusta sivustosta.</span><span class="sxs-lookup"><span data-stu-id="2a884-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="2a884-110">Jos poistit sivuston ja haluat käyttää URL-osoitetta uudelleen, on mahdollista, että poistettu sivusto on edelleen olemassa **Poistetut sivustot**-kohdassa.</span><span class="sxs-lookup"><span data-stu-id="2a884-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="2a884-111">Jos haluat hallita poistettuja sivustoja, Katso, [Poista sivusto](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="2a884-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="2a884-112">Jos haluat poistaa sivuston kokonaan PowerShellin avulla, Katso esimerkki [Poista SPSite-cmdlet-komennosta](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="2a884-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="2a884-113">Jotkut käyttäjät eivät ehkä voi luoda sivustoa.</span><span class="sxs-lookup"><span data-stu-id="2a884-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="2a884-114">Katso [sivuston luomisen hallinta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="2a884-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="2a884-115">On mahdollista, että sivusto näyttää juuttuneen **luomaan** odotettua pidempään.</span><span class="sxs-lookup"><span data-stu-id="2a884-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="2a884-116">Jos tämän ongelman ensimmäisen näkemis kerran jälkeen on kulunut yli 24 tuntia, kirjaudu tuki lippuun.</span><span class="sxs-lookup"><span data-stu-id="2a884-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="2a884-117">Monissa tapa uksissa olemme jo tekemässä ratkaisua.</span><span class="sxs-lookup"><span data-stu-id="2a884-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="2a884-118">Ole hyvä ja anna meille vähintään 24 tuntia aikaa ratkaisun suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="2a884-118">Please give us at least 24 hours to complete a solution.</span></span>
- <span data-ttu-id="2a884-119">Jos sinun on luotava uusi ryhmäsivusto, joka ei sisällä Office 365-ryhmää,</span><span class="sxs-lookup"><span data-stu-id="2a884-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


