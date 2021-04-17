---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820175"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="b2319-102">Vanhan todennuksen estäminen</span><span class="sxs-lookup"><span data-stu-id="b2319-102">Blocking legacy authentication</span></span>

<span data-ttu-id="b2319-103">Vanha todennus on termi, joka viittaa käyttäjän pyyntöön todentamiseen:</span><span class="sxs-lookup"><span data-stu-id="b2319-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="b2319-104">Vanhemmat Office-asiakasohjelmat, jotka eivät käytä modernia todentamista (esimerkiksi Office 2010 -asiakas).</span><span class="sxs-lookup"><span data-stu-id="b2319-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="b2319-105">Mikä tahansa asiakas, joka käyttää vanhoja sähköpostiprotokollia, kuten IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="b2319-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="b2319-106">Lisätietoja vanhan todennuksen estämisestä ja modernin varmennukseen ottamalla käyttöön saat kohdasta [Vanhan todennuksen estäminen.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="b2319-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="b2319-107">Azure Active Directoryn (Azure AD) suojauksen oletusasetukset helpottavat organisaation suojaamista ja suojaamista.</span><span class="sxs-lookup"><span data-stu-id="b2319-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="b2319-108">Suojaus-oletusasetukset sisältävät valmiiksi määritettyjä suojausasetuksia yleisille hyökkäyksille.</span><span class="sxs-lookup"><span data-stu-id="b2319-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="b2319-109">Lisätietoja suojauksen oletusasetuksista on kohdassa Mitä [ovat suojauksen oletusasetukset?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="b2319-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="b2319-110">**Huomautus:** Jos vuokraaja on luotu 22. lokakuuta 2019 tai sen jälkeen, on mahdollista, että käytät uutta suojattua oletusasetusta ja olet jo ottanut suojauksen oletusasetukset käyttöön vuokraajassasi.</span><span class="sxs-lookup"><span data-stu-id="b2319-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="b2319-111">Kaikkien käyttäjien suojaamiseksi suojauksen oletusasetukset ovat käytössä kaikille uusille vuokralaisille.</span><span class="sxs-lookup"><span data-stu-id="b2319-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
