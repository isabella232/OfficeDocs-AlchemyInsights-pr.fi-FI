---
title: Ryhmän lisääminen SharePoint-sivustoon
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770348"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="e2508-102">Ongelmia luotaessa ryhmä yhdistettyä sivustoa SharePointissa</span><span class="sxs-lookup"><span data-stu-id="e2508-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="e2508-103">Joitakin yleisiä ongelmia, joita ilmeni luotaessa tai luotaessa uudelleen ryhmän yhdistettyä sivustoa.</span><span class="sxs-lookup"><span data-stu-id="e2508-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="e2508-104">Jos olet poistanut ryhmän ja sen yhdistetyn sivuston ja haluat luoda toisen sivuston, jolla on sama URL-osoite, sinun on poistettava edellinen sivusto pysyvästi.</span><span class="sxs-lookup"><span data-stu-id="e2508-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="e2508-105">Lataa [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="e2508-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="e2508-106">Lisä tietoja PowerShellin käytön aloittamisesta on Ohje aiheessa [SharePoint Onlinen hallinta liittymän käytön](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)aloittaminen.</span><span class="sxs-lookup"><span data-stu-id="e2508-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="e2508-107">Poista sivusto poistetut sivustot käyttämällä [Poista-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="e2508-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="e2508-108">PowerShell on pakollinen poistamaan ryhmä sivustoja pysyvästi.</span><span class="sxs-lookup"><span data-stu-id="e2508-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="e2508-109">Jos olet luomassa ryhmä liitettyä sivustoa ja saat varoituksen: **toinen samanniminen ryhmä on jo olemassa**, tarkista olemassa olevat ryhmät [Office 365-sivustosta hallinta keskuksesta](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="e2508-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="e2508-110">Voit ratkaista ongelman poistamalla aiemmin luodun ryhmän, jos sitä ei enää tarvita, tai luomalla sivuston, jossa on eri alias määritetty.</span><span class="sxs-lookup"><span data-stu-id="e2508-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="e2508-111">On olemassa erilaisia tapoja luoda ja käyttää nykyaikaisia SharePoint-ryhmiä.</span><span class="sxs-lookup"><span data-stu-id="e2508-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="e2508-112">Voit yhdistää aiemmin luotuja sivustoja Office 365-ryhmään.</span><span class="sxs-lookup"><span data-stu-id="e2508-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="e2508-113">Lisä tietoja on Ohje aiheessa [Office 365-ryhmän yhdistäminen SharePoint-käyttö liittymän avulla](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="e2508-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="e2508-114">Jos haluat luoda Office 365-ryhmään liitetyn sivuston, sinun on luotava [ryhmäsivusto](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="e2508-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
