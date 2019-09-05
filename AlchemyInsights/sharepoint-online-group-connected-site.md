---
title: Ryhmän lisääminen SharePoint-sivustoon
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750517"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="fdd1b-102">Ongelmia luotaessa tai ryhmittäessä yhdistettyjä sivustoja SharePoint Onlinessa</span><span class="sxs-lookup"><span data-stu-id="fdd1b-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="fdd1b-103">Ryhmän yhdistettyä sivustoa luotaessa tai luotaessa uudelleen on ilmennyt muutamia yleisiä ongelmia.</span><span class="sxs-lookup"><span data-stu-id="fdd1b-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="fdd1b-104">Jos olet poistanut ryhmän ja sen yhdistetyn sivuston ja haluat luoda toisen sivuston, jolla on sama URL-osoite, sinun on poistettava edellinen sivusto pysyvästi.</span><span class="sxs-lookup"><span data-stu-id="fdd1b-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="fdd1b-105">Lataa [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="fdd1b-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="fdd1b-106">Lisä tietoja PowerShellin käytön aloittamisesta on Ohje aiheessa [SharePointin online-hallinta liittymän käytön](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) aloittaminen</span><span class="sxs-lookup"><span data-stu-id="fdd1b-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="fdd1b-107">Poista sivusto poistetut sivustot käyttämällä [Poista-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="fdd1b-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="fdd1b-108">Jos olet luomassa ryhmä liitettyä sivustoa ja saat varoituksen, toinen samanniminen ryhmä on jo olemassa, Tarkista nykyiset ryhmät [Office 365-sivustosta hallinta keskuksesta](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="fdd1b-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="fdd1b-109">Voit ratkaista ongelman poistamalla aiemmin luodun ryhmän, jos sitä ei enää tarvita, tai luomalla sivuston, jossa on eri alias määritetty.</span><span class="sxs-lookup"><span data-stu-id="fdd1b-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="fdd1b-110">On olemassa erilaisia tapoja luoda ja käyttää nykyaikaisia SharePoint-ryhmiä.</span><span class="sxs-lookup"><span data-stu-id="fdd1b-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="fdd1b-111">Voit yhdistää aiemmin luotuja sivustoja Office 365-ryhmään.</span><span class="sxs-lookup"><span data-stu-id="fdd1b-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="fdd1b-112">Lisä tietoja on Ohje aiheessa [Office 365-ryhmän yhdistäminen SharePoint-käyttäjän Interface-toiminnolla](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="fdd1b-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="fdd1b-113">Jos haluat luoda Office 365-ryhmään liitetyn sivuston, sinun on luotava Ryhmäsivusto.</span><span class="sxs-lookup"><span data-stu-id="fdd1b-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="fdd1b-114">Lisä tietoja on kohdassa [ryhmäsivuston luominen SharePointissa](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="fdd1b-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

