---
title: Avaa Resurssienhallinnassa ei toimi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713031"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="17229-102">Avaa Resurssienhallinnassa ei toimi</span><span class="sxs-lookup"><span data-stu-id="17229-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="17229-103">Jos **Avaa Resurssienhallinnassa** tai **Näytä Resurssienhallinnassa** -asetus ei toimi, varmista, että WebClient-palvelun asetuksena on **Käynnissä,** noudattamalla alla olevia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="17229-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="17229-104">Esimerkiksi SharePoint- tai OneDrive-kirjaston avaaminen voi kestää kauan, kun palvelu ei ole käynnissä.</span><span class="sxs-lookup"><span data-stu-id="17229-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="17229-105">Kirjoita Windowsin hakuruutuun suorita, valitse Suorita työpöytäsovellus, kirjoita services.msc ja valitse sitten **Enter**.</span><span class="sxs-lookup"><span data-stu-id="17229-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="17229-106">Vieritä alas WebClient-palveluun ja **Status** tarkista Tila-sarake.</span><span class="sxs-lookup"><span data-stu-id="17229-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="17229-107">Jos WebClient-palvelun tila ei ole **Käynnissä**, kaksoisnapsauta palvelua, napsauta **Käynnistä -painiketta**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="17229-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="17229-108">Ota palvelu tarvittaessa käyttöön valitsemalla **Käynnistystapa-ruudusta** **Joko Manuaalinen** tai **Automaattinen.**</span><span class="sxs-lookup"><span data-stu-id="17229-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="17229-109">Lisätietoja Resurssienhallinnan avaamiseen liittyvien ongelmien vianmäärityksestä on [ohjeaiheessa AvaaMinen Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="17229-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="17229-110">Tutustu synkronointiin parempina vaihtoehtoina: [Synkronoi SharePoint-tiedostot uuden OneDrive-synkronointiohjelman kanssa](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="17229-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

