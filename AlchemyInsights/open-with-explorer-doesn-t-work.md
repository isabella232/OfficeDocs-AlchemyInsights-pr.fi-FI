---
title: Avaa Explorer ei toimi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764905"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="2e04c-102">Avaa Explorer ei toimi</span><span class="sxs-lookup"><span data-stu-id="2e04c-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="2e04c-103">Jos **Avaa Explorerissa** - tai **Resurssienhallinta-näkymässä** ei toimi Varmista WebClient-palvelu on **käynnissä** seuraamalla alla olevia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="2e04c-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="2e04c-104">Se voi kestää kauan, voit avata SharePoint- tai OneDrive-kirjastossa, kun palvelu ei ole käynnissä.</span><span class="sxs-lookup"><span data-stu-id="2e04c-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="2e04c-105">Valitse Windows-hakuruutuun Suorita, kirjoita Suorita desktop app, kirjoita services.msc ja valitse sitten **Enter**.</span><span class="sxs-lookup"><span data-stu-id="2e04c-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="2e04c-106">Vieritä WebClient-palvelu ja tarkista **tila** -sarakkeesta.</span><span class="sxs-lookup"><span data-stu-id="2e04c-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="2e04c-107">**Jos WebClient-palvelun tilaa ei ole **käynnissä**, kaksoisnapsauta palvelua ja valitse **Käynnistä**.**</span><span class="sxs-lookup"><span data-stu-id="2e04c-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="2e04c-108">Ottaa käyttöön palvelun, tarvittaessa valitsemalla **manuaalisen** tai **automaattisen** **käynnistyksen tyyppi** -ruudusta.</span><span class="sxs-lookup"><span data-stu-id="2e04c-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="2e04c-109">Avattaessa tiedostoa Explorer-ongelmien vianmäärityksen, on [avoinna Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="2e04c-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="2e04c-110">Tutustu parempi vaihtoehto kuin synkronointi: [synkronointi SharePoint-tiedostot OneDrive synkronointi uuden asiakkaan kanssa](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="2e04c-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

