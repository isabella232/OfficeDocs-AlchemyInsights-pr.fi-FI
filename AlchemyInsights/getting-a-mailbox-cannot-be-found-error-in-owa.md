---
title: 126 Postilaatikon hakeminen ei ole virhe OWA:ssa?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: e061ad6b74b27e3f0d597586cb2c8e31b8fa5d23
ms.sourcegitcommit: 83c644c35c2700dc515f091c8f41f9c283b89967
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2020
ms.locfileid: "43105236"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="b863a-102">Saatko postilaatikon, joka ei ole löytynyt -virheestä Outlookin verkkoversiossa?</span><span class="sxs-lookup"><span data-stu-id="b863a-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="b863a-103">Jos käytät Outlookin verkkoyhteyttä ja **postilaatikkoa ei löytynyt virheeksi,** tilillä, jolla muodostat yhteyden Outlookin verkkoversioon, ei ole Exchange Online -käyttöoikeutta, joten tiliin ei ole liitetty postilaatikkoa.</span><span class="sxs-lookup"><span data-stu-id="b863a-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="b863a-104">Järjestelmänvalvoja voi määrittää tiliisi käyttöoikeuden seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="b863a-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="b863a-105">Avaa [Microsoft 365 -hallintakeskus](https://portal.office.com/adminportal/home#/homepage) ja siirry **Käyttäjät-osan** **Aktiiviset käyttäjät** -kohtaan ja valitse käyttäjä, joka näkee virheen.</span><span class="sxs-lookup"><span data-stu-id="b863a-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="b863a-106">Siirry avautuvan käyttäjäsivun Käyttöoikeudet **ja sovellukset -osaan,** valitse asianmukainen **Sijainti-arvo** ja määritä Käyttöoikeus, joka sisältää Exchange Onlinen (laajenna käyttöoikeus nähdäksesi sen tiedot).</span><span class="sxs-lookup"><span data-stu-id="b863a-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="b863a-107">Kun olet valmis, valitse **Tallenna muutokset**.</span><span class="sxs-lookup"><span data-stu-id="b863a-107">When you're finished, click **Save changes**.</span></span>
