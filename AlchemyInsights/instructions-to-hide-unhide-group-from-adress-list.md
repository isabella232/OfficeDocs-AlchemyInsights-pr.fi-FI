---
title: Ohjeet ryhmän piilotta tai näyttäminen osoiteluettelosta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926242"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Piilota Microsoft 365 osoiteluettelosta (GAL)

Jos haluat Microsoft 365 ryhmän osoiteluetteloista (GAL) Exchange (kuten Outlook tai OWA), käytä seuraavaa komentoa EXO-liittymässä:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Jos haluat Microsoft 365 ryhmän näkymisen muille Exchange, käytä seuraavaa komentoa EXO-liittymässä:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

