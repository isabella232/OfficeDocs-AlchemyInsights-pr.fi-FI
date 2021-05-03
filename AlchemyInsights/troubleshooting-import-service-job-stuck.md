---
title: Tuontipalvelutyön jumiutuessa vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125106"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="42284-102">Tuontipalvelutyön jumiutuessa vianmääritys</span><span class="sxs-lookup"><span data-stu-id="42284-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="42284-103">Jos sinulla on ongelmia jumiutuvien tai epäonnistuvien tuontipalvelutöiden kanssa, tarkista ja kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="42284-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="42284-104">Tarkista PST-tiedoston koko.</span><span class="sxs-lookup"><span data-stu-id="42284-104">Review the size of of the PST file.</span></span> <span data-ttu-id="42284-105">PST-tiedoston tuonnin suositeltu enimmäiskoko on 20 Gt.</span><span class="sxs-lookup"><span data-stu-id="42284-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="42284-106">Jos epäilet ohittaneen kohteita vioittumisen vuoksi, suorita Scanpst.exe pst-tiedostojen virheiden vianmääritystä ja korjaamista varten.</span><span class="sxs-lookup"><span data-stu-id="42284-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="42284-107">Jos näet Tuonnin aikana MapiExceptionTyökalutoffQuotaExceeded-virheen, varmista, että kohdepostilaatikossa on riittävästi kapasiteettia haluttujen PST-tiedostojen tuomiseen.</span><span class="sxs-lookup"><span data-stu-id="42284-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="42284-108">Lisätietoja PST-tuontityön ongelmien vianmäärityksestä on kohdassa [PST-tuontitöiden ongelmien vianmääritys.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="42284-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="42284-109">Lisätietoja siitä, miten voit korjata ongelmia tuotaessa PST-tiedostoja Outlook on kohdassa [.pst-tiedoston Outlook (microsoft.com) ongelmien ratkaiseminen.](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="42284-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>