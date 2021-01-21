---
title: Käyttöoikeustietueiden saamista koskevat ongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7776"
- "9004351"
ms.openlocfilehash: e2d15603835d3fb43df1b6b5dadec64af00290ff
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916837"
---
# <a name="issues-with-getting-access-tokens"></a><span data-ttu-id="6d8ce-102">Käyttöoikeustietueiden saamista koskevat ongelmat</span><span class="sxs-lookup"><span data-stu-id="6d8ce-102">Issues with getting access tokens</span></span>

<span data-ttu-id="6d8ce-103">Tässä artikkelissa käsitellään resurssin käyttöoikeustietueiden hankinnan epäonnistumisesta.</span><span class="sxs-lookup"><span data-stu-id="6d8ce-103">This topic deals with failures to acquire access tokens to access a resource.</span></span>

<span data-ttu-id="6d8ce-104">**Minulla on ongelmia käytön aloittaminen**</span><span class="sxs-lookup"><span data-stu-id="6d8ce-104">**I'm having trouble getting started**</span></span>

<span data-ttu-id="6d8ce-105">Seuraavissa artikkeleissa on tietoja aloitusongelmien vianmäärityksestä:</span><span class="sxs-lookup"><span data-stu-id="6d8ce-105">To troubleshoot issues you encounter when trying to get started, see the following articles:</span></span>

- [<span data-ttu-id="6d8ce-106">En löydä koodimallia, jotta pääset alkuun</span><span class="sxs-lookup"><span data-stu-id="6d8ce-106">I can't find a code sample to get started</span></span>](https://docs.microsoft.com/azure/active-directory/develop/sample-v2-code) 
- [<span data-ttu-id="6d8ce-107">Tarvitsen apua tunnuksen saaminen .NET:ssä</span><span class="sxs-lookup"><span data-stu-id="6d8ce-107">I need help getting a token in .NET</span></span>](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios)

<span data-ttu-id="6d8ce-108">**En tiedä, miten voin pyytää ja käyttää tunnuksia**</span><span class="sxs-lookup"><span data-stu-id="6d8ce-108">**I don't know how to request and use tokens**</span></span>

<span data-ttu-id="6d8ce-109">Ohjeita tunnusten pyytäminen ja käyttö on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="6d8ce-109">For guidance on how to request and use tokens, see the following articles:</span></span>

- [<span data-ttu-id="6d8ce-110">En tiedä, miten voin pyytää valtuutuskoodia</span><span class="sxs-lookup"><span data-stu-id="6d8ce-110">I don’t know how to request an authorization code</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#request-an-authorization-code) 
- [<span data-ttu-id="6d8ce-111">En tiedä, miten käyttöoikeustietueen pyytäminen voidaan pyytää</span><span class="sxs-lookup"><span data-stu-id="6d8ce-111">I don’t know how to request an access token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-authorization-code-to-request-an-access-token) 
- [<span data-ttu-id="6d8ce-112">En tiedä, miten resurssin käyttöoikeustietueen avulla voi käyttää</span><span class="sxs-lookup"><span data-stu-id="6d8ce-112">I don’t know how to use an access token to access a resource</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-access-token-to-access-the-resource) 
- [<span data-ttu-id="6d8ce-113">En tiedä, miten käyttöoikeustietueen voi päivittää</span><span class="sxs-lookup"><span data-stu-id="6d8ce-113">I don’t know how to refresh an access token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refreshing-the-access-tokens)

<span data-ttu-id="6d8ce-114">**Sain virheilmoituksen pyytäessäni tunnusta**</span><span class="sxs-lookup"><span data-stu-id="6d8ce-114">**I got an error while requesting a token**</span></span>

<span data-ttu-id="6d8ce-115">Seuraavissa artikkeleissa on tietoja tunnuksen pyytämisen aikana kohtaamistasi virheistä:</span><span class="sxs-lookup"><span data-stu-id="6d8ce-115">To troubleshoot errors you have encountered while requesting for a token, see the following articles:</span></span>

- [<span data-ttu-id="6d8ce-116">Sain palveluvirheen tunnuksen pyytämisen jälkeen</span><span class="sxs-lookup"><span data-stu-id="6d8ce-116">I received a service error when requesting a token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- [<span data-ttu-id="6d8ce-117">Saan uuden virheen aiemmin toimivaan sovellukseen</span><span class="sxs-lookup"><span data-stu-id="6d8ce-117">I'm getting a new error to a previously working app</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-breaking-changes)

<span data-ttu-id="6d8ce-118">**Mistä saan lisätietoja AADSTS-virhekoodeista?**</span><span class="sxs-lookup"><span data-stu-id="6d8ce-118">**How do I get more information about AADSTS error codes?**</span></span>

<span data-ttu-id="6d8ce-119">Lisätietoja on kohdassa Todennus- [ja valtuutusvirhekoodit.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)</span><span class="sxs-lookup"><span data-stu-id="6d8ce-119">For more information, see [Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes).</span></span>





