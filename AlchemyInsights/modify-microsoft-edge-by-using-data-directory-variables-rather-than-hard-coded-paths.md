---
title: Microsoft Edgen muokkaaminen datahakemiston muuttujien avulla kovakoodaajien polkujen sijaan
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035284"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a><span data-ttu-id="5e8d1-102">Microsoft Edgen muokkaaminen datahakemiston muuttujien avulla kovakoodaajien polkujen sijaan</span><span class="sxs-lookup"><span data-stu-id="5e8d1-102">Modify Microsoft Edge by using data directory variables rather than hard-coded paths</span></span>

<span data-ttu-id="5e8d1-103">Jos esimerkiksi tallennat profiilitiedot käyttäjän paikallisiin sovellustietoihin Windowsin oletussijainnin sijaan, määritä *UserDataDir-käytännön* arvoksi **${local_app_data}\Edge\Profile.**</span><span class="sxs-lookup"><span data-stu-id="5e8d1-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the *UserDataDir* policy to **${local_app_data}\Edge\Profile**.</span></span>

<span data-ttu-id="5e8d1-104">Lisätietoja on kohdassa [Microsoft Edgen käyttäjätietohakemiston muuttujien luominen.](https://docs.microsoft.com/deployedge/microsoft-edge-policies)</span><span class="sxs-lookup"><span data-stu-id="5e8d1-104">For more information, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span></span>