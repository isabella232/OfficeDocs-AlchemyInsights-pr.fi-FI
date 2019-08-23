---
title: 2010 hyväksynnän työnkulun lisääminen ei onnistu
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 1f564c5d1e689dcf41b22fab5a05ab1b488c2b0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558614"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="5015b-102">2010 hyväksynnän työnkulun lisääminen ei onnistu</span><span class="sxs-lookup"><span data-stu-id="5015b-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="5015b-103">Microsoft SharePoint-sivustokokoelman luetteloon tai kirjastoon voi lisätä yleisesti Uudelleenkäytettävä työnkulku (kuten ”hyväksyminen - SharePoint 2010”).</span><span class="sxs-lookup"><span data-stu-id="5015b-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="5015b-104">Voit ratkaista tämän ongelman seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="5015b-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="5015b-105">Avaa sivustokokoelman päätason Web-sivuston SharePoint Designerissa 2013.</span><span class="sxs-lookup"><span data-stu-id="5015b-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="5015b-106">**Sivuston objektit**Valitse **Työnkulut**.</span><span class="sxs-lookup"><span data-stu-id="5015b-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="5015b-107">**Uusi** valintanauhan **Työnkulut** -kohdassa Valitse **Uudelleenkäytettävä työnkulku**.</span><span class="sxs-lookup"><span data-stu-id="5015b-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="5015b-108">**Luo Uudelleenkäytettävä työnkulku** -lomakkeessa, kirjoita nimi \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="5015b-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="5015b-109">**Platform tyyppi** **SharePoint 2010 työnkulun**, ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="5015b-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="5015b-110">**Tallenna** -osassa **työnkulun** valintanauhan Valitse **Julkaise**.</span><span class="sxs-lookup"><span data-stu-id="5015b-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="5015b-111">Valitse valintanauhan **työnkulun** **hallinta** -osasta **Julkaise yleisesti**.</span><span class="sxs-lookup"><span data-stu-id="5015b-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="5015b-112">Vahvistus valintaikkunassa, joka tulee näkyviin Valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="5015b-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="5015b-113">Etsi sivustokokoelman päätason Web-sivun web-selaimessa ja käyttää **Sivuston asetukset** \> **Sivustokokoelmaominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="5015b-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="5015b-114">Vaihda **Työnkulut** -ominaisuus:</span><span class="sxs-lookup"><span data-stu-id="5015b-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="5015b-115">· Jos ominaisuus on *aktivoitu* , valitse **Poista käytöstä,** ja valitse sitten **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="5015b-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="5015b-116">· Jos ominaisuus on *aktivointi poistetaan* , valitse **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="5015b-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="5015b-117">Saat lisätietoja tutustu seuraavassa [artikkelissa](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="5015b-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

