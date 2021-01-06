---
title: Vaihda Microsoft 365 -ryhmän tai Microsoft Teamsin sähköpostiosoite
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756554"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Vaihda Microsoft 365 -ryhmän tai Microsoft Teamsin sähköpostiosoite

Voit vaihtaa Microsoft 365 -ryhmän tai Microsoft Teamsin sähköpostiosoitteen menemällä [Microsoft 365 -hallintakeskukseen](https://admin.microsoft.com/). Valitse ryhmä ja sitten @muokkaa sähköpostiosoitetta.

Voit myös käyttää seuraavaa EXO PowerShell -komentoa vaihtaaksesi Microsoft 365 -ryhmän tai Teamsin ensisijaisen SMTP-osoitteen:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Esimerkki:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
