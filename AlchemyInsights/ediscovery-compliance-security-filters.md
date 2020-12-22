---
title: Sisältö haun/viennin aikana ei palautettu tuloksia
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727220"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="30918-102">Sisältö haun/viennin aikana ei palautettu tuloksia</span><span class="sxs-lookup"><span data-stu-id="30918-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="30918-103">Jos kohtaat ongelmia seuraavissa eDiscoveryn skenaarioissa:</span><span class="sxs-lookup"><span data-stu-id="30918-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="30918-104">Sisältö haku/vienti palauttaa tietoja tai odottamattomia tietoja</span><span class="sxs-lookup"><span data-stu-id="30918-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="30918-105">eDiscoveryn haku tai vienti epäonnistuu</span><span class="sxs-lookup"><span data-stu-id="30918-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="30918-106">Tämä voi johtua joistakin vaatimustenmukaisuutta koskevista tieto turva suodattimista, jotka on määritetty tietyn järjestelmänvalvojan toimesta ja joita ei ole toimitettu kaikille järjestelmänvalvojille.</span><span class="sxs-lookup"><span data-stu-id="30918-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="30918-107">Jos haluat korjata ongelman, tarkista, että seuraavat ongelmat voivat aiheuttaa yhteensopivuus suojausta:</span><span class="sxs-lookup"><span data-stu-id="30918-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="30918-108">Yhteyden muodostaminen tieto turva-ja yhteensopivuus keskuksen PowerShellin avulla</span><span class="sxs-lookup"><span data-stu-id="30918-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="30918-109">Suorita seuraavat komentosovelmat:</span><span class="sxs-lookup"><span data-stu-id="30918-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="30918-110">Lisä tietoja yhteensopivuuden suojaus suodattimista on Ohje aiheessa [sisältö haun käyttö oikeuksien suodattaminen](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="30918-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
