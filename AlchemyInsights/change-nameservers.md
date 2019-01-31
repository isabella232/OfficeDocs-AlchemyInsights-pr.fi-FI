---
title: NameServers muuttaminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 901e0aaaa6550059318bfce35a2e97ad60a71360
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659732"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="81400-102">Toimialueen nimipalvelimien päivittäminen Office 365:een</span><span class="sxs-lookup"><span data-stu-id="81400-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="81400-103">Huomautus: Nameserver muutokset Joskus voi kestää jopa 48 tuntia levittämiseen.</span><span class="sxs-lookup"><span data-stu-id="81400-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="81400-p101">Jos haluat määrittää toimialueen Office 365:ssä, rekisteröijän nimipalvelimet on päivitettävä. Luo nimipalvelintietueet tai muokkaa niitä toimialuerekisteröintipalvelussa.</span><span class="sxs-lookup"><span data-stu-id="81400-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="81400-106">Siirry toimialuerekisteröijän sivustolle ja etsi kohta, jossa voit muokata nimipalvelimia.</span><span class="sxs-lookup"><span data-stu-id="81400-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="81400-107">Luo kaksi nimipalvelintietuetta tai muokkaa tietueita niin, että ne vastaavat seuraavia arvoja:</span><span class="sxs-lookup"><span data-stu-id="81400-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="81400-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="81400-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="81400-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="81400-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="81400-110">Tallenna muutokset.</span><span class="sxs-lookup"><span data-stu-id="81400-110">Save changes.</span></span>
    
<span data-ttu-id="81400-111">Voit lukea tarkat ohjeet myös seuraavasta artikkelista: [Määritä Office 365 toimimaan minkä tahansa toimialuerekisteröijän kanssa muuttamalla nimipalvelimia](https://support.office.com/article/https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="81400-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

