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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995619"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Vaihda Microsoft 365 -ryhmän tai Microsoft Teamsin sähköpostiosoite

Voit vaihtaa Microsoft 365 -ryhmän tai Microsoft Teamsin sähköpostiosoitteen menemällä [Microsoft 365 -hallintakeskukseen](https://admin.microsoft.com/). Valitse ryhmä ja sitten @muokkaa sähköpostiosoitetta.

Voit myös käyttää seuraavaa EXO PowerShell -komentoa vaihtaaksesi Microsoft 365 -ryhmän tai Teamsin ensisijaisen SMTP-osoitteen:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Esimerkki:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
