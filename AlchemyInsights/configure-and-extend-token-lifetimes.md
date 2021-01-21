---
title: Tunnusten elinkaaren määrittäminen ja pidentäminen
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
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916825"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="43df7-102">Tunnusten elinkaaren määrittäminen ja pidentäminen</span><span class="sxs-lookup"><span data-stu-id="43df7-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="43df7-103">Voit määrittää Microsoftin tunnistetietoympäristön myöntämien käytön, SAML-tunnusten tai tunnustietueiden elinkaaren.</span><span class="sxs-lookup"><span data-stu-id="43df7-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="43df7-104">Voit määrittää tunnuksen elinkaaren kaikille organisaation sovelluksille, usean vuokraajan (usean organisaation) sovellukselle tai tietylle organisaation palvelun päätasolle.</span><span class="sxs-lookup"><span data-stu-id="43df7-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="43df7-105">Lisätietoja on lukukelpoisissa [tunnusten käyttöiän määrittämisessä.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="43df7-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="43df7-106">Esimerkkejä tunnusten elinkaaren määrittämisestä on [esimerkeissä.](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="43df7-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="43df7-107">Lisätietoja tunnuksen elinkaaren ja yhteensopivuuden määrittämisestä Azure Active Directory B2C:ssä (Azure AD B2C) on kohdassa Tunnusten määrittäminen [Azure Active Directory B2C:ssä.](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)</span><span class="sxs-lookup"><span data-stu-id="43df7-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="43df7-108">Artikkelissa Määritä istunnon toiminta [Azure Active Directory B2C:ssä](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) kuvataan Azure AD B2C:ssä käytettävät kertakirjautumismenetelmät ja sen avulla voit valita sopivimman kertakirjautumismenetelmän käytäntöä määritettäessä.</span><span class="sxs-lookup"><span data-stu-id="43df7-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="43df7-109">**Kuinka kauan tunnukset kestävät? Kuinka kauan ne ovat voimassa?**</span><span class="sxs-lookup"><span data-stu-id="43df7-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="43df7-110">Tunnusten käyttöajat ovat 1 tunti ja istunnon elinaika on 24 tuntia.</span><span class="sxs-lookup"><span data-stu-id="43df7-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="43df7-111">Tämä tarkoittaa, että jos pyyntöjä ei ole tehty 24 tunnin kuluessa, sinun on kirjauduttava uudelleen sisään ennen uuden tunnuksen pyytämista.</span><span class="sxs-lookup"><span data-stu-id="43df7-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="43df7-112">30. toukokuuta 2020 jälkeen kukaan uusi vuokraaja ei voi käyttää Määritettävissä olevan tunnusten elinkaari -käytäntöä istuntojen ja päivitystunnusten määrittämiseen.</span><span class="sxs-lookup"><span data-stu-id="43df7-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="43df7-113">Poisto tapahtuu useiden kuukausien kuluessa, mikä tarkoittaa, että lopetamme nykyisen istunnon ja päivitämme tunnusten tunnukset.</span><span class="sxs-lookup"><span data-stu-id="43df7-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="43df7-114">Voit edelleen määrittää käyttöoikeustietueen elinkaaren poiston jälkeen.</span><span class="sxs-lookup"><span data-stu-id="43df7-114">You can still configure access token lifetimes after the deprecation.</span></span>






