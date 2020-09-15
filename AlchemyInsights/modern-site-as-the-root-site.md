---
title: Moderni sivusto pääsivustona
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666867"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="e8a26-102">Moderni sivusto pääsivustona</span><span class="sxs-lookup"><span data-stu-id="e8a26-102">Modern site as root site</span></span>

<span data-ttu-id="e8a26-103">Olemme alkaneet ottaa käyttöön uuden ominaisuuden, jonka avulla voit [vaihtaa perinteisen sivuston pääsivustoa modernilla sivustolla](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="e8a26-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="e8a26-104">Käytä [Invoke-SPOSiteSwap-](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) vaihto pistettä, jos haluat vaihtaa sivuston sijainnin toiseen sivustoon arkistoitaessa alkuperäistä sivustoa.</span><span class="sxs-lookup"><span data-stu-id="e8a26-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="e8a26-105">Saatavilla sekä Ryhmäsivustolle (ei yhdistetty ryhmään) että Viestintäsivustoon.</span><span class="sxs-lookup"><span data-stu-id="e8a26-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="e8a26-106">Älä poista perinteistä pääsivustoa nykyaikaisen Viestintäsivuston luomi seksi.</span><span class="sxs-lookup"><span data-stu-id="e8a26-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="e8a26-107">Microsoft ei tue tätä.</span><span class="sxs-lookup"><span data-stu-id="e8a26-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="e8a26-108">Kun pääsivusto poistetaan, kaikki organisaation SharePoint-sivustot eivät ole kaikkien käyttäjien käytettävissä, ennen kuin palautat sivuston tai luot uuden sivuston samaan URL-osoitteeseen.</span><span class="sxs-lookup"><span data-stu-id="e8a26-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="e8a26-109">Ilmoitamme tästä ominaisuudesta viesti keskuksen kautta.</span><span class="sxs-lookup"><span data-stu-id="e8a26-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="e8a26-110">Sinun pitäisi odottaa, että ominaisuus otetaan käyttöön vuokra ajassa pian.</span><span class="sxs-lookup"><span data-stu-id="e8a26-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="e8a26-111">Sivuston vaihtamisen tunnetut ongelmat</span><span class="sxs-lookup"><span data-stu-id="e8a26-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="e8a26-112">Kohdesivusto voi palauttaa lyhyen ajan "not found" (HTTP 404)-virheen.</span><span class="sxs-lookup"><span data-stu-id="e8a26-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="e8a26-113">Sisältö on määritettävä uudelleen, jotta haku indeksiä voi päivittää.</span><span class="sxs-lookup"><span data-stu-id="e8a26-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="e8a26-114">Tässä ei tarvita manuaalista vaihetta, tämä tapahtuu automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="e8a26-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="e8a26-115">Kaikki staattisista linkeistä riippuvat (kuten tiedostojen synkronointi ja OneNote-tiedostot) on korjattava manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="e8a26-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="e8a26-116">Project Server-sivustot on ehkä vahvistettava sen varmistamiseksi, että ne liitetään edelleen oikein.</span><span class="sxs-lookup"><span data-stu-id="e8a26-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
