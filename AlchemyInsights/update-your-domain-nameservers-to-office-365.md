---
title: Toimialueen nimipalvelimien päivittäminen Office 365:een
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36742174"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="ac01c-102">Toimialueen nimipalvelimien päivittäminen Office 365:een</span><span class="sxs-lookup"><span data-stu-id="ac01c-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="ac01c-103">Huomautus: Nimipalvelinmuutosten levittyminen saattaa joskus kestää jopa 48 tuntia.</span><span class="sxs-lookup"><span data-stu-id="ac01c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="ac01c-p101">Jos haluat määrittää toimialueen Office 365:ssä, rekisteröijän nimipalvelimet on päivitettävä. Luo nimipalvelintietueet tai muokkaa niitä toimialuerekisteröintipalvelussa.</span><span class="sxs-lookup"><span data-stu-id="ac01c-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="ac01c-106">Siirry toimialuerekisteröijän sivustolle ja etsi kohta, jossa voit muokata nimipalvelimia.</span><span class="sxs-lookup"><span data-stu-id="ac01c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="ac01c-107">Luo kaksi nimipalvelintietuetta tai muokkaa tietueita niin, että ne vastaavat seuraavia arvoja:</span><span class="sxs-lookup"><span data-stu-id="ac01c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="ac01c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ac01c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="ac01c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ac01c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="ac01c-110">Tallenna muutokset.</span><span class="sxs-lookup"><span data-stu-id="ac01c-110">Save changes.</span></span>

<span data-ttu-id="ac01c-111">Voit lukea tarkat ohjeet myös seuraavasta artikkelista: [Määritä Office 365 toimimaan minkä tahansa toimialuerekisteröijän kanssa muuttamalla nimipalvelimia](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="ac01c-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  