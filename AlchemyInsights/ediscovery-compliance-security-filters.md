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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678676"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="5a466-102">Sisältö haun/viennin aikana ei palautettu tuloksia</span><span class="sxs-lookup"><span data-stu-id="5a466-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="5a466-103">Jos kohtaat ongelmia seuraavissa eDiscoveryn skenaarioissa:</span><span class="sxs-lookup"><span data-stu-id="5a466-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="5a466-104">Sisältö haku/vienti palauttaa tietoja tai odottamattomia tietoja</span><span class="sxs-lookup"><span data-stu-id="5a466-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="5a466-105">eDiscoveryn haku tai vienti epäonnistuu</span><span class="sxs-lookup"><span data-stu-id="5a466-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="5a466-106">Tämä voi johtua siitä, että tietty järjestelmänvalvoja on saattanut määrittää tietyt yhteensopivuuden tieto turva suodattimen, eikä sitä ole toimitettu kaikille järjestelmänvalvojille.</span><span class="sxs-lookup"><span data-stu-id="5a466-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="5a466-107">Jos haluat korjata ongelman, tarkista, että seuraavat ongelmat voivat aiheuttaa yhteensopivuus suojausta:</span><span class="sxs-lookup"><span data-stu-id="5a466-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="5a466-108">Yhteyden muodostaminen tieto turva-ja yhteensopivuus keskuksen PowerShellin avulla</span><span class="sxs-lookup"><span data-stu-id="5a466-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="5a466-109">Suorita seuraavat komentosovelmat:</span><span class="sxs-lookup"><span data-stu-id="5a466-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="5a466-110">Lisä tietoja yhteensopivuuden suojaus suodattimista on Ohje aiheessa [sisältö haun käyttö oikeuksien suodattaminen](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="5a466-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
