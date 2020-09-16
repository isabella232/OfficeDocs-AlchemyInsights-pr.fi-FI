---
title: 2419 – ei voi ottaa käyttöön – valvonta
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
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767596"
---
# <a name="unable-to-enable-unified-auditing"></a>Yhdistettyä valvontaa ei voi ottaa käyttöön

Kun yrität ottaa käyttöön yhdistetyn valvonnan organisaatiossa, näyttöön voi tulla seuraavankaltainen virhe sanoma:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Voit korjata ongelman toimimalla seuraavasti:

1. [Muodosta yhteys Exchange Online PowerShelliin](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Suorita seuraava cmdlet-komento:

   ```
   Enable-OrganizationCustomization
   ```

3. Odota 60 minuuttia, ennen kuin edellinen asetus tulee voimaan.

4. Suorita seuraava komento Exchange Online PowerShellissä:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Lisä tietoja on seuraavissa artikkeleissa:

- [Yhteyden muodostaminen Exchange Online PowerShelliin monimenetelmäisen todentamisen avulla](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Valvonta lokien haun ottaminen käyttöön tai poistaminen käytöstä](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
