---
title: Moderni sivusto kuin pääsivusto
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054699"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="a2517-102">Moderni sivusto pääsivusto</span><span class="sxs-lookup"><span data-stu-id="a2517-102">Modern site as root site</span></span>

<span data-ttu-id="a2517-103">Olemme alkaneet ottaa käyttöön uuden ominaisuuden, jonka avulla voit [vaihtaa klassisen sivuston juuri sivuston modernilla sivustolla](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="a2517-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="a2517-104">Käytä [Kutsu-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , jos haluat vaihtaa sivuston sijainnin toisen sivuston kanssa arkistoitaessa alkuperäistä sivustoa.</span><span class="sxs-lookup"><span data-stu-id="a2517-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="a2517-105">Käytettävissä sekä ryhmäsivustoon (ei yhdistetty ryhmään) että viestintä sivustoon.</span><span class="sxs-lookup"><span data-stu-id="a2517-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="a2517-106">Älä poista klassista pääsivustoa, jotta voit luoda nykyaikaisen viestintä paikan.</span><span class="sxs-lookup"><span data-stu-id="a2517-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="a2517-107">Microsoft ei tue tätä.</span><span class="sxs-lookup"><span data-stu-id="a2517-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="a2517-108">Pääsivuston poistaminen tekee kaikista organisaatioosi kuuluvista SharePoint-sivustoista kaikkien käyttäjien käytettävissä, kunnes palautat sivuston tai luot uuden sivuston samaan URL-osoitteeseen.</span><span class="sxs-lookup"><span data-stu-id="a2517-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="a2517-109">Viestimme tästä ominaisuudesta viesti keskuksen kautta.</span><span class="sxs-lookup"><span data-stu-id="a2517-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="a2517-110">Odota, että ominaisuus on käytössä vuokraajassasi lähiaikoina.</span><span class="sxs-lookup"><span data-stu-id="a2517-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="a2517-111">Sivustojen vaihtamisen tunnetut ongelmat</span><span class="sxs-lookup"><span data-stu-id="a2517-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="a2517-112">Kohde sivusto saattaa palauttaa virheen "ei löytynyt" (HTTP 404), joka on lyhyt ajan jakso.</span><span class="sxs-lookup"><span data-stu-id="a2517-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="a2517-113">Sisältö on indeksoida uudelleen, jotta haku indeksi voidaan päivittää.</span><span class="sxs-lookup"><span data-stu-id="a2517-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="a2517-114">Tässä ei ole manuaalista vaihetta, tämä tapahtuu automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="a2517-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="a2517-115">Kaikki, jotka ovat riippuvaisia "staattisista" linkeistä (kuten tiedostojen synkronointi ja OneNote-tiedostot), on korjattava manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="a2517-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="a2517-116">Project Server-sivustot on ehkä validoitava sen varmistamiseksi, että ne liittyvät edelleen oikein.</span><span class="sxs-lookup"><span data-stu-id="a2517-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
