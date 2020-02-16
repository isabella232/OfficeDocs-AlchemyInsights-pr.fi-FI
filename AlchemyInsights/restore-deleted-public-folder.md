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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="5bad1-102">Poistetun yleisen kansion palauttaminen</span><span class="sxs-lookup"><span data-stu-id="5bad1-102">Restore a deleted public folder</span></span>

<span data-ttu-id="5bad1-103">**Poistettujen kohteiden palauttaminen yleisestä kansiosta:**</span><span class="sxs-lookup"><span data-stu-id="5bad1-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="5bad1-104">Lisätietoja [on ohjeaiheessa Poistettujen kohteiden palauttaminen outlook 2016:n muusta kuin sähköpostin yleisestä kansiosta](https://aka.ms/pfrec)ei voi palauttaa.</span><span class="sxs-lookup"><span data-stu-id="5bad1-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="5bad1-105">**Poistetun yleisen kansion palauttaminen (minkä tahansa tyyppinen)**:</span><span class="sxs-lookup"><span data-stu-id="5bad1-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="5bad1-106">Käytä seuraavaa EXO PowerShell -komentoa:</span><span class="sxs-lookup"><span data-stu-id="5bad1-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="5bad1-107">Syntaksi:</span><span class="sxs-lookup"><span data-stu-id="5bad1-107">Syntax:</span></span>

    ><span data-ttu-id="5bad1-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Nimi -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-Polku, johon kansio palautetaan></span><span class="sxs-lookup"><span data-stu-id="5bad1-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="5bad1-109">Esimerkki: Seuraava komento palauttaa Alikansion1 ja sijoittaa sen \Parent1:n alle:</span><span class="sxs-lookup"><span data-stu-id="5bad1-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="5bad1-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Nimi -eq "Alikansio1"}; Set-PublicFolder $pf.identity -Polku \Parent1</span><span class="sxs-lookup"><span data-stu-id="5bad1-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="5bad1-111">Lisätietoja on ohjeaiheessa [Poistetun yleisen kansion palauttaminen.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)</span><span class="sxs-lookup"><span data-stu-id="5bad1-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
