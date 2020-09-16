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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="2d7fa-102">Yleisen kansion siirto erä, jossa on Completedwithapperrors-tila</span><span class="sxs-lookup"><span data-stu-id="2d7fa-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="2d7fa-103">Viimeistele erä suorittamalla seuraavat vaiheet, Ohita suuret/Virheelliset kohteet:</span><span class="sxs-lookup"><span data-stu-id="2d7fa-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="2d7fa-104">Siirto erän ohitettujen kohteiden hyväksyminen:</span><span class="sxs-lookup"><span data-stu-id="2d7fa-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="2d7fa-105">Käytä seuraavaa komentoa, jos haluat hyväksyä ohitettujen kohteiden siirto pyynnöt, jotka on synkronoitu, mutta joita ei ole täytetty:</span><span class="sxs-lookup"><span data-stu-id="2d7fa-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="2d7fa-106">Siirto erän ja pyyntöjen pitäisi jatkua ja valmistu muutamassa minuutissa.</span><span class="sxs-lookup"><span data-stu-id="2d7fa-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

