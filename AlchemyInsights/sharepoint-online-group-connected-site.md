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
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582808"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="79a80-102">Ongelmia luotaessa ryhmälle yhdistettyä sivustoa SharePointissa</span><span class="sxs-lookup"><span data-stu-id="79a80-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="79a80-103">Joitakin yleisiä ongelmia ilmeni luotaessa tai luotaessa uudelleen yhdistettyä ryhmää.</span><span class="sxs-lookup"><span data-stu-id="79a80-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="79a80-104">Jos olet poistanut ryhmän ja siihen liittyvän sivuston ja haluat luoda toisen sivuston, jolla on sama URL-osoite, sinun on poistettava edellinen sivusto pysyvästi.</span><span class="sxs-lookup"><span data-stu-id="79a80-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="79a80-105">Lataa [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="79a80-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="79a80-106">Lisätietoja Powershellin käytön aloittamisesta on ohjeaiheessa [SharePoint Online -hallintaliittymän käytön aloittaminen](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="79a80-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="79a80-107">Poista sivusto poistetuista sivustoista [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell -cmdlet-nännin avulla.</span><span class="sxs-lookup"><span data-stu-id="79a80-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="79a80-108">Ryhmäsivustojen poistaminen edellyttää Powershelliä.</span><span class="sxs-lookup"><span data-stu-id="79a80-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="79a80-109">Jos luot ryhmään yhdistettyä sivustoa ja saat varoituksen: **Toinen ryhmä, jolla on sama alias, on jo olemassa,** tarkista aiemmin luodut ryhmät [Microsoft 365 -hallintakeskuksesta](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="79a80-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="79a80-110">Voit ratkaista ongelman poistamalla aiemmin luodun ryhmän, jos sitä ei enää tarvita, tai luomalla sivuston, jossa on toinen alias määritettynä.</span><span class="sxs-lookup"><span data-stu-id="79a80-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="79a80-111">Voit luoda ja käyttää moderneja ryhmiä SharePointin kanssa eri tavoin.</span><span class="sxs-lookup"><span data-stu-id="79a80-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="79a80-112">Voit yhdistää aiemmin luodut sivustot Microsoft 365 -ryhmään.</span><span class="sxs-lookup"><span data-stu-id="79a80-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="79a80-113">Lisätietoja on [ohjeaiheessa Microsoft 365 -ryhmän yhdistäminen SharePoint-käyttöliittymän avulla](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="79a80-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="79a80-114">Jos haluat luoda Microsoft 365 -ryhmän yhdistetyn sivuston, sinun on luotava [ryhmäsivusto](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="79a80-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
