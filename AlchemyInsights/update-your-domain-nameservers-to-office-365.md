---
title: Toimialueen nimipalvelimien päivittäminen Office 365:een
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.openlocfilehash: 81479c4438ce7d981af1312fd4eb7b6ae51ffd42
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286326"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="d2c75-102">Toimialueen nimipalvelimien päivittäminen Office 365:een</span><span class="sxs-lookup"><span data-stu-id="d2c75-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="d2c75-103">Huomautus: Nameserver muutokset Joskus voi kestää jopa 48 tuntia levittämiseen.</span><span class="sxs-lookup"><span data-stu-id="d2c75-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="d2c75-p101">Jos haluat määrittää toimialueen Office 365:ssä, rekisteröijän nimipalvelimet on päivitettävä. Luo nimipalvelintietueet tai muokkaa niitä toimialuerekisteröintipalvelussa.</span><span class="sxs-lookup"><span data-stu-id="d2c75-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="d2c75-106">Siirry toimialuerekisteröijän sivustolle ja etsi kohta, jossa voit muokata nimipalvelimia.</span><span class="sxs-lookup"><span data-stu-id="d2c75-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="d2c75-107">Luo kaksi nimipalvelintietuetta tai muokkaa tietueita niin, että ne vastaavat seuraavia arvoja:</span><span class="sxs-lookup"><span data-stu-id="d2c75-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="d2c75-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="d2c75-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="d2c75-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="d2c75-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="d2c75-110">Tallenna muutokset.</span><span class="sxs-lookup"><span data-stu-id="d2c75-110">Save changes.</span></span>
    
<span data-ttu-id="d2c75-111">Voit lukea tarkat ohjeet myös seuraavasta artikkelista: [Määritä Office 365 toimimaan minkä tahansa toimialuerekisteröijän kanssa muuttamalla nimipalvelimia](https://support.office.com/article/https://support.office.com/en-us/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="d2c75-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/https://support.office.com/en-us/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

