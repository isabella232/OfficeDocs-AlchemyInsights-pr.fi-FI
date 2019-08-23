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
ms.openlocfilehash: 9e4e9ade058c60ecd7a6ce1b2a40c4996ac5676f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36552463"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="ed0f9-102">Palauta poistettu sivusto</span><span class="sxs-lookup"><span data-stu-id="ed0f9-102">Restore a deleted site</span></span>

<span data-ttu-id="ed0f9-103">Kun järjestelmänvalvojan poistaa sivuston, se sijoitetaan sivustokokoelman roskakoriin, jossa se pidetään 93 päivää ennen kuin se poistetaan pysyvästi.</span><span class="sxs-lookup"><span data-stu-id="ed0f9-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="ed0f9-104">Palauta sivusto:</span><span class="sxs-lookup"><span data-stu-id="ed0f9-104">To restore the site:</span></span>
  
1. <span data-ttu-id="ed0f9-105">Valitse uuden SharePoint-hallintakeskukseen nauhan **Roskakoriin** .</span><span class="sxs-lookup"><span data-stu-id="ed0f9-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="ed0f9-106">Valitse valintaruutu, jonka haluat palauttaa sivustokokoelman.</span><span class="sxs-lookup"><span data-stu-id="ed0f9-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="ed0f9-107">Valitse **Palauta poistetut kohteet**.</span><span class="sxs-lookup"><span data-stu-id="ed0f9-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="ed0f9-108">Voit palauttaa poistetun Viestimissivusto, uusi SharePoint-hallintakeskukseen.</span><span class="sxs-lookup"><span data-stu-id="ed0f9-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="ed0f9-109">Muussa tapauksessa sinun on käytettävä Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ed0f9-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="ed0f9-110">Jos haluat palauttaa sivuston, joka kuuluu Office 365-ryhmään, sinun on palautettava ryhmän Exchange admin Centerissä.</span><span class="sxs-lookup"><span data-stu-id="ed0f9-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="ed0f9-111">Ryhmiä voidaan palauttaa 30 päivän ajan sen jälkeen, kun ne ovat poistettu.</span><span class="sxs-lookup"><span data-stu-id="ed0f9-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

