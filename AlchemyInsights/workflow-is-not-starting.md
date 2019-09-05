---
title: Työn kulku ei käynnistyi
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738086"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="f45b0-102">Työn kulku ei käynnistyi</span><span class="sxs-lookup"><span data-stu-id="f45b0-102">Workflow is not starting</span></span>

- <span data-ttu-id="f45b0-103">SharePoint 2010 ja SharePoint 2013-työn kulut eivät käynnistyi.</span><span class="sxs-lookup"><span data-stu-id="f45b0-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="f45b0-104">Jos työn kulku ei ole käynnistyminen, saattaa olla tilapäinen palvelu ongelma, jossa käyttäjät saattavat kohdata ajoittaisia viiveitä työn kulun edistymisen kanssa.</span><span class="sxs-lookup"><span data-stu-id="f45b0-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="f45b0-105">Tarkista [palvelun kunnon koonti näytöstä](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , onko organisaatiossasi vaikutusta.</span><span class="sxs-lookup"><span data-stu-id="f45b0-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="f45b0-106">Jos tämän ongelman ensimmäisen näkemis kerran jälkeen on kulunut yli 24 tuntia, kirjaudu tuki lippuun.</span><span class="sxs-lookup"><span data-stu-id="f45b0-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="f45b0-107">Monissa tapa uksissa olemme jo tekemässä ratkaisua.</span><span class="sxs-lookup"><span data-stu-id="f45b0-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f45b0-108">Ole hyvä ja anna meille vähintään 24 tuntia aikaa ratkaisun suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="f45b0-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="f45b0-109">SharePoint 2010-työn kulut viivästyivät käynnistyksen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="f45b0-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="f45b0-110">Näin tapahtuu, jos työn kulku käynnistetään suurissa erissä.</span><span class="sxs-lookup"><span data-stu-id="f45b0-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="f45b0-111">(esimerkiksi kun useita kohteita lisätään kerralla).</span><span class="sxs-lookup"><span data-stu-id="f45b0-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="f45b0-112">Työn kulkuja ei ole suunniteltu suorittamaan reaaliaikaista toimintaa, joten viive on suunnittelun mukaan suoritettava.</span><span class="sxs-lookup"><span data-stu-id="f45b0-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="f45b0-113">Jos työn kulku on monimutkainen XMOL (Extensible Object Markup Language)-kieli, kääntäminen voi olla hidasta.</span><span class="sxs-lookup"><span data-stu-id="f45b0-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="f45b0-114">Tarkista [Tämä](https://support.microsoft.com//kb/3043697) artikkeli.</span><span class="sxs-lookup"><span data-stu-id="f45b0-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="f45b0-115">Yksinkertaista työn kulkua tai Suunnittele se uudelleen käyttämällä Microsoft SharePoint 2013-työn kulku ympäristön tyyppiä.</span><span class="sxs-lookup"><span data-stu-id="f45b0-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="f45b0-116">Jos työn kulku historiasi on kasvanut suureksi, haluat ehkä tyhjentää kohteet tai luoda uuden historia luettelon.</span><span class="sxs-lookup"><span data-stu-id="f45b0-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="f45b0-117">Lisä tietoja: [työn kulku historian Tyhjentuminen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="f45b0-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="f45b0-118">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="f45b0-118">Related topics</span></span>
<span data-ttu-id="f45b0-119">Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="f45b0-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="f45b0-120">Luo työn kulku</span><span class="sxs-lookup"><span data-stu-id="f45b0-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="f45b0-121">SharePoint ja Flow</span><span class="sxs-lookup"><span data-stu-id="f45b0-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


