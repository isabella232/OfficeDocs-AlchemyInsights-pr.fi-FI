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
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Microsoft Edgen muokkaaminen datahakemiston muuttujien avulla kovakoodaajien polkujen sijaan

Jos esimerkiksi tallennat profiilitiedot käyttäjän paikallisiin sovellustietoihin Windowsin oletussijainnin sijaan, määritä *UserDataDir-käytännön* arvoksi **${local_app_data}\Edge\Profile.**

Lisätietoja on kohdassa [Microsoft Edgen käyttäjätietohakemiston muuttujien luominen.](https://docs.microsoft.com/deployedge/microsoft-edge-policies)