---
title: Yleisen kansion siirtoerä, jonka tila on CompletedWithErrors
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
- "3532"
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068161"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Yleisen kansion siirtoerä, jonka tila on CompletedWithErrors

Suorita erä loppuun noudattamalla seuraavia ohjeita ja ohita suuret/huonot kohteet: 
1. Hyväksy ohitetut kohteet siirtoerässä:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Seuraavan komennon avulla voit hyväksyä ohitetut kohteet siirtopyynnöissä, jotka on "synkronoitu", mutta joita ei ole suoritettu loppuun:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Siirtoerän ja pyyntöjen pitäisi jatkua ja valmistua muutaman minuutin kuluttua.

