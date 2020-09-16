---
title: Toimialueen nimipalvelimien päivittäminen osoittamaan Microsoftiin
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734908"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="71317-102">Toimialueen nimipalvelimien päivittäminen osoittamaan Microsoftiin</span><span class="sxs-lookup"><span data-stu-id="71317-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="71317-103">Huomautus: Nimipalvelinmuutosten levittyminen saattaa joskus kestää jopa 48 tuntia.</span><span class="sxs-lookup"><span data-stu-id="71317-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="71317-104">Jotta voit määrittää toimi alueesi Microsoftin kanssa, rekisteröinti palvelun nimi palvelimet on päivitettävä.</span><span class="sxs-lookup"><span data-stu-id="71317-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="71317-105">Luo nimipalvelintietueet tai muokkaa niitä toimialuerekisteröintipalvelussa.</span><span class="sxs-lookup"><span data-stu-id="71317-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="71317-106">Siirry toimialuerekisteröijän sivustolle ja etsi kohta, jossa voit muokata nimipalvelimia.</span><span class="sxs-lookup"><span data-stu-id="71317-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="71317-107">Luo kaksi nimipalvelintietuetta tai muokkaa tietueita niin, että ne vastaavat seuraavia arvoja:</span><span class="sxs-lookup"><span data-stu-id="71317-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="71317-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="71317-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="71317-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="71317-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="71317-110">Tallenna muutokset.</span><span class="sxs-lookup"><span data-stu-id="71317-110">Save changes.</span></span>

<span data-ttu-id="71317-111">Tässä artikkelissa on myös yksityiskohtaisia ohjeita: [nimi palvelimien muuttaminen niin, että Microsoft 365 on määritetty toimi alueen rekisteröinti palveluun](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="71317-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  