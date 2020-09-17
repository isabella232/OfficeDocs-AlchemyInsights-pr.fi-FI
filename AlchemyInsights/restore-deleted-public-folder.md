---
title: Poistetun yleisen kansion palauttaminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774528"
---
# <a name="restore-a-deleted-public-folder"></a>Poistetun yleisen kansion palauttaminen

**Poistettujen kohteiden palauttaminen julkisesta kansiosta**:

- Katso [, ettet voi palauttaa poistettuja kohteita muusta kuin sähkö postin julkisesta kansiosta Outlook 2016: ssä](https://aka.ms/pfrec).
 
**Poistetun yleisen kansion (minkä tahansa tyypin) palauttaminen**: 

- Käytä seuraavaa EXO PowerShell-komentoa:

    Syntaksi

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Esimerkki: seuraava komento palauttaa Subfolder1 ja sijoittaa sen \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Lisä tietoja [on kohdassa poistetun julkisen kansion palauttaminen](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
