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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="2a7bb-102">Poistetun yleisen kansion palauttaminen</span><span class="sxs-lookup"><span data-stu-id="2a7bb-102">Restore a deleted public folder</span></span>

<span data-ttu-id="2a7bb-103">**Poistettujen kohteiden palauttaminen yleisestä kansiosta:**</span><span class="sxs-lookup"><span data-stu-id="2a7bb-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="2a7bb-104">Lisätietoja [on ohjeaiheessa Poistettujen kohteiden palauttaminen outlook 2016:n muusta kuin sähköpostin yleisestä kansiosta](https://aka.ms/pfrec)ei voi palauttaa.</span><span class="sxs-lookup"><span data-stu-id="2a7bb-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="2a7bb-105">**Poistetun yleisen kansion palauttaminen (minkä tahansa tyyppinen)**:</span><span class="sxs-lookup"><span data-stu-id="2a7bb-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="2a7bb-106">Käytä seuraavaa EXO PowerShell -komentoa:</span><span class="sxs-lookup"><span data-stu-id="2a7bb-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="2a7bb-107">Syntaksi:</span><span class="sxs-lookup"><span data-stu-id="2a7bb-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="2a7bb-108">Esimerkki: Seuraava komento palauttaa Alikansion1 ja sijoittaa sen \Parent1:n alle:</span><span class="sxs-lookup"><span data-stu-id="2a7bb-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="2a7bb-109">Lisätietoja on ohjeaiheessa [Poistetun yleisen kansion palauttaminen.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)</span><span class="sxs-lookup"><span data-stu-id="2a7bb-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
