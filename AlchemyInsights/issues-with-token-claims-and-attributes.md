---
title: Token Claims and Attributes -tunnuksiin liittyvät ongelmat
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035890"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="3b263-102">Token Claims and Attributes -tunnuksiin liittyvät ongelmat</span><span class="sxs-lookup"><span data-stu-id="3b263-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="3b263-103">**Tunnusvaatimusten päivittäminen, määrittäminen tai poistaminen**</span><span class="sxs-lookup"><span data-stu-id="3b263-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="3b263-104">Käyttämällä Azure Active Directorya (Azure [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) AD) voit mukauttaa roolivaatimuksen väitetyyppiä vastaustunnuksessa, jonka saat, kun olet valtuuttanut sovelluksen.</span><span class="sxs-lookup"><span data-stu-id="3b263-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="3b263-105">Sovelluskehittäjät voivat määrittää Azure AD -sovelluksissaan valinnaisten vaateiden avulla, mitä tunnuksia sovellus haluaa käyttää.</span><span class="sxs-lookup"><span data-stu-id="3b263-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="3b263-106">Lisätietoja on kohdassa [Sovelluksesi valinnaisten vaateiden tarjoaminen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="3b263-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="3b263-107">[Määritä ryhmävaatimukset sovelluksille Azure Active Directoryn avulla.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="3b263-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="3b263-108">Jos käytät saumatonta kertakirjaamista sovelluksessasi, tutustu saml-tunnuksessa yrityssovellusten [SAML-tunnusten](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)myöntäjän vaatimusten mukauttamiseen.</span><span class="sxs-lookup"><span data-stu-id="3b263-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="3b263-109">**Claims Attribute Mapping**</span><span class="sxs-lookup"><span data-stu-id="3b263-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="3b263-110">Lisätietoja väiteiden yhdistämiskäytännön määrittämisestä PowerShellin avulla on kohdassa Mukauta vuokraajan tietyn sovelluksen tunnuksiin jätettyjä vaateita [(esikatselu).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="3b263-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="3b263-111">Hakemistorakenteen laajennusmääritteiden avulla voit tallentaa Azure Active Directoryyn lisätietoja käyttäjäobjekteihin ja muihin hakemisto-objekteihin, kuten ryhmiin, vuokraajatietoihin ja palvelun pääobjekteihin.</span><span class="sxs-lookup"><span data-stu-id="3b263-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="3b263-112">Vain käyttäjäobjektien laajennusmääritteitä voidaan käyttää sovellusten vaateiden hakemiseksi.</span><span class="sxs-lookup"><span data-stu-id="3b263-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="3b263-113">[Hakemistorakenteen laajennusmääritteiden](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) käyttäminen vaateissa kuvaa, miten käyttäjätiedot lähetetään sovelluksiin tunnuksen väiteissä hakemistorakenteen laajennusten määritteiden avulla.</span><span class="sxs-lookup"><span data-stu-id="3b263-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="3b263-114">Lisätietoja tunnuksen vaateista on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="3b263-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="3b263-115">Käyttöoikeustietueita koskevat vaateet</span><span class="sxs-lookup"><span data-stu-id="3b263-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="3b263-116">Vaateet id_token</span><span class="sxs-lookup"><span data-stu-id="3b263-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="3b263-117">[Väite,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) että käyttäjä voi odottaa Azure AD B2C:n myöntämia tunnustunnuksia ja käyttöoikeustunnuksia</span><span class="sxs-lookup"><span data-stu-id="3b263-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="3b263-118">SAML-tunnuksen väiteviittaus</span><span class="sxs-lookup"><span data-stu-id="3b263-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
