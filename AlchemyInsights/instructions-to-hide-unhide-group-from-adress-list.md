---
title: Ohjeet Piilota/Näytä ryhmä osoite luettelosta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768916"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Piilota Office 365-ryhmä osoite luettelosta (GAL)

Voit piilottaa Office 365-ryhmän Exchange-asiakkaiden (kuten Outlookin tai OWA) osoite luetteloista (GAL) käyttämällä seuraavaa komentoa EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Jos haluat piilottaa Office 365-ryhmän näkyvistä Exchange-asiakkaille, käytä EXO Shell-kohteessa seuraavaa komentoa:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

