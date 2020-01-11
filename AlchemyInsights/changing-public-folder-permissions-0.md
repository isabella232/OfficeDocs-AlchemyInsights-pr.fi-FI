---
title: Yleisen kansion käyttö oikeuksien muuttaminen
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: 9d043e81b66cea1fcb985b0e1e79078409ba0b93
ms.sourcegitcommit: f23c39009d988228213fdb2bb7350bf4a0194194
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/11/2020
ms.locfileid: "41022194"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="f3d0e-102">Yleisen kansion käyttö oikeuksien muuttaminen</span><span class="sxs-lookup"><span data-stu-id="f3d0e-102">Changing public folder permissions</span></span>

<span data-ttu-id="f3d0e-103">Outlookin käyttäjät ja järjestelmänvalvojat voivat muuttaa yleisten kansioiden käyttö oikeuksia.</span><span class="sxs-lookup"><span data-stu-id="f3d0e-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="f3d0e-104">Järjestelmänvalvojat voivat myös valvoa Exchange-hallinta keskuksen (EAC) käyttö oikeuksia tekemällä seuraavat toimet:</span><span class="sxs-lookup"><span data-stu-id="f3d0e-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="f3d0e-105">Siirry Microsoft 365-hallinta keskukseen ja valitse **hallinta keskusten** \> **vaihto**.</span><span class="sxs-lookup"><span data-stu-id="f3d0e-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="f3d0e-106">Valitse **yleiset kansiot**.</span><span class="sxs-lookup"><span data-stu-id="f3d0e-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="f3d0e-107">Voit muuttaa yksittäisten yleisten kansioiden käyttö oikeuksia määrittämällä suojaus ryhmät käyttö oikeuksille.</span><span class="sxs-lookup"><span data-stu-id="f3d0e-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="f3d0e-108">Jotta loppu käyttäjä voisi muuttaa yleisten kansioiden käyttö oikeuksia, käyttäjällä on oltava kansion omistajan oikeudet.</span><span class="sxs-lookup"><span data-stu-id="f3d0e-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

> [!NOTE]
> <span data-ttu-id="f3d0e-109">Yleisten kansioiden käyttö oikeuksien muuttamisen yhteydessä saattaa olla useita tunnettuja ongelmia.</span><span class="sxs-lookup"><span data-stu-id="f3d0e-109">There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="f3d0e-110">Lisä tietoja on seuraavissa artikkeleissa.</span><span class="sxs-lookup"><span data-stu-id="f3d0e-110">See the following articles for more information.</span></span>
>
> [<span data-ttu-id="f3d0e-111">Yleisten kansioiden alikansioiden käyttö oikeuksia ei voi käyttää EAC-kohteessa</span><span class="sxs-lookup"><span data-stu-id="f3d0e-111">Can’t apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)
>
> [<span data-ttu-id="f3d0e-112">"Posti laatikkoa ei löydy paikallisesta puuryhmässä"-virhe, kun käytät julkisia kansioita</span><span class="sxs-lookup"><span data-stu-id="f3d0e-112">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
