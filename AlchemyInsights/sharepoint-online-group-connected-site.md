---
title: Ryhmän lisääminen SharePoint-sivustoon
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758728"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="41c83-102">Ryhmän yhteydessä sivuston luominen SharePoint Onlinessa</span><span class="sxs-lookup"><span data-stu-id="41c83-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="41c83-103">Jakautuvat yleisten ongelmien yhteydessä luominen tai luominen uudelleen ryhmän sivusto havainnut pari.</span><span class="sxs-lookup"><span data-stu-id="41c83-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="41c83-104">Jos olet poistanut ryhmän ja sen yhteydessä sivuston ja haluat luoda toisen sivuston kanssa samaa URL-Osoitetta, sinun on poistaa pysyvästi Edellinen sivusto.</span><span class="sxs-lookup"><span data-stu-id="41c83-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="41c83-105">Lataa [SPO-hallintaliittymä](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="41c83-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="41c83-106">Katso lisätietoja aloittaminen powershell [aloittaminen SharePoint Online-hallintaliittymä](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="41c83-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="41c83-107">Sivuston poistaminen poistaa sivustot käyttämällä [Poista-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell-komentosovelmalla.</span><span class="sxs-lookup"><span data-stu-id="41c83-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="41c83-108">Jos luot ryhmän yhteydessä sivuston ja samaa tunnusta toiselle ryhmälle on jo varoituksen, tarkista [Office 365-hallintakeskukseen](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)olemassa olevat ryhmät.</span><span class="sxs-lookup"><span data-stu-id="41c83-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="41c83-109">Määritetty ratkaise ongelmaa, poista aiemmin luotu ryhmä, jos ei enää tarvita tai luo sivuston, jossa toinen alias.</span><span class="sxs-lookup"><span data-stu-id="41c83-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="41c83-110">Voit luoda ja käyttää SharePointin kanssa nykyaikaisen ryhmille eri tavoin.</span><span class="sxs-lookup"><span data-stu-id="41c83-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="41c83-111">Voit muodostaa yhteyden Office 365-ryhmän aiemmin luotuihin sivustoihin.</span><span class="sxs-lookup"><span data-stu-id="41c83-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="41c83-112">Lisätietoja Katso [yhteyden Office 365-ryhmälle, käyttämällä SharePoint-käyttäjä ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="41c83-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="41c83-113">Office 365-ryhmän yhteydessä sivuston luominen, sinun on luoda ryhmäsivuston.</span><span class="sxs-lookup"><span data-stu-id="41c83-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="41c83-114">Saat lisätietoja, [Luo SharePoint-ryhmäsivuston](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="41c83-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

