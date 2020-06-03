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
ms.openlocfilehash: f295e0d7872a13cf47e386343b159e51bc0504de
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508085"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="30db2-102">Toimialueen nimipalvelimien päivittäminen osoittamaan Microsoftiin</span><span class="sxs-lookup"><span data-stu-id="30db2-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="30db2-103">Huomautus: Nimipalvelinmuutosten levittyminen saattaa joskus kestää jopa 48 tuntia.</span><span class="sxs-lookup"><span data-stu-id="30db2-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="30db2-p101">Jos haluat määrittää toimialueen Microsoft 365:ssä, rekisteröijän nimipalvelimet on päivitettävä. Luo nimipalvelintietueet tai muokkaa niitä toimialuerekisteröijän palvelussa.</span><span class="sxs-lookup"><span data-stu-id="30db2-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="30db2-106">Siirry toimialuerekisteröijän sivustolle ja etsi kohta, jossa voit muokata nimipalvelimia.</span><span class="sxs-lookup"><span data-stu-id="30db2-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="30db2-107">Luo kaksi nimipalvelintietuetta tai muokkaa tietueita niin, että ne vastaavat seuraavia arvoja:</span><span class="sxs-lookup"><span data-stu-id="30db2-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="30db2-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="30db2-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="30db2-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="30db2-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="30db2-110">Tallenna muutokset.</span><span class="sxs-lookup"><span data-stu-id="30db2-110">Save changes.</span></span>

<span data-ttu-id="30db2-111">Voit lukea tarkat ohjeet myös seuraavasta artikkelista: [Muuta nimipalvelimet minkä tahansa toimialuerekisteröijän kanssa](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="30db2-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  