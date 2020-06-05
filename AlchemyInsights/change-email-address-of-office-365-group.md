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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580654"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 -ryhmän sähköpostiosoitteen muuttaminen

Voit muuttaa Microsoft 365 -ryhmän sähköpostiosoitetta hallintakeskuksen avulla. Valitse vain ryhmä ja valitse @edit sähköpostiosoite.

Voit myös muuttaa Microsoft 365 -ryhmän ensisijaista SMTP-osoitetta exo PowerShell -komennon avulla:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Esimerkki:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
