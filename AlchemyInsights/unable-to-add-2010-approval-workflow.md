---
title: 2010-hyväksynnän työn kulkua ei voi lisätä
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049550"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="61895-102">2010-hyväksynnän työn kulkua ei voi lisätä</span><span class="sxs-lookup"><span data-stu-id="61895-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="61895-103">Microsoft SharePoint-sivustokokoelmassa ei voi lisätä yleisesti uudelleenkäytettävää työn kulkua (kuten "hyväksyntä-SharePoint 2010") luetteloon tai kirjastoon.</span><span class="sxs-lookup"><span data-stu-id="61895-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="61895-104">Voit ratkaista tämän ongelman tekemällä seuraavat toimet:</span><span class="sxs-lookup"><span data-stu-id="61895-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="61895-105">Avaa sivustokokoelman pääsivusto SharePoint Designerissa 2013.</span><span class="sxs-lookup"><span data-stu-id="61895-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="61895-106">Valitse **Sivustoobjektit**-kohdassa **työn kulut**.</span><span class="sxs-lookup"><span data-stu-id="61895-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="61895-107">Valitse **työn kulkujen** valinta nauhan **Uusi** -osasta **uudelleenkäytettävä työn kulku**.</span><span class="sxs-lookup"><span data-stu-id="61895-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="61895-108">Kirjoita **Luo uudelleen käytettävä työn kulku** -lomakkeeseen nimi \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="61895-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="61895-109">Valitse **alustan tyypille** **SharePoint 2010-työn kulku**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="61895-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="61895-110">Valitse **työn kulun** valinta nauhan **Tallenna** -osasta **Julkaise**.</span><span class="sxs-lookup"><span data-stu-id="61895-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="61895-111">Valitse **työn kulun** valinta nauhan **hallinta** -osasta **Julkaise maailmanlaajuisesti**.</span><span class="sxs-lookup"><span data-stu-id="61895-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="61895-112">Valitse avautuvassa vahvistus ikkunassa **OK**.</span><span class="sxs-lookup"><span data-stu-id="61895-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="61895-113">Etsi Web-selaimessa sivustokokoelman pääsivusto ja avaa sitten **sivuston asetusten** \> sivustokokoelman **Ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="61895-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="61895-114">Vaihda **työn kulut** -toiminto:</span><span class="sxs-lookup"><span data-stu-id="61895-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="61895-115">· Jos ominaisuus on *aktivoitu* , valitse **Poista Akti vointi** ja valitse sitten **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="61895-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="61895-116">· Jos toiminto on *poistettu käytöstä* , valitse **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="61895-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="61895-117">Katso lisä tietoja seuraavasta [artikkelista](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="61895-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

