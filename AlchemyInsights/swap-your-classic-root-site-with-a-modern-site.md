---
title: Vaihda Classic pääkansio sivuston Moderni sivusto
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270741"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="bb59e-102">Vaihda Classic pääkansio sivuston Moderni sivusto</span><span class="sxs-lookup"><span data-stu-id="bb59e-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="bb59e-103">Jos ympäristösi on määritetty ennen huhtikuuta 2019, voit muuttaa päätason sivustossa Moderni sivustoon käyttämällä Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="bb59e-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="bb59e-104">Jos sinulla on toinen sivusto, jota haluat käyttää oman pääsivusto, jonka korvaava (swap) pääkansio sivuston.</span><span class="sxs-lookup"><span data-stu-id="bb59e-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="bb59e-105">[Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) avulla sivuston toisen sivuston kanssa vaihdettava tallennettaessa alkuperäiseen sivustoon.</span><span class="sxs-lookup"><span data-stu-id="bb59e-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="bb59e-106">Sekä ryhmän (ei yhteyttä ryhmään) ja tiedonannon sivustojen käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="bb59e-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="bb59e-107">Lisäominaisuuksia se esitellään pian, joka mahdollistaa sivuston sisällön avulla pitää, mutta sivusto muuntaminen Viestimissivusto.</span><span class="sxs-lookup"><span data-stu-id="bb59e-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="bb59e-108">Näitä toimintoja toteutetaan vielä vähitellen.</span><span class="sxs-lookup"><span data-stu-id="bb59e-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="bb59e-109">Tarkista päivitykset Office 365 Message Center jatkaa.</span><span class="sxs-lookup"><span data-stu-id="bb59e-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="bb59e-110">Tunnettuja ongelmia vaihtamisen sivustot</span><span class="sxs-lookup"><span data-stu-id="bb59e-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="bb59e-111">Kohdesivuston saattaa palauttaa (HTTP 404) ”ei löydy” virhe lyhyen ajan kuluessa.</span><span class="sxs-lookup"><span data-stu-id="bb59e-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="bb59e-112">Sisältöä täytyy päivittää hakuindeksin tehdään uudelleen.</span><span class="sxs-lookup"><span data-stu-id="bb59e-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="bb59e-113">On manuaalinen vaihe, ei pakollinen – tämä tehdään automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="bb59e-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="bb59e-114">Mitään riippuvainen ”staattinen” linkkejä (kuten tiedoston synkronointiin ja OneNote-tiedostoja) on korjattava manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="bb59e-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="bb59e-115">Jos lähde on organisaation uutissivuston, Päivitä URL-osoite.</span><span class="sxs-lookup"><span data-stu-id="bb59e-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="bb59e-116">Näyttöön tulee luettelo sivustoja organisaatiota koskevia uutisia.</span><span class="sxs-lookup"><span data-stu-id="bb59e-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="bb59e-117">Project Server-sivustoja on ehkä tarkistettava sen varmistamiseksi, että ne liittyvät yhä oikein.</span><span class="sxs-lookup"><span data-stu-id="bb59e-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





