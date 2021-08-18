---
title: Ryhmien tai Office 365 piilottaminen tai piilottaminen osoiteluettelosta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088393"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Ryhmien tai Office 365 piilottaminen tai piilottaminen osoiteluettelosta

Seuraavan EXO PowerShell -komennon avulla voit piilottaa Office 365 tai poistaa sen Exchange asiakkaiden osoiteluetteloista (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Seuraavan EXO PowerShell -komennon avulla voit piilottaa tai poistaa Office365 -ryhmän tai -tiimit Exchange -asiakasohjelmista (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Lisätietoja on kohdassa Ryhmien [piilo Office 365 gal:sta ja Exchange asiakkaat.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
