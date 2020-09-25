---
title: eDiscoveryn vienti työkalu
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277939"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="24671-102">Etkö voi asentaa tai suorittaa eDiscoveryn vienti työkalua?</span><span class="sxs-lookup"><span data-stu-id="24671-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="24671-103">Jos et voi asentaa tai käyttää eDiscoveryn vienti työkalua haku tulosten lataamiseen, tarkista seuraavat asiat:</span><span class="sxs-lookup"><span data-stu-id="24671-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="24671-104">Käyttämäsi tieto kone täyttää seuraavat vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="24671-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="24671-105">32-tai 64-bittiset Windows 7-versiot ja uudemmat versiot</span><span class="sxs-lookup"><span data-stu-id="24671-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="24671-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="24671-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="24671-107">Tuetulla selaimella:</span><span class="sxs-lookup"><span data-stu-id="24671-107">A supported browser:</span></span>

  - <span data-ttu-id="24671-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="24671-108">Microsoft Edge</span></span>

    <span data-ttu-id="24671-109">TAI</span><span class="sxs-lookup"><span data-stu-id="24671-109">Or</span></span>

  - <span data-ttu-id="24671-110">Internet Explorer 10 ja uudemmat versiot</span><span class="sxs-lookup"><span data-stu-id="24671-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="24671-111">Muita selaimia, kuten Google Chromea ja Mozilla Firefoxia, ei voi tukea.</span><span class="sxs-lookup"><span data-stu-id="24671-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="24671-112">Organisaatiosi voi muodostaa yhteyden Azure-pääte pisteeseen, joka on \*\* \* . blob.Core.Windows.net\*\* (Yleismerkki vastaa vienti työn yksilöllistä tunnistetta).</span><span class="sxs-lookup"><span data-stu-id="24671-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="24671-113">Olet määrittänyt vienti roolin Microsoft 365-tieto turva &amp; yhteensopivuus keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="24671-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="24671-114">Oletusarvoisesti tämä rooli määritetään vain eDiscoveryn hallinta-rooli ryhmälle.</span><span class="sxs-lookup"><span data-stu-id="24671-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="24671-115">Lisä tietoja on Ohje aiheessa [eDiscoveryn käyttö oikeuksien määrittäminen](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="24671-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="24671-116">Lisä tietoja on Ohje aiheessa [sisältö haun tulosten vieminen](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="24671-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="24671-117">Jos viet yli 100 000 posti laatikkoa, sinun on ladattava vienti tulokset seuraavan PowerShellin avulla: vie  [tulokset yli 100k posti laatikosta](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="24671-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>