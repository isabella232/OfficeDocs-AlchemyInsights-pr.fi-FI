---
title: Nimipalvelimen vaihtaminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706752"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="997f3-102">Toimialueen nimipalvelimien päivittäminen osoittamaan Microsoftiin</span><span class="sxs-lookup"><span data-stu-id="997f3-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="997f3-103">Huomautus: Nimipalvelinmuutosten levittyminen saattaa joskus kestää jopa 48 tuntia.</span><span class="sxs-lookup"><span data-stu-id="997f3-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="997f3-p101">Jos haluat määrittää toimialueen Microsoft 365:ssä, rekisteröijän nimipalvelimet on päivitettävä. Luo nimipalvelintietueet tai muokkaa niitä toimialuerekisteröijän palvelussa.</span><span class="sxs-lookup"><span data-stu-id="997f3-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="997f3-106">Siirry toimialuerekisteröijän sivustolle ja etsi kohta, jossa voit muokata nimipalvelimia.</span><span class="sxs-lookup"><span data-stu-id="997f3-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="997f3-107">Luo kaksi nimipalvelintietuetta tai muokkaa tietueita niin, että ne vastaavat seuraavia arvoja:</span><span class="sxs-lookup"><span data-stu-id="997f3-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="997f3-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="997f3-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="997f3-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="997f3-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="997f3-110">Tallenna muutokset.</span><span class="sxs-lookup"><span data-stu-id="997f3-110">Save changes.</span></span>

<span data-ttu-id="997f3-111">Voit lukea tarkat ohjeet myös seuraavasta artikkelista: [Muuta nimipalvelimet minkä tahansa toimialuerekisteröijän kanssa](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="997f3-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  