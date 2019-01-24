---
title: Profiilin synkronoinnin
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29468044"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="6d8a9-102">Kun profiiliin tehtyjä muutoksia synkronointi SharePoint käyttäjäprofiilisovellus?</span><span class="sxs-lookup"><span data-stu-id="6d8a9-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="6d8a9-103">SharePoint Online käyttää Active Directoryn tuo ajastintyö (AD tuonti) käyttäjien ja ryhmien tuominen käyttäjäprofiilisovellus.</span><span class="sxs-lookup"><span data-stu-id="6d8a9-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="6d8a9-p101">AD tuo Synkronoi muutokset SharePoint Online kauppa Directory käyttäjäprofiilisovellus. Muutokset käsitellään erissä.</span><span class="sxs-lookup"><span data-stu-id="6d8a9-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="6d8a9-106">Ajastintyö suoritetaan, kunnes muutokset on synkronoitu.</span><span class="sxs-lookup"><span data-stu-id="6d8a9-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="6d8a9-p102">Työn suorittamiseen kuluva aika riippuu määrä käsitellä muutokset. Muutoksia on paljon hitaampaa. Palvelun tason sopimus (SLA) ilmoittaa, että käyttäjän SharePoint Online Directory muutos heijastuu käyttäjäprofiilisovellus 24 tunnin aikana.</span><span class="sxs-lookup"><span data-stu-id="6d8a9-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="6d8a9-110">Lisätietoja käyttäjäprofiilin synkronointia SharePoint Online-tietoja</span><span class="sxs-lookup"><span data-stu-id="6d8a9-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

