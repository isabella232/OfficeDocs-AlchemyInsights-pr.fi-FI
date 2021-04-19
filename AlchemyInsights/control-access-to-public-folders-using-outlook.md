---
title: Julkisten kansioiden käytön hallinta Outlookin avulla
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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816737"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Julkisten kansioiden käytön hallinta Outlookin avulla

Voit määrittää, k voivatko käyttäjät käyttää julkisia kansioita Outlookin avulla:

1. Käytä `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Salli käyttäjien käyttää julkisia kansioita Outlookissa  
$false: Estä käyttäjien pääsy Yleisiin kansioihin Outlookissa. Tämä on oletusarvo.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Huomautus: Tässä menettelyssä voidaan hallita ainoastaan yhteyksiä Outlookin työpöytäversioon Windows-asiakassovellohjelmia varten. Käyttäjät voivat edelleen käyttää julkisia kansioita OWA:n tai Outlook for Macin avulla.

Lisätietoja on kohdassa [Hallitut yhteydet yleisiin kansioihin Outlookissa.](https://aka.ms/controlpf)
