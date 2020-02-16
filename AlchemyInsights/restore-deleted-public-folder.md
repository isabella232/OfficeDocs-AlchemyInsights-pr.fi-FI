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
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063640"
---
# <a name="restore-a-deleted-public-folder"></a>Poistetun yleisen kansion palauttaminen

**Poistettujen kohteiden palauttaminen yleisestä kansiosta:**

- Lisätietoja [on ohjeaiheessa Poistettujen kohteiden palauttaminen outlook 2016:n muusta kuin sähköpostin yleisestä kansiosta](https://aka.ms/pfrec)ei voi palauttaa.
 
**Poistetun yleisen kansion palauttaminen (minkä tahansa tyyppinen)**: 

- Käytä seuraavaa EXO PowerShell -komentoa:

    Syntaksi:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Nimi -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-Polku, johon kansio palautetaan>

    Esimerkki: Seuraava komento palauttaa Alikansion1 ja sijoittaa sen \Parent1:n alle:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Nimi -eq "Alikansio1"}; Set-PublicFolder $pf.identity -Polku \Parent1

Lisätietoja on ohjeaiheessa [Poistetun yleisen kansion palauttaminen.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
