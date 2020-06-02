---
title: 2419-unable-to-enable-auditointi
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510425"
---
# <a name="unable-to-enable-unified-auditing"></a>Yhtenäistä valvontaa ei voi ottaa käyttöön

Kun yrität ottaa yhtenäisen valvonnan käyttöön organisaatiossasi, näyttöön saattaa tulla seuraavankaltainen virhe:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Voit ratkaista tämän ongelman seuraavasti:

1. [Muodosta yhteys Exchange Online Powershelliin](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Suorita seuraava cmdlet-komento:

   ```
   Enable-OrganizationCustomization
   ```

3. Odota 60 minuuttia, jotta edellinen asetus tulee voimaan.

4. Suorita seuraava komento Exchange Online PowerShellissä:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Lisätietoja on seuraavissa artikkeleissa:

- [Yhteyden muodostaminen Exchange Online PowerShelliin monivaiheisen todennuksen avulla](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Valvontalokin haun ottaminen käyttöön tai poistaminen käytöstä](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
