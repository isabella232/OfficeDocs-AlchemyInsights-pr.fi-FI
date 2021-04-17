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
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Vaihda Microsoft 365 -ryhmän tai Microsoft Teamsin sähköpostiosoite

Voit vaihtaa Microsoft 365 -ryhmän tai Microsoft Teamsin sähköpostiosoitteen menemällä [Microsoft 365 -hallintakeskukseen](https://admin.microsoft.com/). Valitse ryhmä ja sitten @muokkaa sähköpostiosoitetta.

Voit myös käyttää seuraavaa EXO PowerShell -komentoa vaihtaaksesi Microsoft 365 -ryhmän tai Teamsin ensisijaisen SMTP-osoitteen:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Esimerkki:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
