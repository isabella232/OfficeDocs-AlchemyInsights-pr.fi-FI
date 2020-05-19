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
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="7dd4a-102">Microsoft 365 -ryhmän sähköpostiosoitteen muuttaminen</span><span class="sxs-lookup"><span data-stu-id="7dd4a-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="7dd4a-103">Voit muuttaa Microsoft 365 -ryhmän sähköpostiosoitetta hallintakeskuksen avulla.</span><span class="sxs-lookup"><span data-stu-id="7dd4a-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="7dd4a-104">Valitse vain ryhmä ja valitse @edit sähköpostiosoite.</span><span class="sxs-lookup"><span data-stu-id="7dd4a-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="7dd4a-105">Voit myös muuttaa Microsoft 365 -ryhmän ensisijaista SMTP-osoitetta seuraavan EXO PowerShell -komennon avulla:</span><span class="sxs-lookup"><span data-stu-id="7dd4a-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="7dd4a-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress -asetus<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="7dd4a-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="7dd4a-107">Esimerkki:</span><span class="sxs-lookup"><span data-stu-id="7dd4a-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
