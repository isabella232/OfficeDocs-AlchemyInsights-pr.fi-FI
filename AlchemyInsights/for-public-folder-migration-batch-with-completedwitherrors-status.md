---
title: Yleisen kansion siirto erä, jossa on Completedwithapperrors-tila
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
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744110"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Yleisen kansion siirto erä, jossa on Completedwithapperrors-tila

Viimeistele erä suorittamalla seuraavat vaiheet, Ohita suuret/Virheelliset kohteet: 
1. Siirto erän ohitettujen kohteiden hyväksyminen:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Käytä seuraavaa komentoa, jos haluat hyväksyä ohitettujen kohteiden siirto pyynnöt, jotka on synkronoitu, mutta joita ei ole täytetty:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Siirto erän ja pyyntöjen pitäisi jatkua ja valmistu muutamassa minuutissa.

