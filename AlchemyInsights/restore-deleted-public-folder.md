---
title: Poistetun yleisen kansion palauttaminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158496"
---
# <a name="restore-a-deleted-public-folder"></a>Poistetun yleisen kansion palauttaminen

**Poistettujen kohteiden palauttaminen yleisestä kansiosta:**

- Lisätietoja [on ohjeaiheessa Poistettujen kohteiden palauttaminen outlook 2016:n muusta kuin sähköpostin yleisestä kansiosta](https://aka.ms/pfrec)ei voi palauttaa.
 
**Poistetun yleisen kansion palauttaminen (minkä tahansa tyyppinen)**: 

- Käytä seuraavaa EXO PowerShell -komentoa:

    Syntaksi:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Esimerkki: Seuraava komento palauttaa Alikansion1 ja sijoittaa sen \Parent1:n alle:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Lisätietoja on ohjeaiheessa [Poistetun yleisen kansion palauttaminen.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
