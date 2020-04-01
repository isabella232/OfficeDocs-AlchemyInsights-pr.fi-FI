---
title: BlockLegacyAuth -tunniste
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079257"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="d94de-102">Vanhan todennuksen estäminen</span><span class="sxs-lookup"><span data-stu-id="d94de-102">Blocking legacy authentication</span></span>

<span data-ttu-id="d94de-103">Vanha todennus on termi, joka viittaa todennuspyyntöön, jonka on tehnyt:</span><span class="sxs-lookup"><span data-stu-id="d94de-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="d94de-104">Vanhemmat Office-asiakkaat, jotka eivät käytä nykyaikaista todennusta (esimerkiksi Office 2010 -asiakasohjelma).</span><span class="sxs-lookup"><span data-stu-id="d94de-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="d94de-105">Mikä tahansa asiakas, joka käyttää vanhoja sähköpostiprotokollia, kuten IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="d94de-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="d94de-106">Lisätietoja vanhan todennuksen estämisestä ja nykyaikaisen todennuksen ottamisesta käyttöön on ohjeaiheessa [Vanhan todennuksen estäminen](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="d94de-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="d94de-107">Azure Active Directoryn (Azure AD) suojausoletusarvot helpottavat organisaation suojausta ja auttavat suojaamaan organisaatiotasi.</span><span class="sxs-lookup"><span data-stu-id="d94de-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="d94de-108">Suojauksen oletusarvot sisältävät valmiiksi määritetyt suojausasetukset tavallisille hyökkäyksille.</span><span class="sxs-lookup"><span data-stu-id="d94de-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="d94de-109">Lisätietoja suojauksen oletusarvoista on ohjeaiheessa [Mitä ovat suojausoletukset?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="d94de-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="d94de-110">**Huomautus:** Jos vuokraaja on luotu 22.10.2019 tai sen jälkeen, on mahdollista, että käytössäsi on uusi suojattu oletusarvoisesti -toiminto ja käytössä on jo oletusasetukset vuokraajassasi.</span><span class="sxs-lookup"><span data-stu-id="d94de-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="d94de-111">Jotta kaikki käyttäjät voidaan suojata, tietoturvan oletusarvoja otetaan käyttöön kaikille uusille vuokralaisille.</span><span class="sxs-lookup"><span data-stu-id="d94de-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
