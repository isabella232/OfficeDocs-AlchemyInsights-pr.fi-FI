---
title: eDiscovery-/sisältöhaun tulosten vieminen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481727"
---
# <a name="export-ediscoverycontent-search-results"></a><span data-ttu-id="d3e52-102">eDiscovery-/sisältöhaun tulosten vieminen</span><span class="sxs-lookup"><span data-stu-id="d3e52-102">Export eDiscovery/Content Search results</span></span>

<span data-ttu-id="d3e52-103">Sinun on ehkä vietävä hakutulokset PST-tiedostoon (sähköpostista) tai alkuperäisiin Office-tiedostoihin (SharePoint- ja OneDrive for Business -sivustoista).</span><span class="sxs-lookup"><span data-stu-id="d3e52-103">You may need to export your search results to a PST file (from email) or to native Office documents (from SharePoint and OneDrive for Business sites).</span></span> <span data-ttu-id="d3e52-104">Jos näin on, tee näin:</span><span class="sxs-lookup"><span data-stu-id="d3e52-104">If so, do the following:</span></span>

- <span data-ttu-id="d3e52-105">Varmista, että tilillesi on määritetty asianmukaiset vientioikeudet.</span><span class="sxs-lookup"><span data-stu-id="d3e52-105">Make sure your account is assigned the proper permissions to export.</span></span> <span data-ttu-id="d3e52-106">Lisätietoja on kohdassa [eDiscovery-käyttöoikeuksien määrittäminen.](https://go.microsoft.com/fwlink/?linkid=2102406)</span><span class="sxs-lookup"><span data-stu-id="d3e52-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span></span>
- <span data-ttu-id="d3e52-107">Varmista, että tietokoneesi täyttää [kaikki edellytykset.](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin)</span><span class="sxs-lookup"><span data-stu-id="d3e52-107">Make sure your computer has met all [prerequisites](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span></span> <span data-ttu-id="d3e52-108">Kaikkia selaimia, kuten Chromea, ei tueta.</span><span class="sxs-lookup"><span data-stu-id="d3e52-108">Not all browsers are supported, such as Chrome.</span></span>
- <span data-ttu-id="d3e52-109">Vieminen sisältöhaun avulla: a.</span><span class="sxs-lookup"><span data-stu-id="d3e52-109">To export from a Content Search: a.</span></span> <span data-ttu-id="d3e52-110">Siirry [tietoturva- & yhteensopivuuskeskukseen,](https://protection.office.com/contentsearch) valitse **Hae** ja valitse sitten **Sisältöhaku.**</span><span class="sxs-lookup"><span data-stu-id="d3e52-110">Go to the [Security & Compliance Center](https://protection.office.com/contentsearch) and click **Search**, and then select **Content search**.</span></span> <span data-ttu-id="d3e52-111">Valitse **tallennettu haku** Sisältö-hakusivulla.</span><span class="sxs-lookup"><span data-stu-id="d3e52-111">On the **Content search** page, select a saved search.</span></span>
    <span data-ttu-id="d3e52-112">b.</span><span class="sxs-lookup"><span data-stu-id="d3e52-112">b.</span></span> <span data-ttu-id="d3e52-113">Valitse Tiedot-ruudun Vie **tulokset tietokoneeseen -kohdassa** Aloita **vienti.**</span><span class="sxs-lookup"><span data-stu-id="d3e52-113">On the Details pane, under **Export results to a computer**, select **Start export**.</span></span> <span data-ttu-id="d3e52-114">Jos viet yli 100 000 postilaatikkoa, sinun on ladattava vientitulokset PowerShellin avulla.</span><span class="sxs-lookup"><span data-stu-id="d3e52-114">If you're exporting more than 100K mailboxes, you'll need to use PowerShell to download the export results.</span></span> <span data-ttu-id="d3e52-115">Lisätietoja on kohdassa Yli [100 000 000 postilaatikon tulosten vieminen.](https://go.microsoft.com/fwlink/?linkid=2143861)</span><span class="sxs-lookup"><span data-stu-id="d3e52-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span></span>

<span data-ttu-id="d3e52-116">Lisätietoja on kohdassa [Sisällön hakutulosten vieminen.](https://go.microsoft.com/fwlink/?linkid=2102118)</span><span class="sxs-lookup"><span data-stu-id="d3e52-116">To learn more, see [Export Content Search Results](https://go.microsoft.com/fwlink/?linkid=2102118).</span></span>