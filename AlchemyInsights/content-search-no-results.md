---
title: Sisältö ei ole hakutulokset
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800314"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="e4f83-102">Tuloksia-sisällön haku ja vienti</span><span class="sxs-lookup"><span data-stu-id="e4f83-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="e4f83-103">Ongelmia kanssa sisällön haku ja vienti tuota tietoja voi olla tiettyjen vaatimusten Suojaussuodatin, jonka oli asennuksen tiettyyn Admin ja ei toimi kaikki järjestelmänvalvojat.</span><span class="sxs-lookup"><span data-stu-id="e4f83-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="e4f83-104">Voit ratkaista ongelman, Tarkista ovatko noudattaminen suojaus-suodattimia, jotka saattavat aiheuttaa tämän:</span><span class="sxs-lookup"><span data-stu-id="e4f83-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="e4f83-105">Security and Compliance Centeriin PowerShellin muodostaa yhteyden</span><span class="sxs-lookup"><span data-stu-id="e4f83-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="e4f83-106">Suorita seuraavat commandlets:</span><span class="sxs-lookup"><span data-stu-id="e4f83-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="e4f83-107">$org = ”yourdomain.com”</span><span class="sxs-lookup"><span data-stu-id="e4f83-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="e4f83-108">Get-ComplianceSecurityFilter-$org-organisaatio</span><span class="sxs-lookup"><span data-stu-id="e4f83-108">Get-ComplianceSecurityFilter -Organization $org</span></span>