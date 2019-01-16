---
title: 2010 hyväksynnän työnkulun lisääminen ei onnistu
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287568"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="31259-102">2010 hyväksynnän työnkulun lisääminen ei onnistu</span><span class="sxs-lookup"><span data-stu-id="31259-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="31259-103">Microsoft SharePoint-sivustokokoelman luetteloon tai kirjastoon voi lisätä yleisesti Uudelleenkäytettävä työnkulku (kuten ”hyväksyminen - SharePoint 2010”).</span><span class="sxs-lookup"><span data-stu-id="31259-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="31259-104">Voit ratkaista tämän ongelman seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="31259-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="31259-105">Avaa sivustokokoelman päätason Web-sivuston SharePoint Designerissa 2013.</span><span class="sxs-lookup"><span data-stu-id="31259-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="31259-106">**Sivuston objektit**Valitse **Työnkulut**.</span><span class="sxs-lookup"><span data-stu-id="31259-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="31259-107">**Uusi** valintanauhan **Työnkulut** -kohdassa Valitse **Uudelleenkäytettävä työnkulku**.</span><span class="sxs-lookup"><span data-stu-id="31259-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="31259-p101">**Luo Uudelleenkäytettävä työnkulku** -lomakkeessa, kirjoita nimi \*\* *Repair2010* \*\*. **Platform tyyppi** **SharePoint 2010 työnkulun**, ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="31259-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="31259-110">**Tallenna** -osassa **työnkulun** valintanauhan Valitse **Julkaise**.</span><span class="sxs-lookup"><span data-stu-id="31259-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="31259-p102">Valitse valintanauhan **työnkulun** **hallinta** -osasta **Julkaise yleisesti**. Vahvistus valintaikkunassa, joka tulee näkyviin Valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="31259-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="31259-p103">Etsi sivustokokoelman päätason Web-sivun web-selaimessa ja käyttää **Sivuston asetukset** \> **Sivustokokoelmaominaisuudet**. Vaihda **Työnkulut** -ominaisuus:</span><span class="sxs-lookup"><span data-stu-id="31259-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="31259-115">· Jos ominaisuus on *aktivoitu* , valitse **Poista käytöstä,** ja valitse sitten **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="31259-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="31259-116">· Jos ominaisuus on *aktivointi poistetaan* , valitse **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="31259-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="31259-117">Saat lisätietoja tutustu seuraavassa [artikkelissa](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="31259-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

