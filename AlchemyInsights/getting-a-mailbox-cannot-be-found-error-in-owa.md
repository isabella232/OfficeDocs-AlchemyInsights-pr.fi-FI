---
title: 126 Postilaatikon saaminen ei löydy virheestä OWA:ssa?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426659"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="45a2d-102">Saatko postilaatikon, joka ei löydy -virheestä Outlookin verkkosovelluksessa?</span><span class="sxs-lookup"><span data-stu-id="45a2d-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="45a2d-103">Jos käytät Outlookin verkkotiliä ja  saat virheilmoituksen postilaatikosta, tiliä, jolla muodostat yhteyden Outlookin verkkosovellukseen, ei ole Exchange Online -käyttöoikeutta, joten tiliin ei ole liitetty postilaatikkoa.</span><span class="sxs-lookup"><span data-stu-id="45a2d-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="45a2d-104">Järjestelmänvalvoja voi määrittää tilin käyttöoikeuden seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="45a2d-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="45a2d-105">Avaa [Microsoft 365 -hallintakeskus,](https://portal.office.com/adminportal/home#/homepage) siirry  Aktiiviset käyttäjät -osioon ja valitse käyttäjä, joka näkee virheen. </span><span class="sxs-lookup"><span data-stu-id="45a2d-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="45a2d-106">Siirry käyttäjäsivulla Käyttöoikeudet ja  sovellukset -osaan, valitse asianmukainen Sijainti-arvo ja määritä käyttöoikeus, joka sisältää Exchange Onlinen (laajenna käyttöoikeus, jotta näet sen tiedot). </span><span class="sxs-lookup"><span data-stu-id="45a2d-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="45a2d-107">Kun olet valmis, valitse **Tallenna muutokset.**</span><span class="sxs-lookup"><span data-stu-id="45a2d-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="45a2d-108">Joissakin tapauksissa, jos käyttöoikeus on jo määritetty käyttäjätilille, käyttöoikeuden poistaminen ja uudelleennimeäminen auttaa ratkaisemaan ongelman ja valmistella sen oikein järjestelmässä:</span><span class="sxs-lookup"><span data-stu-id="45a2d-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="45a2d-109">Tarkista, ovatko M365 Exchange Online -tilauksesi (ja muut, jos sinulla on) tilaukset ajan tasalla ja eivät ole hiljattain vanhentuneet.</span><span class="sxs-lookup"><span data-stu-id="45a2d-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="45a2d-110">Kun olet varmistanut, että tilauksesi ei ole päättynyt ja että käyttäjätilille on määritetty kelvollinen käyttöoikeus, käyttöoikeuden valmistelu voi kestää jopa 24 tuntia, joten sinun on ehkä odotettava ongelman ratkaisemista.</span><span class="sxs-lookup"><span data-stu-id="45a2d-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="45a2d-111">Lisätietoja on kohdassa [Käyttöoikeuksien määrittäminen ja hallinta.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="45a2d-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>