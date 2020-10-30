---
title: Ongelman ratkaiseminen tuntematon käyttäjä Teamsissa-keskustelussa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003807"
- "6809"
ms.openlocfilehash: 523c11cb9d5c4696703c67c2a6b3184f5d12f8e7
ms.sourcegitcommit: d151b09064df3fb573ae07a387a08d98a9553b9b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807455"
---
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a><span data-ttu-id="eefb1-102">Ongelman ratkaiseminen teamsin keskustelu ohjelmassa tuntematon käyttäjä</span><span class="sxs-lookup"><span data-stu-id="eefb1-102">Resolving issue with "Unknown User" in Teams Chat</span></span>

<span data-ttu-id="eefb1-103">Toisinaan poistettu käyttäjä näkyy tuntematon käyttäjä-muodossa.</span><span class="sxs-lookup"><span data-stu-id="eefb1-103">At times, a removed user will appear as "Unknown User".</span></span> <span data-ttu-id="eefb1-104">Tämä on [tunnettu ongelma](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span><span class="sxs-lookup"><span data-stu-id="eefb1-104">This is a [known issue](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span></span>

<span data-ttu-id="eefb1-105">Jos käyttäjä näkee käyttäjät jatkuvasti, jotka näkyvät "tuntemattomana käyttäjänä" teamsin keskusteluissa, yritä tyhjentää väli muisti:</span><span class="sxs-lookup"><span data-stu-id="eefb1-105">If you are persistently seeing users showing as "Unknown User" in Teams chats, try and clear the cache:</span></span>

1.  <span data-ttu-id="eefb1-106">Napsauta tehtävä palkin tiimit-kuvaketta hiiren kakkos painikkeella.</span><span class="sxs-lookup"><span data-stu-id="eefb1-106">Right-click the Teams icon in the taskbar.</span></span> <span data-ttu-id="eefb1-107">Valitse  **Lopeta** .</span><span class="sxs-lookup"><span data-stu-id="eefb1-107">Click  **Quit** .</span></span>
2.  <span data-ttu-id="eefb1-108">Siirry tieto koneen%appdata%\Microsoft\teams\-kansioon ja poista kaikki kyseisen hakemiston tiedostot.</span><span class="sxs-lookup"><span data-stu-id="eefb1-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>

<span data-ttu-id="eefb1-109">Voit estää anonyymejä käyttäjiä liittymästä koko ukseen varmistamalla, että he odottavat odotus tilassa.</span><span class="sxs-lookup"><span data-stu-id="eefb1-109">You can prevent anonymous users from joining meetings by ensuring that they wait in the lobby.</span></span> <span data-ttu-id="eefb1-110">Lisä tietoja on Ohje aiheessa [teamsin koko uksen osallistuja-asetusten muuttaminen](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span><span class="sxs-lookup"><span data-stu-id="eefb1-110">For more information, see [Change participant settings for a Teams meeting](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span></span>
