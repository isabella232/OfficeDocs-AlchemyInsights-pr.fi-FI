---
title: Teams-keskustelussa jaettuja tiedostoja ei voi käyttää
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 5290b1eea907fc5b785c20654d92467a4ed0af04
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51595608"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a><span data-ttu-id="abbbe-102">Teams-keskustelussa jaettuja tiedostoja ei voi käyttää</span><span class="sxs-lookup"><span data-stu-id="abbbe-102">Unable to access files shared in Teams chat</span></span>

<span data-ttu-id="abbbe-103">Microsoft Teamsissa käyttäjän keskusteluikkunassa jakamaa tiedostoa säilytetään automaattisesti jaetun käyttäjän OneDrive-sivustoon.</span><span class="sxs-lookup"><span data-stu-id="abbbe-103">In Microsoft Teams, a file shared by a user in a chat window is stored automatically on the sharing user's OneDrive site.</span></span>

<span data-ttu-id="abbbe-104">Kun toinen käyttäjä yrittää avata tiedoston Teamsissa ja näyttöön tulee virhesanoma "Sinulla ei ole tämän tiedoston käyttöoikeutta", ongelma ilmenee, koska Rajoitetun käyttöoikeuden lukittu tila -toiminto on aktivoitu OneDrive-sivustossa.</span><span class="sxs-lookup"><span data-stu-id="abbbe-104">When another user tries to open the file in Teams and receives the error message "You don't have access to this file," the issue occurs because the Limited-access user permission lockdown mode feature is activated on your OneDrive site.</span></span>

1. <span data-ttu-id="abbbe-105">Ohjeet ominaisuuden poistamiseen käytöstä OneDrive-sivustossa ovat kohdassa [Virhe avattaessa tiedostoa Teamsissa.](https://go.microsoft.com/fwlink/?linkid=2155733)</span><span class="sxs-lookup"><span data-stu-id="abbbe-105">For instructions to disable the feature on the OneDrive site, see [Error when opening a file in Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span></span>

1. <span data-ttu-id="abbbe-106">Tarkista, onko toisella käyttäjällä OneDrive-sivuston käyttöoikeus, ja anna käyttöoikeudet noudattamalla OneDrive-tiedostojen ja -kansioiden jakaminen [-ohjeita.](https://go.microsoft.com/fwlink/?linkid=2156017)</span><span class="sxs-lookup"><span data-stu-id="abbbe-106">Check whether another user has access to the OneDrive site, and provide access by following the instructions in [Share OneDrive files and folders](https://go.microsoft.com/fwlink/?linkid=2156017).</span></span>