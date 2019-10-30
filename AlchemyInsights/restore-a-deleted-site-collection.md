---
title: Poistetun sivuston palauttaminen
ms.author: kaarins
author: kaarins
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: a1fb15869b9f576696de4eda4c0b2101bd6cca17
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768545"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="d6e9f-102">Poistetun sivuston palauttaminen</span><span class="sxs-lookup"><span data-stu-id="d6e9f-102">Restore a deleted site</span></span>

<span data-ttu-id="d6e9f-103">Kun järjestelmänvalvoja poistaa SharePoint-sivuston, se sijoitetaan sivustokokoelman roska koriin, jossa se säilytetään 93 päivää ennen sen poistamista pysyvästi.</span><span class="sxs-lookup"><span data-stu-id="d6e9f-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="d6e9f-104">Voit palauttaa sivuston:</span><span class="sxs-lookup"><span data-stu-id="d6e9f-104">To restore the site:</span></span>
  
1. <span data-ttu-id="d6e9f-105">Valitse uudessa SharePoint-hallinta keskuksessa valinta nauhassa **roska** kori.</span><span class="sxs-lookup"><span data-stu-id="d6e9f-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="d6e9f-106">Valitse palautettavan sivustokokoelman vieressä oleva valinta ruutu.</span><span class="sxs-lookup"><span data-stu-id="d6e9f-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="d6e9f-107">Valitse **Palauta poistetut kohteet**.</span><span class="sxs-lookup"><span data-stu-id="d6e9f-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="d6e9f-108">Voit palauttaa poistetun viestintä sivuston käyttämällä uutta SharePointin hallinta keskusta.</span><span class="sxs-lookup"><span data-stu-id="d6e9f-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="d6e9f-109">Muussa tapa uksessa sinun on käytettävä Microsoft PowerShelliä.</span><span class="sxs-lookup"><span data-stu-id="d6e9f-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="d6e9f-110">Jos haluat palauttaa sivuston, joka kuuluu Office 365-ryhmään, sinun on palautettava ryhmä Exchangen hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="d6e9f-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="d6e9f-111">Ryhmät voidaan palauttaa 30 päivän ajan niiden poistamisen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="d6e9f-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

