---
title: Työnkulku ei käynnisty
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403740"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="b5393-102">Työnkulku ei käynnisty</span><span class="sxs-lookup"><span data-stu-id="b5393-102">Workflow is not starting</span></span>

- <span data-ttu-id="b5393-103">SharePoint 2010- ja SharePoint 2013 -työnkulut eivät käynnisty.</span><span class="sxs-lookup"><span data-stu-id="b5393-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="b5393-104">Jos työnkulku ei käynnisty, saattaa olla tilapäinen palveluongelma, jossa käyttäjillä voi olla ajoittaista viivettä työnkulun edistyessä.</span><span class="sxs-lookup"><span data-stu-id="b5393-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="b5393-105">Tarkista Palvelun [kunto -koontinäytöstä,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) vaikuttaako se organisaatioosi.</span><span class="sxs-lookup"><span data-stu-id="b5393-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="b5393-106">Jos yli 24 tuntia on kulunut siitä, kun näit tämän ongelman ensimmäisen kerran, kirjaudu tukipalveluun.</span><span class="sxs-lookup"><span data-stu-id="b5393-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="b5393-107">Monissa tapauksissa ratkaisua on jo ennestään valmis.</span><span class="sxs-lookup"><span data-stu-id="b5393-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b5393-108">Anna meille vähintään 24 tuntia aikaa ratkaisun suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="b5393-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="b5393-109">SharePoint 2010 -työnkulut viivästyivät alusta.</span><span class="sxs-lookup"><span data-stu-id="b5393-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="b5393-110">Näin tapahtuu, jos työnkulku käynnistyy suurissa erissä.</span><span class="sxs-lookup"><span data-stu-id="b5393-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="b5393-111">(esimerkiksi kun useita kohteita lisätään kerralla).</span><span class="sxs-lookup"><span data-stu-id="b5393-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="b5393-112">Työnkulkuja ei ole suunniteltu suoritettavaksi reaaliaikaisesti, joten viive on suunnittelun mukaan suoritettava toimintatapa.</span><span class="sxs-lookup"><span data-stu-id="b5393-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="b5393-113">Jos työnkulku on monimutkainen XHAUN (Extensible Object Markup Language) -kieli, kääntäminen voi olla hidasta.</span><span class="sxs-lookup"><span data-stu-id="b5393-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="b5393-114">Tutustu [tähän artikkeliin.](https://support.microsoft.com//kb/3043697)</span><span class="sxs-lookup"><span data-stu-id="b5393-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="b5393-115">Sinun kannattaa yksinkertaistaa työnkulkua tai suunnitella se uudelleen Microsoft SharePoint 2013 -työnkulkuympäristön tyypin avulla.</span><span class="sxs-lookup"><span data-stu-id="b5393-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="b5393-116">Jos työnkulun historia on kasvanut suureksi, haluat ehkä tyhjentää kohteet tai luoda uuden historialuettelon.</span><span class="sxs-lookup"><span data-stu-id="b5393-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="b5393-117">Lisätietoja: [Työnkulun historian tyhjentäminen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="b5393-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="b5393-118">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="b5393-118">Related topics</span></span>
<span data-ttu-id="b5393-119">Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="b5393-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="b5393-120">Työnkulun luominen</span><span class="sxs-lookup"><span data-stu-id="b5393-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="b5393-121">SharePoint ja Työnkulku</span><span class="sxs-lookup"><span data-stu-id="b5393-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
