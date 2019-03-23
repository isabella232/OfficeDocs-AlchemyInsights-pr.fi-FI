---
title: Poistetun sivustokokoelman palauttaminen
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 1f9a66daf7bee43291b785b6260aec8725ee782f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753783"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="2653d-102">Poistetun sivustokokoelman palauttaminen</span><span class="sxs-lookup"><span data-stu-id="2653d-102">Restore a deleted site collection</span></span>

<span data-ttu-id="2653d-103">Järjestelmänvalvojan poistaa sivustokokoelman classic, kun se sijoitetaan sivustokokoelman roskakoriin, jossa se pidetään 93 päivää ennen kuin se poistetaan pysyvästi.</span><span class="sxs-lookup"><span data-stu-id="2653d-103">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="2653d-104">Voit palauttaa sivustokokoelman seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="2653d-104">To restore the site collection:</span></span>
  
1. <span data-ttu-id="2653d-105">Valitse klassinen SharePoint-hallintakeskukseen nauhan **Roskakoriin** .</span><span class="sxs-lookup"><span data-stu-id="2653d-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="2653d-106">Valitse valintaruutu, jonka haluat palauttaa sivustokokoelman.</span><span class="sxs-lookup"><span data-stu-id="2653d-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="2653d-107">Valitse **Palauta poistetut kohteet**.</span><span class="sxs-lookup"><span data-stu-id="2653d-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="2653d-108">Voit palauttaa poistetun Viestimissivusto, uusi SharePoint-admin center esikatselu.</span><span class="sxs-lookup"><span data-stu-id="2653d-108">To restore a deleted communication site, you can use the new SharePoint admin center preview.</span></span> <span data-ttu-id="2653d-109">Muussa tapauksessa sinun on käytettävä PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2653d-109">Otherwise, you need to use PowerShell.</span></span> <span data-ttu-id="2653d-110">Jos haluat palauttaa sivuston, joka kuuluu Office 365-ryhmään, sinun on palautettava ryhmän Exchange admin Centerissä.</span><span class="sxs-lookup"><span data-stu-id="2653d-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="2653d-111">Ryhmiä voidaan palauttaa 30 päivän ajan sen jälkeen, kun ne ovat poistettu.</span><span class="sxs-lookup"><span data-stu-id="2653d-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

