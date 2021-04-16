---
title: eDiscovery-vientityökalu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814585"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="294e5-102">Eikö eDiscovery-vientityökalua voi asentaa tai suorittaa?</span><span class="sxs-lookup"><span data-stu-id="294e5-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="294e5-103">Jos et voi asentaa tai suorittaa eDiscovery-vientityökalua hakutulosten lataamiseksi, tarkista seuraavat asiat:</span><span class="sxs-lookup"><span data-stu-id="294e5-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="294e5-104">Käytössäsi on tietokone, joka täyttää seuraavat vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="294e5-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="294e5-105">Windows 7:n ja uudempien versioiden 32- tai 64-bittiset versiot</span><span class="sxs-lookup"><span data-stu-id="294e5-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="294e5-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="294e5-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="294e5-107">Tuettu selain:</span><span class="sxs-lookup"><span data-stu-id="294e5-107">A supported browser:</span></span>

  - <span data-ttu-id="294e5-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="294e5-108">Microsoft Edge</span></span>

    <span data-ttu-id="294e5-109">TAI</span><span class="sxs-lookup"><span data-stu-id="294e5-109">Or</span></span>

  - <span data-ttu-id="294e5-110">Internet Explorer 10 ja uudemmat versiot</span><span class="sxs-lookup"><span data-stu-id="294e5-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="294e5-111">Muita selaimia, kuten Google Chromea ja Mozilla Firefoxia, ei tueta.</span><span class="sxs-lookup"><span data-stu-id="294e5-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="294e5-112">Organisaatiosi voi muodostaa yhteyden Azuren päätepisteeseen, joka on **\* .blob.core.windows.net** (yleismerkki edustaa vientityön yksilöllistä tunnistetta).</span><span class="sxs-lookup"><span data-stu-id="294e5-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="294e5-113">Sinulle määritetään vientirooli Microsoft 365:n tietoturvan &amp; yhteensopivuuskeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="294e5-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="294e5-114">Tämä rooli määritetään oletusarvoisesti vain eDiscovery Manager -rooliryhmään.</span><span class="sxs-lookup"><span data-stu-id="294e5-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="294e5-115">Katso [eDiscovery-oikeuksien määrittäminen.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="294e5-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="294e5-116">Lisätietoja on kohdassa [Sisältöhaun tulosten vieminen.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="294e5-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="294e5-117">Jos viet yli 100 000 000 postilaatikkoa, sinun on ladattava vientitulokset seuraavan PowerShellin avulla: Tulosten vieminen yli [100 000 000 postilaatikosta.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="294e5-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>