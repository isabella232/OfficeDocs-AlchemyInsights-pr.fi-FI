---
title: Microsoft 365 -ryhmän sähköpostiosoitteen muuttaminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282711"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Microsoft 365 -ryhmän sähköpostiosoitteen muuttaminen

Voit muuttaa Microsoft 365 -ryhmän sähköpostiosoitetta hallintakeskuksen avulla. Valitse vain ryhmä ja valitse @edit sähköpostiosoite.

Voit myös muuttaa Microsoft 365 -ryhmän ensisijaista SMTP-osoitetta seuraavan EXO PowerShell -komennon avulla:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress -asetus<new SMTP Address>

Esimerkki:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
