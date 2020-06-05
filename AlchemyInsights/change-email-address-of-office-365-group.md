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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="45bc7-102">Microsoft 365 -ryhmän sähköpostiosoitteen muuttaminen</span><span class="sxs-lookup"><span data-stu-id="45bc7-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="45bc7-103">Voit muuttaa Microsoft 365 -ryhmän sähköpostiosoitetta hallintakeskuksen avulla.</span><span class="sxs-lookup"><span data-stu-id="45bc7-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="45bc7-104">Valitse vain ryhmä ja valitse @edit sähköpostiosoite.</span><span class="sxs-lookup"><span data-stu-id="45bc7-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="45bc7-105">Voit myös muuttaa Microsoft 365 -ryhmän ensisijaista SMTP-osoitetta exo PowerShell -komennon avulla:</span><span class="sxs-lookup"><span data-stu-id="45bc7-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="45bc7-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="45bc7-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="45bc7-107">Esimerkki:</span><span class="sxs-lookup"><span data-stu-id="45bc7-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
