---
title: 126, että posti laatikkoa ei löydy-virhe OWA-sovelluksessa?
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
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706747"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="0459d-102">Etkö löytänyt Sähkö posti laatikkoa virheestä Outlookin verkko versiossa?</span><span class="sxs-lookup"><span data-stu-id="0459d-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="0459d-103">Jos käytät Outlookia verkossa ja saat **Posti laatikkoa ei löydy** virheestä, tilillä, jolla muodostat yhteyden Outlookin verkko versioon, ei ole Exchange Online-käyttö oikeutta, joten tiliin ei ole liitetty posti laatikkoa.</span><span class="sxs-lookup"><span data-stu-id="0459d-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="0459d-104">Järjestelmänvalvojasi voi määrittää tilillesi käyttö oikeuden noudattamalla seuraavia ohjeita:</span><span class="sxs-lookup"><span data-stu-id="0459d-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="0459d-105">Avaa [Microsoft 365-hallinta keskus](https://portal.office.com/adminportal/home#/homepage) ja siirry **käyttäjät** -osion **aktiiviset käyttäjät** -osioon ja valitse käyttäjä, joka näkee virheen.</span><span class="sxs-lookup"><span data-stu-id="0459d-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="0459d-106">Siirry avautuvassa käyttäjä sivulla käyttö oikeudet **ja sovellukset** -osioon, valitse sopiva **Sijainti** -arvo ja määritä käyttö oikeus, joka sisältää Exchange Onlinen (Laajenna käyttö oikeus, jotta näet sen tiedot).</span><span class="sxs-lookup"><span data-stu-id="0459d-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="0459d-107">Kun olet valmis, valitse **Tallenna muutokset**.</span><span class="sxs-lookup"><span data-stu-id="0459d-107">When you're finished, click **Save changes**.</span></span>
