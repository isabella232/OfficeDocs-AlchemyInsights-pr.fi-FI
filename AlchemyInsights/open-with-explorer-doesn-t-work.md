---
title: Avaa Resurssienhallinnassa ei toimi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694453"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="551cc-102">Avaa Resurssienhallinnassa ei toimi</span><span class="sxs-lookup"><span data-stu-id="551cc-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="551cc-103">Jos **Resurssienhallinta** **-tai Näytä Resurssienhallinnassa-** asetus ei toimi, varmista, että WebClient-palvelu on **käytössä** , noudattamalla seuraavia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="551cc-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="551cc-104">Esimerkiksi SharePoint-tai OneDrive-kirjaston avaaminen voi kestää kauan, kun palvelu ei ole käynnissä.</span><span class="sxs-lookup"><span data-stu-id="551cc-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="551cc-105">Kirjoita Windowsin haku ruutuun Suorita, valitse Suorita Työpöytä sovellus, kirjoita Services. msc ja valitse sitten **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="551cc-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="551cc-106">Vieritä alas WebClient-palveluun ja tarkista **tila** -sarake.</span><span class="sxs-lookup"><span data-stu-id="551cc-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="551cc-107">Jos WebClient-palvelun tila ei ole **käynnissä**, kaksoisnapsauta palvelua, valitse **Käynnistä**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="551cc-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="551cc-108">Ota palvelu käyttöön, jos se on tarpeen, valitsemalla **Käynnistys tapa** -ruudussa joko **Manuaalinen** tai **Automaattinen** .</span><span class="sxs-lookup"><span data-stu-id="551cc-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="551cc-109">Lisä tietoja Resurssienhallinnan avaamis ongelmien vian määrityksestä on kohdassa [Avaa Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="551cc-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="551cc-110">Tutustu synkronointiin paremmin vaihtoehtoisena: [Synkronoi SharePoint-tiedostot uuden OneDrive-synkronointi sovelluksen kanssa](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="551cc-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

