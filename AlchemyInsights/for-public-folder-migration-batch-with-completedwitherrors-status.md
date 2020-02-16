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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="eb985-102">Yleisen kansion siirtoerä, jonka Tila on CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="eb985-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="eb985-103">Suorita erä seuraavasti ja ohita suuret/virheelliset kohteet:</span><span class="sxs-lookup"><span data-stu-id="eb985-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="eb985-104">Hyväksy ohitetut nimikkeet siirtoerässä:</span><span class="sxs-lookup"><span data-stu-id="eb985-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="eb985-105">Aseta-MigrationBatch \<batchname> -ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="eb985-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="eb985-106">Seuraavan komennon avulla voit hyväksyä ohitetut kohteet siirtopyynnöissä, jotka on synkronoitu mutta joita ei ole suoritettu loppuun:</span><span class="sxs-lookup"><span data-stu-id="eb985-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="eb985-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -includereport; ForEach ($i $pf) {jos ($i.LargeItemsEncountered -gt 0 -tai $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="eb985-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="eb985-108">Siirtoerän ja pyyntöjen pitäisi jatkua ja suorittaa muutamassa minuutissa.</span><span class="sxs-lookup"><span data-stu-id="eb985-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

