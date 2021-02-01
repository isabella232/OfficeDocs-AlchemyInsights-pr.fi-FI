---
title: Todentamiskirjastoihin liittyvät ongelmat
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063606"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="12ae6-102">Todentamiskirjastoihin liittyvät ongelmat</span><span class="sxs-lookup"><span data-stu-id="12ae6-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="12ae6-103">[Microsoftin käyttäjätietoympäristön todennuskirjastoissa](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) on luettelo Microsoftin tukemista ja yhteensopivista asiakas- ja middleware-kirjastoista.</span><span class="sxs-lookup"><span data-stu-id="12ae6-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="12ae6-104">Microsoftin todentamiskirjasto (MSAL) tukee useita [todennusvirtoja](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) käytettäväksi eri sovellusskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="12ae6-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="12ae6-105">Jos haluat todentaa ja hankkia tunnuksia, alusta uusi julkinen tai luottamuksellinen asiakassovellus koodissasi.</span><span class="sxs-lookup"><span data-stu-id="12ae6-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="12ae6-106">Voit määrittää useita määritysasetuksia, kun alustat asiakassovelluksen Microsoftin todennuskirjastossa (MSAL).</span><span class="sxs-lookup"><span data-stu-id="12ae6-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="12ae6-107">Lisätietoja on kohdassa Sovelluksen [määritysasetukset.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="12ae6-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="12ae6-108">**Azure Active Directory -todennuskirjaston (ADAL) ja Azure AD Graph API:n (AAD Graph) tuen päättyminen**</span><span class="sxs-lookup"><span data-stu-id="12ae6-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="12ae6-109">**30. kesäkuuta 2020** alkaen uusia ominaisuuksia ei enää lisätä ADAL:een ja Azure AD Graphiin.</span><span class="sxs-lookup"><span data-stu-id="12ae6-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="12ae6-110">Tarjoamme jatkossakin teknistä tukea ja suojauspäivityksiä, mutta emme enää tarjoa ominaisuuspäivityksiä.</span><span class="sxs-lookup"><span data-stu-id="12ae6-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="12ae6-111">**30. kesäkuuta 2022** alkaen microsoft lopettaa ADAL: n ja Azure AD Graphin tuen, eikä se enää tarjoa teknistä tukea tai suojauspäivityksiä.</span><span class="sxs-lookup"><span data-stu-id="12ae6-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="12ae6-112">Sovellukset, jotka käyttävät ADAL:tä nykyisissä käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa *teknistä tukea tai suojauspäivityksiä.*</span><span class="sxs-lookup"><span data-stu-id="12ae6-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="12ae6-113">Azure AD Graphia tämän jälkeen käyttävät sovellukset eivät ehkä enää saa vastauksia Azure AD Graph -päätepisteltä.</span><span class="sxs-lookup"><span data-stu-id="12ae6-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="12ae6-114">**ADAL-siirto**</span><span class="sxs-lookup"><span data-stu-id="12ae6-114">**ADAL Migration**</span></span>

<span data-ttu-id="12ae6-115">Suosittelemme päivittämistä [Microsoft todentamiskirjastoon (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), jossa on uusimmat ominaisuudet ja suojauspäivitykset.</span><span class="sxs-lookup"><span data-stu-id="12ae6-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="12ae6-116">Jos käytät Microsoft-sovelluksia, tiedät, että Microsoft on parhaillaan muuttamassa sovelluksiaan MSAL-sovelluksiin tuen päättymiseen mennessä, jotta ne hyötyvät MSAL:n käynnissä olevista suojaus- ja ominaisuusparannuksista.</span><span class="sxs-lookup"><span data-stu-id="12ae6-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="12ae6-117">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="12ae6-117">For more information, see:</span></span>

1. [<span data-ttu-id="12ae6-118">Lue ADAL:ää koskevat usein kysytyt kysymykset</span><span class="sxs-lookup"><span data-stu-id="12ae6-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="12ae6-119">Lisätietoja sovellusten siirtämisestä käyttöympäristökohtaisesti</span><span class="sxs-lookup"><span data-stu-id="12ae6-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="12ae6-120">Jos tarvitset apua sen ymmärtämiseen, mitkä sovellukset käyttävät ADAL:tä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit ja tarvittaessa ottaa yhteyttä internet-palveluntarjoajiin tai sovellustarjoajiin.</span><span class="sxs-lookup"><span data-stu-id="12ae6-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="12ae6-121">Microsoftin tukipalvelu voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.</span><span class="sxs-lookup"><span data-stu-id="12ae6-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="12ae6-122">**AAD Graph -siirto**</span><span class="sxs-lookup"><span data-stu-id="12ae6-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="12ae6-123">Jos sovellus käyttää Azure AD Graphia, noudata ohjeita azure AD Graph -sovellusten [siirtämiseksi Microsoft Graphiin.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="12ae6-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="12ae6-124">Siirron tarkistusluettelomme tarjoaa aloituspisteen.</span><span class="sxs-lookup"><span data-stu-id="12ae6-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="12ae6-125">Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia.</span><span class="sxs-lookup"><span data-stu-id="12ae6-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="12ae6-126">Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit. Ota tarvittaessa yhteyttä internet-palveluntarjoajaan tai sovelluksen toimittajaan.</span><span class="sxs-lookup"><span data-stu-id="12ae6-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="12ae6-127">Microsoft-tuki voi myös tarjota sinulle luettelon vuokraajan kaikista AAD Graph -käytöstä.</span><span class="sxs-lookup"><span data-stu-id="12ae6-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="12ae6-128">Jotta sovellus voi käyttää Microsoft Graphin tietoja, käyttäjän tai järjestelmänvalvojan on myönnettävä se oikeat käyttöoikeudet suostumusprosessin kautta.</span><span class="sxs-lookup"><span data-stu-id="12ae6-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="12ae6-129">[Microsoft Graph -käyttöoikeusviittauksessa](https://docs.microsoft.com/graph/permissions-reference) luetellaan kuhunkin Microsoft Graph -ohjelmointirajapintojen pääjoukkoon liittyvät käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="12ae6-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="12ae6-130">Artikkelissa on myös ohjeita käyttöoikeuksien käyttöön.</span><span class="sxs-lookup"><span data-stu-id="12ae6-130">It also provides guidance about how to use the permissions.</span></span>
