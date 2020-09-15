---
title: Poistetun sivuston palauttaminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692040"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="68f61-102">Poistetun sivuston palauttaminen</span><span class="sxs-lookup"><span data-stu-id="68f61-102">Restore a deleted site</span></span>

<span data-ttu-id="68f61-103">Kun järjestelmänvalvoja poistaa SharePoint-sivuston, se sijoitetaan sivustokokoelman roska koriin, jossa se säilytetään 93 päivän ajan, ennen kuin se poistetaan pysyvästi.</span><span class="sxs-lookup"><span data-stu-id="68f61-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="68f61-104">Sivuston palauttaminen:</span><span class="sxs-lookup"><span data-stu-id="68f61-104">To restore the site:</span></span>
  
1. <span data-ttu-id="68f61-105">Valitse uudessa SharePoint-hallinta keskuksessa valinta nauhassa **roska** kori.</span><span class="sxs-lookup"><span data-stu-id="68f61-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="68f61-106">Valitse sen sivustokokoelman vieressä oleva valinta ruutu, jonka haluat palauttaa.</span><span class="sxs-lookup"><span data-stu-id="68f61-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="68f61-107">Valitse **Palauta poistetut kohteet**.</span><span class="sxs-lookup"><span data-stu-id="68f61-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="68f61-108">Jos haluat palauttaa poistetun viestintäsivuston, voit käyttää uutta SharePoint-hallinta keskusta.</span><span class="sxs-lookup"><span data-stu-id="68f61-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="68f61-109">Muussa tapa uksessa sinun on käytettävä Microsoft PowerShelliä.</span><span class="sxs-lookup"><span data-stu-id="68f61-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="68f61-110">Jos haluat palauttaa sivuston, joka kuuluu Microsoft 365-ryhmään, sinun on palautettava ryhmä Exchange-hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="68f61-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="68f61-111">Ryhmät voi palauttaa 30 päivän kuluttua niiden poistamisesta.</span><span class="sxs-lookup"><span data-stu-id="68f61-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

