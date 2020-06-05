---
title: Poistetun sivuston palauttaminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 7c2ae754c86a3502092b622c55d18f3f4006bf8b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582232"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="2e5c0-102">Poistetun sivuston palauttaminen</span><span class="sxs-lookup"><span data-stu-id="2e5c0-102">Restore a deleted site</span></span>

<span data-ttu-id="2e5c0-103">Kun järjestelmänvalvoja poistaa SharePoint-sivuston, se sijoitetaan sivustokokoelman roskakoriin, jossa sitä säilytetään 93 päivää ennen sen poistamista pysyvästi.</span><span class="sxs-lookup"><span data-stu-id="2e5c0-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="2e5c0-104">Sivuston palauttaminen:</span><span class="sxs-lookup"><span data-stu-id="2e5c0-104">To restore the site:</span></span>
  
1. <span data-ttu-id="2e5c0-105">Valitse uudessa SharePoint-hallintakeskuksessa valintanauhasta **Roskakori.**</span><span class="sxs-lookup"><span data-stu-id="2e5c0-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="2e5c0-106">Valitse palautettavan sivustokokoelman vieressä oleva valintaruutu.</span><span class="sxs-lookup"><span data-stu-id="2e5c0-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="2e5c0-107">Valitse **Palauta poistetut kohteet**.</span><span class="sxs-lookup"><span data-stu-id="2e5c0-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="2e5c0-108">Voit palauttaa poistetun tietoliikennesivuston käyttämällä uutta SharePoint-hallintakeskusta.</span><span class="sxs-lookup"><span data-stu-id="2e5c0-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="2e5c0-109">Muussa tapauksessa sinun on käytettävä Microsoft PowerShelliä.</span><span class="sxs-lookup"><span data-stu-id="2e5c0-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="2e5c0-110">Jos haluat palauttaa Microsoft 365 -ryhmään kuuluvan sivuston, sinun on palautettava ryhmä Exchange-hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="2e5c0-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="2e5c0-111">Ryhmät voidaan palauttaa 30 päivän ajan niiden poistamisen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="2e5c0-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

