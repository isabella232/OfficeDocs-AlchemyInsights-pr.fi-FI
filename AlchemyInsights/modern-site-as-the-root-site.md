---
title: Kuin pääsivusto nykyaikaisia sivusto
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232712"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="f96e2-102">Kuin pääsivusto nykyaikaisia sivusto</span><span class="sxs-lookup"><span data-stu-id="f96e2-102">Modern site as root site</span></span>

<span data-ttu-id="f96e2-103">Emme ole aloittaneet rahoittaja on uusi ominaisuus, joka mahdollistaa perinteinen sivuston pääkansio sivustosi Moderni sivuston kanssa vaihdettava.</span><span class="sxs-lookup"><span data-stu-id="f96e2-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="f96e2-104">[Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) avulla sivuston toisen sivuston kanssa vaihdettava tallennettaessa alkuperäiseen sivustoon.</span><span class="sxs-lookup"><span data-stu-id="f96e2-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="f96e2-105">Sekä ryhmän (ei yhteyttä ryhmään) ja tiedonannon sivustojen käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="f96e2-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="f96e2-106">Älä poista perinteinen pääsivusto luoda Nykyaikainen Viestimissivusto.</span><span class="sxs-lookup"><span data-stu-id="f96e2-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="f96e2-107">Microsoft ei tue.</span><span class="sxs-lookup"><span data-stu-id="f96e2-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="f96e2-108">Ensisijaisen säilön poistaminen tekee kaikki SharePoint-sivustot organisaation kaikkien käyttäjien käytettävissä ennen kuin palauttaa sivuston tai luoda uuden sivuston samaan URL-osoitteeseen.</span><span class="sxs-lookup"><span data-stu-id="f96e2-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="f96e2-109">Olemme yhteydessä tämän toiminnon kautta viestikeskus.</span><span class="sxs-lookup"><span data-stu-id="f96e2-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="f96e2-110">Tulee odottaa-ominaisuuden avulla voidaan ottaa käyttöön oman vuokralaisen pian.</span><span class="sxs-lookup"><span data-stu-id="f96e2-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="f96e2-111">Tunnettuja ongelmia vaihtamisen sivustot</span><span class="sxs-lookup"><span data-stu-id="f96e2-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="f96e2-112">Kohdesivuston saattaa palauttaa (HTTP 404) ”ei löydy” virhe lyhyen ajan kuluessa.</span><span class="sxs-lookup"><span data-stu-id="f96e2-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="f96e2-113">Sisältöä täytyy päivittää hakuindeksin tehdään uudelleen.</span><span class="sxs-lookup"><span data-stu-id="f96e2-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="f96e2-114">Ei ole pakollinen tässä kentässä Manuaalinen vaihe, tämä tapahtuu automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="f96e2-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="f96e2-115">Mitään riippuvainen ”staattinen” linkkejä (kuten tiedoston synkronointiin ja OneNote-tiedostoja) on korjattava manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="f96e2-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="f96e2-116">Project Server-sivustoja on ehkä tarkistettava sen varmistamiseksi, että ne liittyvät yhä oikein.</span><span class="sxs-lookup"><span data-stu-id="f96e2-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
