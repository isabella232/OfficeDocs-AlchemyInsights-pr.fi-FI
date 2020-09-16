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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="3533e-102">Yhdistettyä valvontaa ei voi ottaa käyttöön</span><span class="sxs-lookup"><span data-stu-id="3533e-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="3533e-103">Kun yrität ottaa käyttöön yhdistetyn valvonnan organisaatiossa, näyttöön voi tulla seuraavankaltainen virhe sanoma:</span><span class="sxs-lookup"><span data-stu-id="3533e-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="3533e-104">Voit korjata ongelman toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="3533e-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="3533e-105">[Muodosta yhteys Exchange Online PowerShelliin](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="3533e-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="3533e-106">Suorita seuraava cmdlet-komento:</span><span class="sxs-lookup"><span data-stu-id="3533e-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="3533e-107">Odota 60 minuuttia, ennen kuin edellinen asetus tulee voimaan.</span><span class="sxs-lookup"><span data-stu-id="3533e-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="3533e-108">Suorita seuraava komento Exchange Online PowerShellissä:</span><span class="sxs-lookup"><span data-stu-id="3533e-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="3533e-109">Lisä tietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="3533e-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="3533e-110">Yhteyden muodostaminen Exchange Online PowerShelliin monimenetelmäisen todentamisen avulla</span><span class="sxs-lookup"><span data-stu-id="3533e-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="3533e-111">Valvonta lokien haun ottaminen käyttöön tai poistaminen käytöstä</span><span class="sxs-lookup"><span data-stu-id="3533e-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
