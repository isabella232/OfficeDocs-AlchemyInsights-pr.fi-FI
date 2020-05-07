---
title: PST-tiedostojen tuontiongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991156"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="53441-102">PST-tiedostojen tuontiongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="53441-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="53441-103">Jos tuot tietoja Outlook-asiakasohjelmassa, katso artikkeli [Outlookin .pst-tiedoston tuomiseen liittyvien ongelmien korjaaminen](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="53441-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="53441-104">Jos käytät tuontipalvelua ja se jumittuu, huomioi, että jokaisen Azure-tallennussijaintiin ladattavan PST-tiedoston koko saa olla enintään 20 Gt.</span><span class="sxs-lookup"><span data-stu-id="53441-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="53441-105">Yli 20 Gt:n PST-tiedostot voivat vaikuttaa PST-tuontiprosessin suorituskykyyn.</span><span class="sxs-lookup"><span data-stu-id="53441-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="53441-106">Jos haluat tarkistaa tietyn tuontityön tilan, voit käyttää [Get-MailboxImportRequest -eränimeä](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="53441-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="53441-107">Jos haluat lukea tarkempia tietoja tuontipalvelusta, katso artikkeli [Yleiskatsaus organisaation PST-tiedostojen tuonnista](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="53441-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>