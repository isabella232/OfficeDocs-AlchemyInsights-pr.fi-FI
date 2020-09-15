---
title: Sisältö haku ei tulosta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680644"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="4b5b1-102">Ei tuloksia sisältö hausta/viennistä</span><span class="sxs-lookup"><span data-stu-id="4b5b1-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="4b5b1-103">Sisältö haun ja viennin ongelmat, jotka eivät palauta mitään tietoja, voivat johtua siitä, että tietty järjestelmänvalvoja on saattanut määrittää tietyt yhteensopivuus tieto turva suodattimet eikä tiedota asiasta kaikille järjestelmänvalvojille.</span><span class="sxs-lookup"><span data-stu-id="4b5b1-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="4b5b1-104">Jos haluat korjata tämän ongelman, tarkista, onko yhteensopivuus suojausta mahdollisesti aiheuttava.</span><span class="sxs-lookup"><span data-stu-id="4b5b1-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="4b5b1-105">Yhteyden muodostaminen tieto turva-ja yhteensopivuus keskuksen PowerShellin avulla</span><span class="sxs-lookup"><span data-stu-id="4b5b1-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="4b5b1-106">Suorita seuraavat komentosovelmat:</span><span class="sxs-lookup"><span data-stu-id="4b5b1-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="4b5b1-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="4b5b1-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="4b5b1-108">Get-Compreancesecurityfilter-Organization $org</span><span class="sxs-lookup"><span data-stu-id="4b5b1-108">Get-ComplianceSecurityFilter -Organization $org</span></span>