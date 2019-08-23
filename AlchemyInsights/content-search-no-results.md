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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516776"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="35887-102">Tuloksia-sisällön haku ja vienti</span><span class="sxs-lookup"><span data-stu-id="35887-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="35887-103">Ongelmia kanssa sisällön haku ja vienti tuota tietoja voi olla tiettyjen vaatimusten Suojaussuodatin, jonka oli asennuksen tiettyyn Admin ja ei toimi kaikki järjestelmänvalvojat.</span><span class="sxs-lookup"><span data-stu-id="35887-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="35887-104">Voit ratkaista ongelman, Tarkista ovatko noudattaminen suojaus-suodattimia, jotka saattavat aiheuttaa tämän:</span><span class="sxs-lookup"><span data-stu-id="35887-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="35887-105">Security and Compliance Centeriin PowerShellin muodostaa yhteyden</span><span class="sxs-lookup"><span data-stu-id="35887-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="35887-106">Suorita seuraavat commandlets:</span><span class="sxs-lookup"><span data-stu-id="35887-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="35887-107">$org = ”yourdomain.com”</span><span class="sxs-lookup"><span data-stu-id="35887-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="35887-108">Get-ComplianceSecurityFilter-$org-organisaatio</span><span class="sxs-lookup"><span data-stu-id="35887-108">Get-ComplianceSecurityFilter -Organization $org</span></span>