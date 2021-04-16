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
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809436"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="8182d-102">Poistetun yleisen kansion palauttaminen</span><span class="sxs-lookup"><span data-stu-id="8182d-102">Restore a deleted public folder</span></span>

<span data-ttu-id="8182d-103">**Poistettujen kohteiden palauttaminen julkisesta kansiosta:**</span><span class="sxs-lookup"><span data-stu-id="8182d-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="8182d-104">Katso [Poistettuja kohteita ei voi palauttaa Outlook 2016:n](https://aka.ms/pfrec)yleisistä kansioista.</span><span class="sxs-lookup"><span data-stu-id="8182d-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="8182d-105">**Poistetun yleisen kansion (minkä tahansa tyypin) palauttaminen:**</span><span class="sxs-lookup"><span data-stu-id="8182d-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="8182d-106">Käytä seuraavaa EXO PowerShell -komentoa:</span><span class="sxs-lookup"><span data-stu-id="8182d-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="8182d-107">Syntaksi:</span><span class="sxs-lookup"><span data-stu-id="8182d-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="8182d-108">Esimerkki: Seuraava komento palauttaa Alikansio1:n ja sijoittaa sen \Parent1-kansioon:</span><span class="sxs-lookup"><span data-stu-id="8182d-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="8182d-109">Lisätietoja [on kohdassa Poistetun yleisen](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) kansion palauttaminen.</span><span class="sxs-lookup"><span data-stu-id="8182d-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
