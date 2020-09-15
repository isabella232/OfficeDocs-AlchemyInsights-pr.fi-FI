---
title: 2010-hyväksyntä työn kulkua ei voi lisätä
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699732"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="f1b59-102">2010-hyväksyntä työn kulkua ei voi lisätä</span><span class="sxs-lookup"><span data-stu-id="f1b59-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="f1b59-103">Microsoft SharePoint-sivustokokoelmassa et voi lisätä yleisesti käytettävää työn kulkua (kuten "hyväksyntä – SharePoint 2010") luetteloon tai kirjastoon.</span><span class="sxs-lookup"><span data-stu-id="f1b59-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="f1b59-104">Voit korjata ongelman toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="f1b59-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="f1b59-105">Avaa sivustokokoelman pääsivusto SharePoint Designer 2013-sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="f1b59-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="f1b59-106">Valitse **sivuston objektit**-kohdassa **työn kulut**.</span><span class="sxs-lookup"><span data-stu-id="f1b59-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="f1b59-107">Valitse **työn kulut** -valinta nauhan **Uusi** -osasta **uudelleenkäytettävä työn kulku**.</span><span class="sxs-lookup"><span data-stu-id="f1b59-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="f1b59-108">Kirjoita **Luo uudelleenkäytettävä työn kulku** -lomakkeeseen nimi \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="f1b59-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="f1b59-109">Valitse **ympäristö tyyppi**-kohdassa **SharePoint 2010-työn kulku**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="f1b59-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="f1b59-110">Valitse **työn kulun** valinta nauhan **Tallenna** -osassa **Julkaise**.</span><span class="sxs-lookup"><span data-stu-id="f1b59-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="f1b59-111">Valitse **työn kulun** valinta nauhan **hallinta** -osassa **Julkaise globaalisti**.</span><span class="sxs-lookup"><span data-stu-id="f1b59-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="f1b59-112">Valitse näkyviin tulevassa vahvistus valinta ikkunassa **OK**.</span><span class="sxs-lookup"><span data-stu-id="f1b59-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="f1b59-113">Etsi sivustokokoelman pääsivusto selaimessa ja käytä **sivustoasetusten** \> **sivustokokoelman ominaisuuksia**.</span><span class="sxs-lookup"><span data-stu-id="f1b59-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="f1b59-114">**Työn kulut** -ominaisuuden vaihtaminen:</span><span class="sxs-lookup"><span data-stu-id="f1b59-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="f1b59-115">· Jos toiminto on  *aktivoitu*  , valitse **Poista Akti vointi** ja valitse sitten **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="f1b59-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="f1b59-116">· Jos toiminto on  *poistettu käytöstä*  , valitse **Aktivoi**.</span><span class="sxs-lookup"><span data-stu-id="f1b59-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="f1b59-117">Katso lisä tietoja seuraavasta [artikkelista](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="f1b59-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

