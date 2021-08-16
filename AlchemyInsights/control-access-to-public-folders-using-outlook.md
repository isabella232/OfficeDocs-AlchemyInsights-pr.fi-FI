---
title: Hallitse julkisten kansioiden Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032555"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Hallitse julkisten kansioiden Outlook

Voit hallita sitä, k voivatko käyttäjät käyttää julkisia kansioita Outlook:

1. Käytä `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Salli käyttäjien käyttää Outlook  
$false: Voit estää Outlook:n julkisten kansioiden Outlook. Tämä on oletusarvo.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Huomautus: Tämä toimintosarja voi hallita vain Outlook työpöytäsovelluksen Windows kanssa. Käyttäjät voivat edelleen käyttää julkisia kansioita OWA:n tai Outlook for Mac.

Lisätietoja on kohdassa [Hallitut yhteydet](https://aka.ms/controlpf) Outlook kansioihin.
