---
title: 2010-hyväksymistyönkulkua ei voi lisätä
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582844"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="c2157-102">2010-hyväksymistyönkulkua ei voi lisätä</span><span class="sxs-lookup"><span data-stu-id="c2157-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="c2157-103">Microsoft SharePoint -sivustokokoelmassa ei voi lisätä luetteloon tai kirjastoon yleisesti uudelleenkäytettävää työnkulkua (kuten Hyväksyminen - SharePoint 2010).</span><span class="sxs-lookup"><span data-stu-id="c2157-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="c2157-104">Voit ratkaista tämän ongelman seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="c2157-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="c2157-105">Avaa sivustokokoelman pääsivusto SharePoint Designer 2013:ssa.</span><span class="sxs-lookup"><span data-stu-id="c2157-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="c2157-106">Valitse **Sivustoobjektit -kohdasta** **Työnkulut**.</span><span class="sxs-lookup"><span data-stu-id="c2157-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="c2157-107">Valitse **Työnkulut-valintanauhan** **Uusi-osassa** **Uudelleenkäytettävä työnkulku**.</span><span class="sxs-lookup"><span data-stu-id="c2157-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="c2157-108">Kirjoita **Luo uudelleenkäytettävä työnkulku** -lomakkeeseen nimi \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="c2157-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="c2157-109">Valitse **käyttöympäristön tyypiksi** **SharePoint 2010 -työnkulku**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="c2157-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="c2157-110">Valitse **Työnkulun** valintanauhan **Tallenna-osassa** **Julkaise**.</span><span class="sxs-lookup"><span data-stu-id="c2157-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="c2157-111">Valitse **Työnkulun** valintanauhan **Hallinta-osassa** **Julkaise yleisesti**.</span><span class="sxs-lookup"><span data-stu-id="c2157-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="c2157-112">Valitse näyttöön tulevasta vahvistusvalintaikkunasta **OK**.</span><span class="sxs-lookup"><span data-stu-id="c2157-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="c2157-113">Etsi web-selaimessa sivustokokoelman pääsivusto ja käytä **sitten Sivustoasetusten** \> **sivustokokoelman ominaisuuksia**.</span><span class="sxs-lookup"><span data-stu-id="c2157-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="c2157-114">Ota **Työnkulut käyttöön** -toiminto käytöstä:</span><span class="sxs-lookup"><span data-stu-id="c2157-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="c2157-115">· Jos ominaisuus on *aktivoitu,* valitse **Poista aktivointi** ja valitse sitten **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="c2157-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="c2157-116">· Jos ominaisuus on *poistettu käytöstä,* valitse **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="c2157-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="c2157-117">Lisätietoja on seuraavassa [artikkelissa](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c2157-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

