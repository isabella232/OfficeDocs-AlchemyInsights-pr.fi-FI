---
title: Tietojen sijainti
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627843"
---
# <a name="data-location"></a><span data-ttu-id="40e0c-102">Tietojen sijainti</span><span class="sxs-lookup"><span data-stu-id="40e0c-102">Data location</span></span>

<span data-ttu-id="40e0c-103">Voit tarkastella Office 365-vuokra ajan sijaintia hallinta keskuksessa tai yhdistämällä Exchange Onlineen PowerShellin kautta.</span><span class="sxs-lookup"><span data-stu-id="40e0c-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="40e0c-104">**Hallinta keskus:**</span><span class="sxs-lookup"><span data-stu-id="40e0c-104">**Admin center:**</span></span>
1. <span data-ttu-id="40e0c-105">Kirjaudu [hallinta keskukseen](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="40e0c-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="40e0c-106">Valitse **Asetukset** > -**organisaatio profiili**.</span><span class="sxs-lookup"><span data-stu-id="40e0c-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="40e0c-107">Valitse **tietojen sijainti**-kohdassa **Näytä tiedot**.</span><span class="sxs-lookup"><span data-stu-id="40e0c-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="40e0c-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="40e0c-108">**PowerShell:**</span></span>
1. <span data-ttu-id="40e0c-109">Muodosta yhteys Exchange Onlineen Windows PowerShellin avulla.</span><span class="sxs-lookup"><span data-stu-id="40e0c-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="40e0c-110">Suorita [Hanki-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) -cmdlet-komentoa näyttääksesi luettelon vuokra ajan ominaisuuksista.</span><span class="sxs-lookup"><span data-stu-id="40e0c-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="40e0c-111">Katso OrganizationId-ominaisuutta.</span><span class="sxs-lookup"><span data-stu-id="40e0c-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="40e0c-112">Kun tieto sijainti on EXO ja SPO, voit määrittää datan sijainnin muille palveluille, joita voit käyttää [tietojen](https://products.office.com/where-is-your-data-located)sijainti paikasta.</span><span class="sxs-lookup"><span data-stu-id="40e0c-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>