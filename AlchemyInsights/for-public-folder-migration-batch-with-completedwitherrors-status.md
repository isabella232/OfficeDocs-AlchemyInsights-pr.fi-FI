---
title: Yleisen kansion siirtoerä, jonka Tila on CompletedWithErrors
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
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043583"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Yleisen kansion siirtoerä, jonka Tila on CompletedWithErrors

Suorita erä seuraavasti ja ohita suuret/virheelliset kohteet: 
1. Hyväksy ohitetut nimikkeet siirtoerässä:

    Aseta-MigrationBatch \<batchname> -ApproveSkippedItems 
2. Seuraavan komennon avulla voit hyväksyä ohitetut kohteet siirtopyynnöissä, jotka on synkronoitu mutta joita ei ole suoritettu loppuun:

    $pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -includereport; ForEach ($i $pf) {jos ($i.LargeItemsEncountered -gt 0 -tai $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}
3. Siirtoerän ja pyyntöjen pitäisi jatkua ja suorittaa muutamassa minuutissa.

