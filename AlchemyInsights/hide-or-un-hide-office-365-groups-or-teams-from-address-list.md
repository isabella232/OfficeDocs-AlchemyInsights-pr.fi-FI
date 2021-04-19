---
title: Office 365 -ryhmien tai -tiimien piilottaminen osoiteluettelosta tai sen piilottaminen
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
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811453"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Office 365 -ryhmien tai -tiimien piilottaminen osoiteluettelosta tai sen piilottaminen

Seuraavan EXO PowerShell -komennon avulla voit piilottaa Office 365 -ryhmän tai -ryhmät Exchange-asiakasohjelmien osoiteluetteloista (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Seuraavan EXO PowerShell -komennon avulla voit piilottaa tai poistaa Office365 -ryhmän/-tiimit Exchange-asiakasohjelmista (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Lisätietoja on kohdassa [Office 365 -ryhmien piilotminen GAL- ja Exchange-asiakasohjelmista.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
