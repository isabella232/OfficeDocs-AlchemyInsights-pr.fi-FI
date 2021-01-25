---
title: Sovellusten kehittämiseen liittyvät ongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974475"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="18042-102">Sovellusten kehittämiseen liittyvät ongelmat</span><span class="sxs-lookup"><span data-stu-id="18042-102">Issues developing applications</span></span>

<span data-ttu-id="18042-103">Seuraavissa artikkeleissa on tietoja Azure Active Directory (AD) -sovellusten rakentamiseen yleisimpiä ongelmia varten:</span><span class="sxs-lookup"><span data-stu-id="18042-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="18042-104">I am seeing trouble signing in to application(s) using Chrome browser only</span><span class="sxs-lookup"><span data-stu-id="18042-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="18042-105">En tiedä, miten voin muuttaa sovellukseni tunnusten elinkaaren oletusarvoja</span><span class="sxs-lookup"><span data-stu-id="18042-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="18042-106">En tiedä, miten sovelluksen suostumus toimii</span><span class="sxs-lookup"><span data-stu-id="18042-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="18042-107">En tiedä, miten voin myöntää käyttöoikeuksia sovellukseeni</span><span class="sxs-lookup"><span data-stu-id="18042-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="18042-108">En ymmärrä delegoidun ja sovelluksen käyttöoikeuksien välistä eroa</span><span class="sxs-lookup"><span data-stu-id="18042-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="18042-109">\***Azure Active Directory -todennuskirjaston (ADAL) ja Azure AD Graph API:n (AAD Graph) tuen päättyminen** _</span><span class="sxs-lookup"><span data-stu-id="18042-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="18042-110">30. kesäkuuta 2020 alkaen Uusia ominaisuuksia ei enää lisätä Azure Active Directory -todennuskirjastoon (ADAL) ja Azure AD Graph API:een (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="18042-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="18042-111">Teknisen tuen ja suojauspäivitysten tarjoaminen jatkuu, mutta ominaisuuspäivityksiä ei enää tarjota.</span><span class="sxs-lookup"><span data-stu-id="18042-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="18042-112">30. kesäkuuta 2022 alkaen ADAL: n ja AAD Graphin tuki päättyy, eikä se enää tarjoa teknistä tukea tai suojauspäivityksiä.</span><span class="sxs-lookup"><span data-stu-id="18042-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="18042-113">Tämän ehdon vuoksi vaikutukset ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="18042-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="18042-114">Sovellukset, jotka käyttävät ADAL:tä olemassa olevissa käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa teknistä tukea tai suojauspäivityksiä.</span><span class="sxs-lookup"><span data-stu-id="18042-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="18042-115">AAD Graphia tämän jälkeen käyttävät sovellukset eivät ehkä enää saa vastauksia AAD Graph -päätepisteltä</span><span class="sxs-lookup"><span data-stu-id="18042-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="18042-116">_ *ADAL-siirto*\*</span><span class="sxs-lookup"><span data-stu-id="18042-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="18042-117">Jos käytät Microsoft-sovelluksia, suosittelemme päivittämään Microsoftin todennuskirjastoon (MSAL), jossa on uusimmat ominaisuudet ja suojauspäivitykset.</span><span class="sxs-lookup"><span data-stu-id="18042-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="18042-118">Tämä suositus koskee Sitä, että Microsoft aloittaa sovellustensa MSAL-sovelluksiin siirtymisprosessin tuen päättymiseen mennessä.</span><span class="sxs-lookup"><span data-stu-id="18042-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="18042-119">Microsoftin siirtyminen MSAL-sovelluksiin varmistaa, että sovellukset hyötyvät MSAL:n käynnissä olevista suojaus- ja ominaisuusparannuksista.</span><span class="sxs-lookup"><span data-stu-id="18042-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="18042-120">ADAL:n usein kysytyt kysymykset</span><span class="sxs-lookup"><span data-stu-id="18042-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="18042-121">Lisätietoja sovellusten siirtämisestä käyttöympäristökohtaisesti</span><span class="sxs-lookup"><span data-stu-id="18042-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="18042-122">Jos tarvitset apua sen ymmärtämiseen, mitkä sovellukset käyttävät ADAL:tä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit ja ottaa tarvittaessa yhteyttä itsenäisten ohjelmistotoimittajien (ISV) tai sovellustoimittajien kanssa.</span><span class="sxs-lookup"><span data-stu-id="18042-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="18042-123">Microsoft-tuki voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.</span><span class="sxs-lookup"><span data-stu-id="18042-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="18042-124">**AAD Graph -siirto**</span><span class="sxs-lookup"><span data-stu-id="18042-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="18042-125">Jos sovellus käyttää AAD Graphia, noudata ohjeitamme AAD Graph -sovellusten siirtämiseksi Microsoft Graphiin:</span><span class="sxs-lookup"><span data-stu-id="18042-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="18042-126">[Siirron tarkistusluettelomme tarjoaa aloituspisteen.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="18042-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="18042-127">Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia.</span><span class="sxs-lookup"><span data-stu-id="18042-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="18042-128">Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit ja ota tarvittaessa yhteyttä kaikkiin itsenäisten ohjelmistotoimittajien (ISV) tai sovellustoimittajien käyttöön.</span><span class="sxs-lookup"><span data-stu-id="18042-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="18042-129">Microsoft-tuki voi myös antaa tietoja AAD Graphin käytöstä vuokraajassasi.</span><span class="sxs-lookup"><span data-stu-id="18042-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







