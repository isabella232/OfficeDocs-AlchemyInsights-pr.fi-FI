---
title: Vaihda Microsoft 365 -ryhmän tai Microsoft Teamsin sähköpostiosoite
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819077"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="071e4-102">Vaihda Microsoft 365 -ryhmän tai Microsoft Teamsin sähköpostiosoite</span><span class="sxs-lookup"><span data-stu-id="071e4-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="071e4-103">Voit vaihtaa Microsoft 365 -ryhmän tai Microsoft Teamsin sähköpostiosoitteen menemällä [Microsoft 365 -hallintakeskukseen](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="071e4-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="071e4-104">Valitse ryhmä ja sitten @muokkaa sähköpostiosoitetta.</span><span class="sxs-lookup"><span data-stu-id="071e4-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="071e4-105">Voit myös käyttää seuraavaa EXO PowerShell -komentoa vaihtaaksesi Microsoft 365 -ryhmän tai Teamsin ensisijaisen SMTP-osoitteen:</span><span class="sxs-lookup"><span data-stu-id="071e4-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="071e4-106">Esimerkki:</span><span class="sxs-lookup"><span data-stu-id="071e4-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
