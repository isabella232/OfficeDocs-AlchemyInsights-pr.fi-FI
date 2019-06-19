---
title: 2419-pysty-ja-ota-valvonta
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065633"
---
# <a name="unable-to-enable-unified-auditing"></a>Ei voi ottaa käyttöön yhtenäinen valvonta

Kun yrität ottaa käyttöön yhtenäinen valvonnan Office 365-organisaatiosi, näyttöön saattaa tulla virhesanoma seuraavasti:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Voit ratkaista tämän ongelman seuraavasti:

1. [Muodostaa yhteyden Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Suorita seuraavia cmdlet-komento:

   ```
   Enable-OrganizationCustomization
   ```

3. Odota, kunnes edellinen asetus voimaan 60 minuuttia.

4. Suorita seuraava komento Exchange Online-PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Lisätietoja on seuraavissa artikkeleissa:

- [Muodosta yhteys käyttäen monitasoisen todennuksen Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Office 365: n valvonta-lokista etsintää ottaminen käyttöön ja poistaminen käytöstä](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
