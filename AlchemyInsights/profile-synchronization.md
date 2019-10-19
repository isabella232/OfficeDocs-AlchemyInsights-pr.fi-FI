---
title: Profiilin synkronointi
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554330"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="c290c-102">Milloin profiilini muutokset synkronoidaan SharePoint-käyttäjä profiili sovellukseen?</span><span class="sxs-lookup"><span data-stu-id="c290c-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="c290c-103">SharePoint Online käyttää Active Directoryn tuonti ajastin työtä (mainoksen tuonti) käyttäjien ja ryhmien tuomiseen käyttäjä profiili sovellukseen.</span><span class="sxs-lookup"><span data-stu-id="c290c-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="c290c-104">MAINOKSEN tuonti synkronoi muutokset SharePoint Online-hakemisto säilöstä käyttäjä profiili sovellukseen.</span><span class="sxs-lookup"><span data-stu-id="c290c-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="c290c-105">Nämä muutokset käsitellään erissä.</span><span class="sxs-lookup"><span data-stu-id="c290c-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="c290c-106">Ajastin työtä suoritetaan, kunnes muutokset on synkronoitu.</span><span class="sxs-lookup"><span data-stu-id="c290c-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="c290c-107">Aika, joka kuluu työn suorittamiseen, määräytyy prosessin muutosten määrän mukaan.</span><span class="sxs-lookup"><span data-stu-id="c290c-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="c290c-108">Suuri määrä muutoksia kestää kauemmin.</span><span class="sxs-lookup"><span data-stu-id="c290c-108">A large number of changes takes longer.</span></span> <span data-ttu-id="c290c-109">Palvelu taso sopimuksessa (SLA) todetaan, että SharePoint Online-hakemiston käyttäjän muutos näkyy käyttäjä profiili sovelluksessa 24 tunnin kuluessa.</span><span class="sxs-lookup"><span data-stu-id="c290c-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="c290c-110">Lisä tietoja käyttäjä profiilien synkronoinnista SharePoint Onlinessa</span><span class="sxs-lookup"><span data-stu-id="c290c-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

