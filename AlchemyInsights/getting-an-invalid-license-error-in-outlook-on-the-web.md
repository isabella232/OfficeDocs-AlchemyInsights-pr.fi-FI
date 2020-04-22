---
title: 125 Virheellinen käyttöoikeusvirhe Outlookin verkkoversiossa?
ms.author: daeite
author: daeite
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "125"
- "1600021"
ms.assetid: 6d9947d9-6c92-4ada-b655-8ab2a0c2b66d
ms.openlocfilehash: 9324726709423aeb290fcc1866ade5517f71c1ef
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43708828"
---
# <a name="getting-an-invalid-license-error-in-outlook-on-the-web"></a><span data-ttu-id="14675-102">Saatko virheellisen käyttöoikeusvirheen Outlookin verkkoversiossa?</span><span class="sxs-lookup"><span data-stu-id="14675-102">Getting an invalid license error in Outlook on the web?</span></span>

<span data-ttu-id="14675-103">Jos käytät Outlookin verkkoa ja näyttöön tulee **jokin virhe,** joka sisältää **X-OWA-Virhe: Microsoft.Exchange.Data.Storage.InvalidLicenseException,** Exchange Online -käyttöoikeutta ei ole määritetty oikein tai se on äskettäin vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="14675-103">If you're using Outlook on the web and you get a **Something went wrong** error that contains **X-OWA-Error: Microsoft.Exchange.Data.Storage.InvalidLicenseException**, your Exchange Online license isn't correctly assigned or has recently expired.</span></span> <span data-ttu-id="14675-104">Järjestelmänvalvoja voi määrittää käyttöoikeuden sinulle seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="14675-104">Your admin can assign a license to you by following these steps:</span></span>
  
1. <span data-ttu-id="14675-105">Avaa [Microsoft 365 -hallintakeskus](https://portal.office.com/adminportal/home#/homepage) ja valitse **Aktiiviset käyttäjät**-kohdasta **Muokkaa käyttäjää**.</span><span class="sxs-lookup"><span data-stu-id="14675-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and under **Active users**, select **Edit a user**.</span></span>

2. <span data-ttu-id="14675-106">Valitse käyttäjä **Avautuvasta Muokkaa käyttäjää -sivulla.**</span><span class="sxs-lookup"><span data-stu-id="14675-106">In the **Edit a user** page that opens, select the user.</span></span> <span data-ttu-id="14675-107">Valitse avautuvasta käyttäjän ominaisuudet -sivulta **Muokkaa** **tuotteen käyttöoikeuksia**varten .</span><span class="sxs-lookup"><span data-stu-id="14675-107">In the user properties page that opens, click **Edit** for **Product licenses**.</span></span>

3. <span data-ttu-id="14675-108">Valitse avautuvan **Tuotteen käyttöoikeudet -sivulla** sopiva **Sijainti-arvo** ja määritä Exchange Onlinen sisältävä käyttöoikeus (laajenna käyttöoikeus nähdäksesi sen tiedot).</span><span class="sxs-lookup"><span data-stu-id="14675-108">In the **Product licenses** page that opens, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="14675-109">Kun olet valmis, valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="14675-109">When you're finished, click **Save**.</span></span>
