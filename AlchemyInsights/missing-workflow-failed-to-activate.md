---
title: Puuttuva työnkulku ei onnistunut aktivoimaan
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762098"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="d9137-102">Puuttuva työnkulku ei onnistunut aktivoimaan</span><span class="sxs-lookup"><span data-stu-id="d9137-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="d9137-103">Microsoft SharePoint -sivustokokoelmassa ei voi lisätä luetteloon tai kirjastoon yleisesti uudelleenkäytettävää työnkulkua (kuten Hyväksyntä - SharePoint 2010).</span><span class="sxs-lookup"><span data-stu-id="d9137-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="d9137-104">Voit ratkaista tämän ongelman seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="d9137-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="d9137-105">Avaa sivustokokoelman pääsivusto SharePoint Designer 2013:ssa.</span><span class="sxs-lookup"><span data-stu-id="d9137-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="d9137-106">Valitse **Sivustoobjektit**-kohdassa **Työnkulut**.</span><span class="sxs-lookup"><span data-stu-id="d9137-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="d9137-107">Valitse **Työnkulut-valintanauhan** **Uusi-osassa** **Uudelleenkäytettävä työnkulku**.</span><span class="sxs-lookup"><span data-stu-id="d9137-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="d9137-108">Kirjoita **Luo uudelleenkäytettävä työnkulku -lomakkeeseen** nimi \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="d9137-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="d9137-109">Valitse **Ympäristötyyppi**-kohdassa **SharePoint 2010 Workflow**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="d9137-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="d9137-110">Valitse **Työnkulun** valintanauhan **Tallenna** -osassa **Julkaise**.</span><span class="sxs-lookup"><span data-stu-id="d9137-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="d9137-111">Valitse **Työnkulku-valintanauhan** **Hallinta-osassa** **Julkaise yleisesti**.</span><span class="sxs-lookup"><span data-stu-id="d9137-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="d9137-112">Valitse näyttöön tulevasta vahvistusvalintaikkunasta **OK**.</span><span class="sxs-lookup"><span data-stu-id="d9137-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="d9137-113">Etsi web-selaimessa sivustokokoelman pääsivusto ja avaa **sivustoasetusten** \> **sivustokokoelman ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="d9137-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="d9137-114">Vaihda sitten **Työnkulut-ominaisuutta:**</span><span class="sxs-lookup"><span data-stu-id="d9137-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="d9137-115">· Jos ominaisuus on *Aktivoitu* , valitse **Poista aktivointi** ja valitse sitten **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="d9137-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="d9137-116">· Jos toiminto on *poistettu käytöstä* , valitse **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="d9137-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="d9137-117">Lisätietoja on seuraavassa [artikkelissa](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="d9137-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

