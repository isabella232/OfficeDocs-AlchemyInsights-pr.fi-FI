---
title: Avaa Explorer ei toimi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286320"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="12130-102">Avaa Explorer ei toimi</span><span class="sxs-lookup"><span data-stu-id="12130-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="12130-p101">Jos **Avaa Explorerissa** - tai **Resurssienhallinta-näkymässä** ei toimi Varmista WebClient-palvelu on **käynnissä** seuraamalla alla olevia ohjeita. Se voi kestää kauan, voit avata SharePoint- tai OneDrive-kirjastossa, kun palvelu ei ole käynnissä.</span><span class="sxs-lookup"><span data-stu-id="12130-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="12130-105">Valitse Windows-hakuruutuun Suorita, kirjoita Suorita desktop app, kirjoita services.msc ja valitse sitten **Enter**.</span><span class="sxs-lookup"><span data-stu-id="12130-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="12130-p102">Vieritä WebClient-palvelu ja tarkista **tila** -sarakkeesta. **Jos WebClient-palvelun tilaa ei ole **käynnissä**, kaksoisnapsauta palvelua ja valitse **Käynnistä**.** Ottaa käyttöön palvelun, tarvittaessa valitsemalla **manuaalisen** tai **automaattisen** **käynnistyksen tyyppi** -ruudusta.</span><span class="sxs-lookup"><span data-stu-id="12130-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="12130-p103">Avattaessa tiedostoa Explorer-ongelmien vianmäärityksen, on [avoinna Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665). Tutustu parempi vaihtoehto kuin synkronointi: [synkronointi SharePoint-tiedostot OneDrive synkronointi uuden asiakkaan kanssa](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="12130-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

