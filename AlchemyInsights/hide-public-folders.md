---
title: Julkisten kansioiden piilottaminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315369"
---
# <a name="hide-public-folders"></a>Julkisten kansioiden piilottaminen

**Koko yleisen kansiopuun piilotminen:**

Tämän artikkelin ohjeiden avulla [voit piilottaa](https://aka.ms/ControlPF) koko yleisen kansiopuun valikoiduilta tai käyttäjiltä.

**Tietyn yleisen kansion piilottaminen:**

1. Käyttöoikeuksien lisääminen käyttäjille, joiden on tarpeen käyttää yleistä kansiota

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Poista käyttäjä **Oletus** **käyttöoikeusluettelosta:**

    `Remove-PublicFolderClientPermission \test1 -User Default`
