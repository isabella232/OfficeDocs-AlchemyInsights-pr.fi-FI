---
title: Profiilin synkronoinnin
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371981"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="f80ff-102">Kun profiiliin tehtyjä muutoksia synkronointi SharePoint käyttäjäprofiilisovellus?</span><span class="sxs-lookup"><span data-stu-id="f80ff-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="f80ff-103">SharePoint Online käyttää Active Directoryn tuo ajastintyö (AD tuonti) käyttäjien ja ryhmien tuominen käyttäjäprofiilisovellus.</span><span class="sxs-lookup"><span data-stu-id="f80ff-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="f80ff-104">AD tuo Synkronoi muutokset SharePoint Online kauppa Directory käyttäjäprofiilisovellus.</span><span class="sxs-lookup"><span data-stu-id="f80ff-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="f80ff-105">Muutokset käsitellään erissä.</span><span class="sxs-lookup"><span data-stu-id="f80ff-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="f80ff-106">Ajastintyö suoritetaan, kunnes muutokset on synkronoitu.</span><span class="sxs-lookup"><span data-stu-id="f80ff-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="f80ff-107">Työn suorittamiseen kuluva aika riippuu määrä käsitellä muutokset.</span><span class="sxs-lookup"><span data-stu-id="f80ff-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="f80ff-108">Muutoksia on paljon hitaampaa.</span><span class="sxs-lookup"><span data-stu-id="f80ff-108">A large number of changes takes longer.</span></span> <span data-ttu-id="f80ff-109">Palvelun tason sopimus (SLA) ilmoittaa, että käyttäjän SharePoint Online Directory muutos heijastuu käyttäjäprofiilisovellus 24 tunnin aikana.</span><span class="sxs-lookup"><span data-stu-id="f80ff-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="f80ff-110">Lisätietoja käyttäjäprofiilin synkronointia SharePoint Online-tietoja</span><span class="sxs-lookup"><span data-stu-id="f80ff-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

