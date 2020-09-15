---
title: Puuttuva työn kulku ei onnistunut Akti voimaan
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667083"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="9de6f-102">Puuttuva työn kulku ei onnistunut Akti voimaan</span><span class="sxs-lookup"><span data-stu-id="9de6f-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="9de6f-103">Microsoft SharePoint-sivustokokoelmassa et voi lisätä yleisesti käytettävää työn kulkua (kuten "hyväksyntä – SharePoint 2010") luetteloon tai kirjastoon.</span><span class="sxs-lookup"><span data-stu-id="9de6f-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="9de6f-104">Voit korjata ongelman toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="9de6f-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="9de6f-105">Avaa sivustokokoelman pääsivusto SharePoint Designer 2013-sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="9de6f-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="9de6f-106">Valitse **sivuston objektit**-kohdassa **työn kulut**.</span><span class="sxs-lookup"><span data-stu-id="9de6f-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="9de6f-107">Valitse **työn kulut** -valinta nauhan **Uusi** -osasta **uudelleenkäytettävä työn kulku**.</span><span class="sxs-lookup"><span data-stu-id="9de6f-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="9de6f-108">Kirjoita **Luo uudelleenkäytettävä työn kulku** -lomakkeeseen nimi \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="9de6f-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="9de6f-109">Valitse **ympäristö tyyppi**-kohdassa **SharePoint 2010-työn kulku**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="9de6f-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="9de6f-110">Valitse **työn kulun** valinta nauhan **Tallenna** -osassa **Julkaise**.</span><span class="sxs-lookup"><span data-stu-id="9de6f-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="9de6f-111">Valitse **työn kulun** valinta nauhan **hallinta** -osassa **Julkaise globaalisti**.</span><span class="sxs-lookup"><span data-stu-id="9de6f-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="9de6f-112">Valitse näkyviin tulevassa vahvistus valinta ikkunassa **OK**.</span><span class="sxs-lookup"><span data-stu-id="9de6f-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="9de6f-113">Etsi sivustokokoelman pääsivusto selaimessa ja käytä **sivustoasetusten** \> **sivustokokoelman ominaisuuksia**.</span><span class="sxs-lookup"><span data-stu-id="9de6f-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="9de6f-114">Vaihda sitten **työn kulut** -ominaisuus:</span><span class="sxs-lookup"><span data-stu-id="9de6f-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="9de6f-115">· Jos toiminto on  *aktivoitu*  , valitse **Poista Akti vointi** ja valitse sitten **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="9de6f-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="9de6f-116">· Jos toiminto on  *poistettu käytöstä*  , valitse **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="9de6f-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="9de6f-117">Katso lisä tietoja seuraavasta [artikkelista](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="9de6f-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

