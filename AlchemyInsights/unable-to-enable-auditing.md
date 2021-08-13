---
title: 2419-unable-to-enable-auditing
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007787"
---
# <a name="unable-to-enable-unified-auditing"></a>Yhdistetyn valvonnan ottaminen käyttöön ei onnistu

Kun yrität ottaa yhdistetyn valvonnan käyttöön organisaatiossasi, saatat saada seuraavan kaltaisen virhesanoman:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Voit ratkaista ongelman seuraavasti:

1. [Näyttöyhteys Powershellin Exchange Online avulla.](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Suorita seuraava cmdlet-komento:

   ```
   Enable-OrganizationCustomization
   ```

3. Odota 60 minuuttia, että edellinen asetus tulee voimaan.

4. Suorita PowerShellissä seuraava Exchange Online komento:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Lisätietoja on seuraavissa artikkeleissa:

- [Näyttöyhteys PowerShellin Exchange Online monimenetelmäisen todentamisen avulla](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Valvontalokihaun käyttöönottaaminen tai käytöstä pois käytöstä](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
