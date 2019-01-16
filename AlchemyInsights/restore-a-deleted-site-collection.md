---
title: Poistetun sivustokokoelman palauttaminen
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: b3c72033dfcc093dd0c2837d2866c6a78d64449c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286833"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="7ae28-102">Poistetun sivustokokoelman palauttaminen</span><span class="sxs-lookup"><span data-stu-id="7ae28-102">Restore a deleted site collection</span></span>

<span data-ttu-id="7ae28-p101">Järjestelmänvalvojan poistaa sivustokokoelman classic, kun se sijoitetaan sivustokokoelman roskakoriin, jossa se pidetään 93 päivää ennen kuin se poistetaan pysyvästi. Voit palauttaa sivustokokoelman seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="7ae28-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="7ae28-105">Valitse klassinen SharePoint-hallintakeskukseen nauhan **Roskakoriin** .</span><span class="sxs-lookup"><span data-stu-id="7ae28-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="7ae28-106">Valitse valintaruutu, jonka haluat palauttaa sivustokokoelman.</span><span class="sxs-lookup"><span data-stu-id="7ae28-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="7ae28-107">Valitse **Palauta poistetut kohteet**.</span><span class="sxs-lookup"><span data-stu-id="7ae28-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="7ae28-p102">Voit palauttaa poistetun Viestimissivusto, uusi SharePoint-admin center esikatselu. Muussa tapauksessa sinun on käytettävä PowerShell. Jos haluat palauttaa sivuston, joka kuuluu Office 365-ryhmään, sinun on palautettava ryhmän Exchange admin Centerissä. Ryhmiä voidaan palauttaa 30 päivän ajan sen jälkeen, kun ne ovat poistettu.</span><span class="sxs-lookup"><span data-stu-id="7ae28-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

