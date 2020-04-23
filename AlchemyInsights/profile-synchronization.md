---
title: Profiilin synkronointi
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768110"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="54729-102">Milloin profiilini muutokset synkronoidaan SharePoint-käyttäjäprofiilisovellukseen?</span><span class="sxs-lookup"><span data-stu-id="54729-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="54729-103">SharePoint Online tuo käyttäjät ja ryhmät käyttäjäprofiilisovellukseen Active Directoryn tuonnin ajastintyön (AD-tuonti) avulla.</span><span class="sxs-lookup"><span data-stu-id="54729-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="54729-104">AD-tuonti synkronoi sharepoint online -hakemistosäilön muutokset käyttäjäprofiilisovellukseen.</span><span class="sxs-lookup"><span data-stu-id="54729-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="54729-105">Nämä muutokset käsitellään erissä.</span><span class="sxs-lookup"><span data-stu-id="54729-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="54729-106">Ajastintyö suoritetaan, kunnes muutokset synkronoidaan.</span><span class="sxs-lookup"><span data-stu-id="54729-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="54729-107">Työn suorittamiseen kuluu aikaa, joka riippuu prosessiin tehtyjen muutosten määrästä.</span><span class="sxs-lookup"><span data-stu-id="54729-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="54729-108">Suuri määrä muutoksia kestää kauemmin.</span><span class="sxs-lookup"><span data-stu-id="54729-108">A large number of changes takes longer.</span></span> <span data-ttu-id="54729-109">Palvelutasosopimuksen (SLA) mukaan SharePoint Online -hakemiston käyttäjän muutos näkyy käyttäjäprofiilisovelluksessa 24 tunnin kuluttua.</span><span class="sxs-lookup"><span data-stu-id="54729-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="54729-110">Lisätietoja käyttäjäprofiilin synkronoinnista SharePoint Onlinessa</span><span class="sxs-lookup"><span data-stu-id="54729-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

