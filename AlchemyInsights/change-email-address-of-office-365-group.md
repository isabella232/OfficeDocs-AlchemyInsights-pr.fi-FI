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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="fb229-102">Microsoft 365 -ryhmän sähköpostiosoitteen muuttaminen</span><span class="sxs-lookup"><span data-stu-id="fb229-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="fb229-103">Voit muuttaa Microsoft 365 -ryhmän sähköpostiosoitetta hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="fb229-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="fb229-104">Valitse ryhmä ja sitten @muokkaa sähköpostiosoitetta.</span><span class="sxs-lookup"><span data-stu-id="fb229-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="fb229-105">Voit muuttaa Microsoft 365 -ryhmän ensisijaisen SMTP-osoitteen myös exo PowerShell -komennon avulla:</span><span class="sxs-lookup"><span data-stu-id="fb229-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="fb229-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="fb229-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="fb229-107">Esimerkki:</span><span class="sxs-lookup"><span data-stu-id="fb229-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
