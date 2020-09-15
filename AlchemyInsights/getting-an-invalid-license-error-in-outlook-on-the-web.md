---
title: 125 virhe haettaessa virheellistä käyttö oikeus virhettä Outlookin verkko versiossa?
ms.author: daeite
author: daeite
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "125"
- "1600021"
ms.assetid: 6d9947d9-6c92-4ada-b655-8ab2a0c2b66d
ms.openlocfilehash: 825d91cd81646767b100e6fc964d7a94b8bc6879
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677456"
---
# <a name="getting-an-invalid-license-error-in-outlook-on-the-web"></a><span data-ttu-id="3c025-102">Saatko virheellisen käyttö oikeus virheen Outlookin verkko versiossa?</span><span class="sxs-lookup"><span data-stu-id="3c025-102">Getting an invalid license error in Outlook on the web?</span></span>

<span data-ttu-id="3c025-103">Jos käytät Outlookia verkossa ja **saat jonkin virhe ilmoituksen,** joka sisältää **X-OWA-virhe: Microsoft. Exchange. data. Storage. InvalidLicenseException**, Exchange Online-käyttö oikeutta ei ole määritetty oikein tai se on äskettäin vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="3c025-103">If you're using Outlook on the web and you get a **Something went wrong** error that contains **X-OWA-Error: Microsoft.Exchange.Data.Storage.InvalidLicenseException**, your Exchange Online license isn't correctly assigned or has recently expired.</span></span> <span data-ttu-id="3c025-104">Järjestelmänvalvojasi voi määrittää sinulle käyttö oikeuden noudattamalla seuraavia ohjeita:</span><span class="sxs-lookup"><span data-stu-id="3c025-104">Your admin can assign a license to you by following these steps:</span></span>
  
1. <span data-ttu-id="3c025-105">Avaa [Microsoft 365-hallinta keskus](https://portal.office.com/adminportal/home#/homepage) ja valitse **aktiiviset käyttäjät**-kohdassa **Muokkaa käyttäjää**.</span><span class="sxs-lookup"><span data-stu-id="3c025-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and under **Active users**, select **Edit a user**.</span></span>

2. <span data-ttu-id="3c025-106">Valitse näkyviin tulevassa **Muokkaa käyttäjää** -sivulla käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="3c025-106">In the **Edit a user** page that opens, select the user.</span></span> <span data-ttu-id="3c025-107">Valitse avautuvan käyttäjän ominaisuudet-sivulla **Muokkaa** **tuotteen käyttö oikeuksia**varten.</span><span class="sxs-lookup"><span data-stu-id="3c025-107">In the user properties page that opens, click **Edit** for **Product licenses**.</span></span>

3. <span data-ttu-id="3c025-108">Valitse avautuvassa **tuotteen käyttö oikeudet** -sivulla sopiva **Sijainti** -arvo ja määritä käyttö oikeus, joka sisältää Exchange Onlinen (Laajenna käyttö oikeutta, jotta näet sen tiedot).</span><span class="sxs-lookup"><span data-stu-id="3c025-108">In the **Product licenses** page that opens, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="3c025-109">Kun olet valmis, valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="3c025-109">When you're finished, click **Save**.</span></span>
