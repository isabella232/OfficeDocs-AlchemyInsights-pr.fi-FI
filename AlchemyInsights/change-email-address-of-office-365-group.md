---
title: Microsoft 365 -ryhmän sähköpostiosoitteen muuttaminen
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
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819041"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 -ryhmän sähköpostiosoitteen muuttaminen

Voit muuttaa Microsoft 365 -ryhmän sähköpostiosoitetta hallintakeskuksessa. Valitse ryhmä ja sitten @muokkaa sähköpostiosoitetta.

Voit muuttaa Microsoft 365 -ryhmän ensisijaisen SMTP-osoitteen myös exo PowerShell -komennon avulla:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Esimerkki:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
