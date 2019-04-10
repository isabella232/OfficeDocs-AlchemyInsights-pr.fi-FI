---
title: Palauta poistettu sivusto
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
ms.openlocfilehash: 0cf10a3a0effc1774d8a07c5d0be96384362c175
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747775"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="e32a2-102">Palauta poistettu sivusto</span><span class="sxs-lookup"><span data-stu-id="e32a2-102">Restore a deleted site</span></span>

<span data-ttu-id="e32a2-103">Kun järjestelmänvalvojan poistaa sivuston, se sijoitetaan sivustokokoelman roskakoriin, jossa se pidetään 93 päivää ennen kuin se poistetaan pysyvästi.</span><span class="sxs-lookup"><span data-stu-id="e32a2-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="e32a2-104">Palauta sivusto:</span><span class="sxs-lookup"><span data-stu-id="e32a2-104">To restore the site:</span></span>
  
1. <span data-ttu-id="e32a2-105">Valitse uuden SharePoint-hallintakeskukseen nauhan **Roskakoriin** .</span><span class="sxs-lookup"><span data-stu-id="e32a2-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="e32a2-106">Valitse valintaruutu, jonka haluat palauttaa sivustokokoelman.</span><span class="sxs-lookup"><span data-stu-id="e32a2-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="e32a2-107">Valitse **Palauta poistetut kohteet**.</span><span class="sxs-lookup"><span data-stu-id="e32a2-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="e32a2-108">Voit palauttaa poistetun Viestimissivusto, uusi SharePoint-hallintakeskukseen.</span><span class="sxs-lookup"><span data-stu-id="e32a2-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="e32a2-109">Muussa tapauksessa sinun on käytettävä Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e32a2-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="e32a2-110">Jos haluat palauttaa sivuston, joka kuuluu Office 365-ryhmään, sinun on palautettava ryhmän Exchange admin Centerissä.</span><span class="sxs-lookup"><span data-stu-id="e32a2-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="e32a2-111">Ryhmiä voidaan palauttaa 30 päivän ajan sen jälkeen, kun ne ovat poistettu.</span><span class="sxs-lookup"><span data-stu-id="e32a2-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

