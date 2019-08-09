---
title: Työnkulku ei käynnisty
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
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270777"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="49e5e-102">Työnkulku ei käynnisty</span><span class="sxs-lookup"><span data-stu-id="49e5e-102">Workflow is not starting</span></span>

- <span data-ttu-id="49e5e-103">SharePoint 2010 ja SharePoint 2013-työnkulkuja ei käynnisty.</span><span class="sxs-lookup"><span data-stu-id="49e5e-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="49e5e-104">Jos työnkulku ei käynnisty, saattaa olla väliaikaista palvelua ongelma jossa käyttäjät saattavat kohdata ajoittaiset viiveet työnkulun edistymistä.</span><span class="sxs-lookup"><span data-stu-id="49e5e-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="49e5e-105">Tarkista [Palvelun terveyden Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) Nähdäksesi Jos organisaatiosi iskuja.</span><span class="sxs-lookup"><span data-stu-id="49e5e-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="49e5e-106">Jos on kulunut yli 24 tuntia näit tämän ongelman, kirjaudu support ticket.</span><span class="sxs-lookup"><span data-stu-id="49e5e-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="49e5e-107">Monissa tapauksissa olemme jo käsittelet ratkaisua.</span><span class="sxs-lookup"><span data-stu-id="49e5e-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="49e5e-108">Antakaa meille vähintään 24 tuntia ratkaisua.</span><span class="sxs-lookup"><span data-stu-id="49e5e-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="49e5e-109">SharePoint 2010: n työnkulkujen viivästynyt aloituksesta.</span><span class="sxs-lookup"><span data-stu-id="49e5e-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="49e5e-110">Tämä tapahtuu, jos työnkulku käynnistyy suurissa erissä.</span><span class="sxs-lookup"><span data-stu-id="49e5e-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="49e5e-111">(esimerkiksi, kun useita kohteita lisätään samalla kertaa).</span><span class="sxs-lookup"><span data-stu-id="49e5e-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="49e5e-112">Työnkulkuja ei ole suunniteltu suoritettavaksi reaaliaikaisesti, joten viive on rakenne, toiminta.</span><span class="sxs-lookup"><span data-stu-id="49e5e-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="49e5e-113">Jos työnkulku on monimutkaisten Extensible objektin Markup Language (XMOL), käännös voi olla hidas.</span><span class="sxs-lookup"><span data-stu-id="49e5e-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="49e5e-114">Tarkista [tämän](https://support.microsoft.com/en-us/kb/3043697) artikkelin.</span><span class="sxs-lookup"><span data-stu-id="49e5e-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="49e5e-115">Olisi yksinkertaista työnkulun tai suunnitella uudelleen käyttämällä Microsoft SharePoint 2013 ympäristö työnkulkutyypin.</span><span class="sxs-lookup"><span data-stu-id="49e5e-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="49e5e-116">Jos työnkulun historian on kasvanut suuri, haluat ehkä tyhjentää kohteet tai Luo uusi historialuettelo.</span><span class="sxs-lookup"><span data-stu-id="49e5e-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="49e5e-117">Lisätietoja: [Tyhjennä Työnkulkuhistoria](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="49e5e-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="49e5e-118">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="49e5e-118">Related topics</span></span>
<span data-ttu-id="49e5e-119">Jos haluat kokeilla Microsoft SharePoint Online-Flow?</span><span class="sxs-lookup"><span data-stu-id="49e5e-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="49e5e-120">Luo työnkulku</span><span class="sxs-lookup"><span data-stu-id="49e5e-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="49e5e-121">SharePoint- ja</span><span class="sxs-lookup"><span data-stu-id="49e5e-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


