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
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831875"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Piilota Microsoft 365 -ryhmä osoiteluettelosta

Jos haluat piilottaa Microsoft 365 -ryhmän Exchange-asiakkaiden osoiteluetteloista (kuten Outlook tai OWA), käytä seuraavaa komentoa EXO-käyttöliittymässä:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Jos haluat piilottaa Microsoft 365 -ryhmän Exchange-asiakasohjelmien näkyvistä, käytä seuraavaa komentoa EXO-liittymässä:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

