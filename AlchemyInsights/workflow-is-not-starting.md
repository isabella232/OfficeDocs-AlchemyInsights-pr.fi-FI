---
title: Työnkulku ei käynnisty
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766094"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="b3358-102">Työnkulku ei käynnisty</span><span class="sxs-lookup"><span data-stu-id="b3358-102">Workflow is not starting</span></span>

- <span data-ttu-id="b3358-103">SharePoint 2010- ja SharePoint 2013 -työnkulut eivät käynnisty.</span><span class="sxs-lookup"><span data-stu-id="b3358-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="b3358-104">Jos työnkulku ei käynnisty, työnkulussa saattaa ilmetä tilapäinen palveluongelma.</span><span class="sxs-lookup"><span data-stu-id="b3358-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="b3358-105">Tarkista [palvelun kunnon hallintapaneelista,](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) vaikuttaako organisaatiosi organisaatioon.</span><span class="sxs-lookup"><span data-stu-id="b3358-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="b3358-106">Jos tämän ongelman ensimmäisestä näkemästäsi on kulunut yli 24 tuntia, kirjaudu tukilipusta.</span><span class="sxs-lookup"><span data-stu-id="b3358-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="b3358-107">Monissa tapauksissa olemme jo työstänyt ratkaisua.</span><span class="sxs-lookup"><span data-stu-id="b3358-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b3358-108">Anna meille vähintään 24 tuntia ratkaisun viimeistelemiseksi.</span><span class="sxs-lookup"><span data-stu-id="b3358-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="b3358-109">SharePoint 2010 -työnkulut viivästyivät käynnistyksen.</span><span class="sxs-lookup"><span data-stu-id="b3358-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="b3358-110">Näin tapahtuu, jos työnkulku käynnistyy suurissa erissä.</span><span class="sxs-lookup"><span data-stu-id="b3358-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="b3358-111">(esimerkiksi, kun useita kohteita lisätään kerralla).</span><span class="sxs-lookup"><span data-stu-id="b3358-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="b3358-112">Työnkulkuja ei ole suunniteltu toimimaan reaaliaikaisesti, joten viive on suunnittelukäyttäytyminen.</span><span class="sxs-lookup"><span data-stu-id="b3358-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="b3358-113">Jos työnkulku on monimutkainen XMOL (Extensible Object Markup Language) -kieli, kääntäminen voi olla hidasta.</span><span class="sxs-lookup"><span data-stu-id="b3358-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="b3358-114">Tarkista [tämä](https://support.microsoft.com//kb/3043697) artikkeli.</span><span class="sxs-lookup"><span data-stu-id="b3358-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="b3358-115">Yksinkertaista työnkulkua tai suunnittele se uudelleen Microsoft SharePoint 2013 Workflow -ympäristötyypin avulla.</span><span class="sxs-lookup"><span data-stu-id="b3358-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="b3358-116">Jos työnkulkuhistoriaon kasvanut suuri, haluat ehkä tyhjentää kohteet tai luoda uuden historialuettelon.</span><span class="sxs-lookup"><span data-stu-id="b3358-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="b3358-117">Lisätietoja : [Työnkulun historian puhdistaminen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="b3358-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="b3358-118">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="b3358-118">Related topics</span></span>
<span data-ttu-id="b3358-119">Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="b3358-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="b3358-120">Luo työnkulku</span><span class="sxs-lookup"><span data-stu-id="b3358-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="b3358-121">SharePoint ja Flow</span><span class="sxs-lookup"><span data-stu-id="b3358-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


