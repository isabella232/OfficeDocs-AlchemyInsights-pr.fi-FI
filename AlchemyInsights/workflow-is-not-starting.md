---
title: Työn kulku ei käynnisty
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794764"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="1b170-102">Työn kulku ei käynnisty</span><span class="sxs-lookup"><span data-stu-id="1b170-102">Workflow is not starting</span></span>

- <span data-ttu-id="1b170-103">SharePoint 2010 ja SharePoint 2013-työn kulut eivät käynnisty.</span><span class="sxs-lookup"><span data-stu-id="1b170-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="1b170-104">Jos työn kulku ei käynnisty, kyseessä saattaa olla väliaikainen ongelma, jossa käyttäjät saattavat kohdata ajoittaisia viiveitä työn kulun edistymisen aikana.</span><span class="sxs-lookup"><span data-stu-id="1b170-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="1b170-105">Tarkista [palvelun kunnon koonti näytöstä](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , onko organisaatiosi vaikuttanut siihen.</span><span class="sxs-lookup"><span data-stu-id="1b170-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="1b170-106">Jos sinulla on kulunut yli 24 tuntia siitä, kun olet ensimmäisen kerran nähnyt tämän ongelman, kirjaudu tuki lipulla.</span><span class="sxs-lookup"><span data-stu-id="1b170-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="1b170-107">Monissa tapa uksissa pyrimme jo ratkaisemaan ongelman.</span><span class="sxs-lookup"><span data-stu-id="1b170-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="1b170-108">Anna meille vähintään 24 tuntia aikaa ratkaisun suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="1b170-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="1b170-109">SharePoint 2010-työn kulut viivästyvät käynnistettäessä.</span><span class="sxs-lookup"><span data-stu-id="1b170-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="1b170-110">Tämä tapahtuu, jos työn kulku käynnistetään suurissa erissä.</span><span class="sxs-lookup"><span data-stu-id="1b170-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="1b170-111">(esimerkiksi kun useita kohteita lisätään kerralla).</span><span class="sxs-lookup"><span data-stu-id="1b170-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="1b170-112">Työn kulkuja ei ole suunniteltu suoritettavaksi reaaliajassa, joten viive on suunnittelu toiminto.</span><span class="sxs-lookup"><span data-stu-id="1b170-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="1b170-113">Jos työn kulku on monimutkainen eXtensible Object Markup Language (XMOL), kääntäminen voi olla hidasta.</span><span class="sxs-lookup"><span data-stu-id="1b170-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="1b170-114">Valitse [Tämä](https://support.microsoft.com//kb/3043697) artikkeli.</span><span class="sxs-lookup"><span data-stu-id="1b170-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="1b170-115">Sinun on yksinkertaistettava työn kulkua tai suunniteltava se uudelleen Microsoft SharePoint 2013-työn kulku alustan tyypin avulla.</span><span class="sxs-lookup"><span data-stu-id="1b170-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="1b170-116">Jos työn kulku historiasi on kasvanut suureksi, haluat ehkä tyhjentää kohteet tai luoda uuden historia luettelon.</span><span class="sxs-lookup"><span data-stu-id="1b170-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="1b170-117">Lisä tietoja: [työn kulku historian tyhjentäminen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="1b170-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="1b170-118">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="1b170-118">Related topics</span></span>
<span data-ttu-id="1b170-119">Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="1b170-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="1b170-120">Työn kulun luominen</span><span class="sxs-lookup"><span data-stu-id="1b170-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="1b170-121">SharePoint ja Flow</span><span class="sxs-lookup"><span data-stu-id="1b170-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


