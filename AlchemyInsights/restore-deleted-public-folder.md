---
title: Poistetun yleisen kansion palauttaminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943372"
---
# <a name="restore-a-deleted-public-folder"></a>Poistetun yleisen kansion palauttaminen

**Poistettujen kohteiden palauttaminen julkisesta kansiosta:**

- Katso [Lisätietoja on kohdassa Et voi palauttaa poistettuja](https://aka.ms/pfrec)kohteita julkisesta kansiosta, joka ei ole Outlook 2016.
 
**Poistetun yleisen kansion (minkä tahansa tyypin) palauttaminen:** 

- Käytä seuraavaa EXO PowerShell -komentoa:

    Syntaksi:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Esimerkki: Seuraava komento palauttaa Alikansio1:n ja sijoittaa sen \Parent1-kansioon:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Lisätietoja [on kohdassa Poistetun yleisen](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) kansion palauttaminen.
