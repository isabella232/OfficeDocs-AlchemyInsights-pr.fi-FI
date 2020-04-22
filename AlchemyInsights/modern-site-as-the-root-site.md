---
title: Moderni sivusto pääsivustona
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713788"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="9c91b-102">Moderni sivusto pääsivustona</span><span class="sxs-lookup"><span data-stu-id="9c91b-102">Modern site as root site</span></span>

<span data-ttu-id="9c91b-103">Olemme alkaneet ottaa käyttöön uusi ominaisuus, jonka avulla voit [vaihtaa klassinen sivuston juuri sivuston moderni sivusto](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="9c91b-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="9c91b-104">[Käytä Invoke-SPOSiteSwapia](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) sivuston sijainnin vaihtamiseen toisen sivuston kanssa alkuperäisen sivuston arkistoimisen aikana.</span><span class="sxs-lookup"><span data-stu-id="9c91b-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="9c91b-105">Käytettävissä sekä ryhmäsivustossa (ei yhdistettynä ryhmään) että viestintäsivustossa.</span><span class="sxs-lookup"><span data-stu-id="9c91b-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="9c91b-106">Älä poista perinteistä pääsivustoasi luodaksesi modernin viestintäsivuston.</span><span class="sxs-lookup"><span data-stu-id="9c91b-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="9c91b-107">Microsoft ei tue tätä.</span><span class="sxs-lookup"><span data-stu-id="9c91b-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="9c91b-108">Pääsivuston poistaminen tekee kaikista organisaation SharePoint-sivustoista kaikkien käyttäjien käytettävissä, kunnes palautat sivuston tai luot uuden sivuston samaan URL-osoitteeseen.</span><span class="sxs-lookup"><span data-stu-id="9c91b-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="9c91b-109">Kommunikoimme tämän ominaisuuden viestikeskuksen kautta.</span><span class="sxs-lookup"><span data-stu-id="9c91b-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="9c91b-110">Sinun pitäisi odottaa, että ominaisuus otetaan pian käyttöön vuokraajassasi.</span><span class="sxs-lookup"><span data-stu-id="9c91b-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="9c91b-111">Sivustojen vaihtamisen tunnetut ongelmat</span><span class="sxs-lookup"><span data-stu-id="9c91b-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="9c91b-112">Kohdesivusto saattaa palauttaa http 404 (ei löydy) -virheen lyhyeksi ajaksi.</span><span class="sxs-lookup"><span data-stu-id="9c91b-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="9c91b-113">Hakuindeksin päivittäminen edellyttää sisällön indeksointia uudelleen.</span><span class="sxs-lookup"><span data-stu-id="9c91b-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="9c91b-114">Ei ole manuaalista vaihetta tarvitaan täällä, tämä tehdään automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="9c91b-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="9c91b-115">Kaikki staattisesta linkistä riippuvaiset linkit (kuten Tiedostojen synkronointi ja OneNote-tiedostot) on korjattava manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="9c91b-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="9c91b-116">Project Server -sivustot on ehkä vahvistettava, jotta ne voidaan edelleen liittää oikein.</span><span class="sxs-lookup"><span data-stu-id="9c91b-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
