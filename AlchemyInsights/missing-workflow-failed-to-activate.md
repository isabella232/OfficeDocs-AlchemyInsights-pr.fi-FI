---
title: Puuttuva työn kulku ei voinut aktivoitua
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052610"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="3db3b-102">Puuttuva työn kulku ei voinut aktivoitua</span><span class="sxs-lookup"><span data-stu-id="3db3b-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="3db3b-103">Microsoft SharePoint-sivustokokoelmassa ei voi lisätä yleisesti uudelleenkäytettävää työn kulkua (kuten "hyväksyntä-SharePoint 2010") luetteloon tai kirjastoon.</span><span class="sxs-lookup"><span data-stu-id="3db3b-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="3db3b-104">Voit ratkaista tämän ongelman tekemällä seuraavat toimet:</span><span class="sxs-lookup"><span data-stu-id="3db3b-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="3db3b-105">Avaa sivustokokoelman pääsivusto SharePoint Designerissa 2013.</span><span class="sxs-lookup"><span data-stu-id="3db3b-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="3db3b-106">Valitse **Sivustoobjektit**-kohdassa **työn kulut**.</span><span class="sxs-lookup"><span data-stu-id="3db3b-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="3db3b-107">Valitse **työn kulkujen** valinta nauhan **Uusi** -osasta **uudelleenkäytettävä työn kulku**.</span><span class="sxs-lookup"><span data-stu-id="3db3b-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="3db3b-108">Kirjoita **Luo uudelleen käytettävä työn kulku** -lomakkeeseen nimi \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="3db3b-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="3db3b-109">Valitse **alustan tyypille** **SharePoint 2010-työn kulku**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="3db3b-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="3db3b-110">Valitse **työn kulun** valinta nauhan **Tallenna** -osasta **Julkaise**.</span><span class="sxs-lookup"><span data-stu-id="3db3b-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="3db3b-111">Valitse **työn kulun** valinta nauhan **hallinta** -osasta **Julkaise maailmanlaajuisesti**.</span><span class="sxs-lookup"><span data-stu-id="3db3b-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="3db3b-112">Valitse avautuvassa vahvistus ikkunassa **OK**.</span><span class="sxs-lookup"><span data-stu-id="3db3b-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="3db3b-113">Etsi Web-selaimessa sivustokokoelman pääsivusto ja avaa sitten **sivuston asetusten** \> sivustokokoelman **Ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="3db3b-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="3db3b-114">Vaihda sitten **työn kulut** -toiminto:</span><span class="sxs-lookup"><span data-stu-id="3db3b-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="3db3b-115">· Jos ominaisuus on *aktivoitu* , valitse **Poista Akti vointi** ja valitse sitten **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="3db3b-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="3db3b-116">· Jos toiminto on *poistettu käytöstä* , valitse **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="3db3b-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="3db3b-117">Katso lisä tietoja seuraavasta [artikkelista](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="3db3b-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

