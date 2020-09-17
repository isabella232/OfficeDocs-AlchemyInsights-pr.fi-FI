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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="e500d-102">Poistetun yleisen kansion palauttaminen</span><span class="sxs-lookup"><span data-stu-id="e500d-102">Restore a deleted public folder</span></span>

<span data-ttu-id="e500d-103">**Poistettujen kohteiden palauttaminen julkisesta kansiosta**:</span><span class="sxs-lookup"><span data-stu-id="e500d-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="e500d-104">Katso [, ettet voi palauttaa poistettuja kohteita muusta kuin sähkö postin julkisesta kansiosta Outlook 2016: ssä](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="e500d-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="e500d-105">**Poistetun yleisen kansion (minkä tahansa tyypin) palauttaminen**:</span><span class="sxs-lookup"><span data-stu-id="e500d-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="e500d-106">Käytä seuraavaa EXO PowerShell-komentoa:</span><span class="sxs-lookup"><span data-stu-id="e500d-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="e500d-107">Syntaksi</span><span class="sxs-lookup"><span data-stu-id="e500d-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="e500d-108">Esimerkki: seuraava komento palauttaa Subfolder1 ja sijoittaa sen \Parent1:</span><span class="sxs-lookup"><span data-stu-id="e500d-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="e500d-109">Lisä tietoja [on kohdassa poistetun julkisen kansion palauttaminen](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="e500d-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
