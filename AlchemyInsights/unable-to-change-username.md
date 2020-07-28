---
title: Käyttäjänimeä ei voi muuttaa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439552"
---
# <a name="unable-to-change-username"></a>Käyttäjänimeä ei voi muuttaa

Joissakin tapauksissa UPN (UserPrincipalName) -muutoksia ei välitetä pilveen. Näyttöön saattaa tulla vahvistusvirheitä Office 365 -portaalissa tai et voi muuttaa käyttäjänimeä tai sähköpostiosoitetta. Voit ratkaista tämän ongelman määrittämällä UserPrincipalName-nimen manuaalisesti käyttämällä tätä PowerShell-komentoa.

**Esimerkki: Käyttäjän nimeäminen uudelleen**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Tämä komento nimeää davidc@contoso.com uudelleen davidchew@contoso.com.

Lisätietoja on kohdassa [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).