---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685595"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="23d0b-102">Vanhan todennuksen estäminen</span><span class="sxs-lookup"><span data-stu-id="23d0b-102">Blocking legacy authentication</span></span>

<span data-ttu-id="23d0b-103">Vanha todennus on termi, joka viittaa todennus pyyntöön, jonka on tehnyt:</span><span class="sxs-lookup"><span data-stu-id="23d0b-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="23d0b-104">Vanhat Office-Asiakkaat, jotka eivät käytä nykyaikaista todennusta (esimerkiksi Office 2010-asiakas).</span><span class="sxs-lookup"><span data-stu-id="23d0b-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="23d0b-105">Kaikki asiakas ohjelmat, jotka käyttävät vanhoja Sähkö posti protokollia, kuten IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="23d0b-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="23d0b-106">Lisä tietoja vanhan todennuksen estämisestä ja nykyaikaisen todennuksen käyttöönotosta on artikkelissa [vanhan todennuksen estäminen](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="23d0b-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="23d0b-107">Azure Active Directoryn (Azure AD) suojaus oletukset helpottavat suojausta ja auttavat suojaamaan organisaatiota.</span><span class="sxs-lookup"><span data-stu-id="23d0b-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="23d0b-108">Suojausoletukset sisältävät valmiiksi määritetyt turvallisuusasetukset tavallisia hyökkäyksiä varten.</span><span class="sxs-lookup"><span data-stu-id="23d0b-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="23d0b-109">Lisä tietoja tieto turvan oletus arvoista [on artikkelissa Mitä ovat tieto turvan oletukset?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="23d0b-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="23d0b-110">**Huomautus**: Jos vuokraaja on luotu tai sen jälkeen 22 lokakuu, 2019, on mahdollista, että sinulla on uusi suojattu oletus toiminto ja että sinulla on jo suojaus asetukset käytössä vuokra ajassa.</span><span class="sxs-lookup"><span data-stu-id="23d0b-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="23d0b-111">Kaikkien käyttäjien suojaamiseksi on olemassa suojaus oletuksia, jotka on suunniteltu kaikille uusille vuokralaisille.</span><span class="sxs-lookup"><span data-stu-id="23d0b-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
