---
title: Virhe koodi 550 5.7.501 käyttö estetty, roska postin väärinkäyttö havaittu
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 6542450ca4d03daef4a7f63783d431d2091bc5e7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784052"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="cb826-102">550 5.7.501 käyttö estetty, roska postin väärinkäyttö havaittu</span><span class="sxs-lookup"><span data-stu-id="cb826-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="cb826-103">Tämä sanoma tulee yleensä näkyviin, kun käyttäjät lähettävät Sähkö posti viestejä IP-osoitteista käyttäen alkuperäistä *. onmicrosoft.com* -toimi aluetta, joka on määritetty uusille vuokralaisille Microsoft 365-palvelussa.</span><span class="sxs-lookup"><span data-stu-id="cb826-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Microsoft 365.</span></span> <span data-ttu-id="cb826-104">Helpoin ratkaisu ongelmaan on:</span><span class="sxs-lookup"><span data-stu-id="cb826-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="cb826-105">[Lisää toimi alue vuokra](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain)ajalle.</span><span class="sxs-lookup"><span data-stu-id="cb826-105">[Add a domain to your tenant](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="cb826-106">[Vaihda käyttäjien ensisijaisena Sähkö posti osoitteena](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) juuri lisäämääsi uutta mukautettua toimi aluetta.</span><span class="sxs-lookup"><span data-stu-id="cb826-106">[Change your users' primary email address](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
