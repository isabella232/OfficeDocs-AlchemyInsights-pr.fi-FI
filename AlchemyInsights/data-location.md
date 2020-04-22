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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655279"
---
# <a name="data-location"></a><span data-ttu-id="8a605-102">Tietojen sijainti</span><span class="sxs-lookup"><span data-stu-id="8a605-102">Data location</span></span>

<span data-ttu-id="8a605-103">Voit tarkastella vuokraajan sijaintia hallintakeskuksessa tai muodostamalla yhteyden Exchange Onlineen PowerShellin kautta.</span><span class="sxs-lookup"><span data-stu-id="8a605-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="8a605-104">**Hallintakeskus:**</span><span class="sxs-lookup"><span data-stu-id="8a605-104">**Admin center:**</span></span>
1. <span data-ttu-id="8a605-105">Kirjaudu [hallintakeskukseen](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="8a605-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="8a605-106">Valitse **Asetukset** > **Organisaatioprofiili**.</span><span class="sxs-lookup"><span data-stu-id="8a605-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="8a605-107">Valitse **Tietojen sijainti**-kohdassa Näytä **tiedot**.</span><span class="sxs-lookup"><span data-stu-id="8a605-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="8a605-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="8a605-108">**PowerShell:**</span></span>
1. <span data-ttu-id="8a605-109">Muodosta yhteys Exchange Onlineen Windows PowerShellin avulla.</span><span class="sxs-lookup"><span data-stu-id="8a605-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="8a605-110">Suorita [Get-OrganizationalUnit-cmdlet-komento,](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) jolloin näkyviin tulee luettelo vuokraajan ominaisuuksista.</span><span class="sxs-lookup"><span data-stu-id="8a605-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="8a605-111">Katso OrganizationId-ominaisuutta.</span><span class="sxs-lookup"><span data-stu-id="8a605-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="8a605-112">Kun sinulla on EXO:n ja SPO:n tietosijainti, voit määrittää muiden palveluiden tietosijainnin, jota voit käyttää [kohdasta Missä tietosi sijaitsevat](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="8a605-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>