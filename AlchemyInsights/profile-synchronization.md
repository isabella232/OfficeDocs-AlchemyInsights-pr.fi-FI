---
title: Profiilin synkronointi
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801766"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="2388a-102">Milloin profiilini muuttuu synkronoituna SharePoint-käyttäjä profiili sovellukseen?</span><span class="sxs-lookup"><span data-stu-id="2388a-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="2388a-103">SharePoint Online tuo käyttäjät ja ryhmät käyttäjä profiili sovellukseen Active Directoryn Import-ajastin työn (AD Import) avulla.</span><span class="sxs-lookup"><span data-stu-id="2388a-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="2388a-104">MAINOSTEN tuonti Synkronoi SharePoint Online-hakemisto kaupan muutokset käyttäjä profiili sovellukseen.</span><span class="sxs-lookup"><span data-stu-id="2388a-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="2388a-105">Nämä muutokset käsitellään erissä.</span><span class="sxs-lookup"><span data-stu-id="2388a-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="2388a-106">Ajastin työ suoritetaan, kunnes muutokset on synkronoitu.</span><span class="sxs-lookup"><span data-stu-id="2388a-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="2388a-107">Aika, jona työ suoritetaan, määräytyy prosessi muutosten luku määrän mukaan.</span><span class="sxs-lookup"><span data-stu-id="2388a-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="2388a-108">Suuri määrä muutoksia kestää kauemmin.</span><span class="sxs-lookup"><span data-stu-id="2388a-108">A large number of changes takes longer.</span></span> <span data-ttu-id="2388a-109">Palvelu taso sopimus (SLA) toteaa, että SharePoint Online-hakemiston käyttäjän muutos näkyy käyttäjä profiili sovelluksessa 24 tunnin kuluttua.</span><span class="sxs-lookup"><span data-stu-id="2388a-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="2388a-110">Lisä tietoja käyttäjä profiilien synkronoinnista SharePoint Onlinessa</span><span class="sxs-lookup"><span data-stu-id="2388a-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

