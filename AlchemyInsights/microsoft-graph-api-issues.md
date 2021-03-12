---
title: Microsoft Graphin ohjelmointirajapinnan ongelmat
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713702"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="2d3fb-102">Microsoft Graphin ohjelmointirajapinnan ongelmat</span><span class="sxs-lookup"><span data-stu-id="2d3fb-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="2d3fb-103">Tämä ohjeaihe voi koskea myös kehittäjiä, jotka käyttävät edelleen Azure AD Graph -ohjelmointirajapintaa.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="2d3fb-104">On kuitenkin erittäin **suositeltavaa,** että käytät Microsoft Graphia kaikissa hakemisto-, käyttäjätiedot- ja käytönhallintaskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="2d3fb-105">**Todennus- tai valtuutusongelmat**</span><span class="sxs-lookup"><span data-stu-id="2d3fb-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="2d3fb-106">Jos sovellus  ei voi hankkia tunnuksia Microsoft Graph -kutsumista varten, valitse Ongelma, kun saat käyttöoikeustietueen **(todennuksen)** Microsoft Graph -luokan, niin saat tarkempia ohjeita ja tukea tästä aiheesta.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="2d3fb-107">Jos sovellus saa **401-** tai 403-valtuutusvirheitä Microsoft Graphia kutsuttaessa, valitse Hae käyttö estetty **-virhe (Valtuutus)** Microsoft Graph API -luokka, niin saat tarkempia ohjeita ja tukea tästä aiheesta.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="2d3fb-108">**Haluan käyttää Microsoft Graphia, mutta en tiedä, mistä aloittaa**</span><span class="sxs-lookup"><span data-stu-id="2d3fb-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="2d3fb-109">Yleistä Microsoft Graphista</span><span class="sxs-lookup"><span data-stu-id="2d3fb-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="2d3fb-110">Yleistä käyttäjätietojen ja käytön hallinnasta Microsoft Graphissa</span><span class="sxs-lookup"><span data-stu-id="2d3fb-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="2d3fb-111">Microsoft Graph -sovellusten rakentamisen aloittaminen</span><span class="sxs-lookup"><span data-stu-id="2d3fb-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="2d3fb-112">**Microsoft Graph Explorer** – Microsoft Graph -ohjelmointirajapintojen testaaminen vuokraajassa tai esittely vuokraajassa</span><span class="sxs-lookup"><span data-stu-id="2d3fb-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="2d3fb-113">**Haluan käyttää Microsoft Graphia, mutta tukeeko se tarvitsemii v1.0-hakemistorajapintojen käyttöä?**</span><span class="sxs-lookup"><span data-stu-id="2d3fb-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="2d3fb-114">Microsoft Graph on hakemiston, käyttäjätietojen ja käytön hallinnan suositeltu ohjelmointirajapinta.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="2d3fb-115">Azure AD Graphin ja Microsoft Graphin välillä on kuitenkin vielä muutamia aukkoja.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="2d3fb-116">Tutustu seuraaviin artikkeleihin, joissa korostetaan uusimpia eroja, jotka auttavat valitsemaan:</span><span class="sxs-lookup"><span data-stu-id="2d3fb-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="2d3fb-117">Resurssityyppierot Azure AD Graphin ja Microsoft Graphin välillä</span><span class="sxs-lookup"><span data-stu-id="2d3fb-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="2d3fb-118">Azure AD Graphin ja Microsoft Graphin ominaisuuden erot</span><span class="sxs-lookup"><span data-stu-id="2d3fb-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="2d3fb-119">Azure AD:n ja Microsoft Graphin väliset menetelmäerot</span><span class="sxs-lookup"><span data-stu-id="2d3fb-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="2d3fb-120">**Ohjelmointirajapinta, johon soitan, ei toimi – missä voin tehdä enemmän testausta?**</span><span class="sxs-lookup"><span data-stu-id="2d3fb-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="2d3fb-121">**Microsoft Graph Explorer** – Testaa Microsoft Graph -ohjelmointirajapinnat vuokraajassa  tai esittely vuokraajassa ja tutustu myös mallikyselyihin Microsoft Graph Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="2d3fb-122">**Sovellukseni on liian hidas ja sitä myös käytetään kursivassa. Mitä parannuksia voin tehdä?**</span><span class="sxs-lookup"><span data-stu-id="2d3fb-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="2d3fb-123">Skenaariostasi riippuen käytettävissäsi on useita vaihtoehtoja, joilla voit tehdä sovelluksesta entistä tehokkaammin ja joissakin tapauksissa vähemmän altis palvelun utelle (kun puheluita on liikaa).</span><span class="sxs-lookup"><span data-stu-id="2d3fb-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="2d3fb-124">Microsoft Graphin parhaat käytännöt</span><span class="sxs-lookup"><span data-stu-id="2d3fb-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="2d3fb-125">Siirtopyynnöt</span><span class="sxs-lookup"><span data-stu-id="2d3fb-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="2d3fb-126">Muutosten jäljitäminen deltakyselyn avulla</span><span class="sxs-lookup"><span data-stu-id="2d3fb-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="2d3fb-127">Saa ilmoituksia muutoksista verkko-osien kautta</span><span class="sxs-lookup"><span data-stu-id="2d3fb-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="2d3fb-128">Kursimisohjeet</span><span class="sxs-lookup"><span data-stu-id="2d3fb-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="2d3fb-129">**Mistä löydän lisätietoja virheistä ja tunnetuista ongelmista?**</span><span class="sxs-lookup"><span data-stu-id="2d3fb-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="2d3fb-130">Microsoft Graphin virhevastaustiedot</span><span class="sxs-lookup"><span data-stu-id="2d3fb-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="2d3fb-131">Microsoft Graphin tunnetut ongelmat</span><span class="sxs-lookup"><span data-stu-id="2d3fb-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="2d3fb-132">**Mistä voin tarkistaa palvelun käytettävyyden ja yhteyden tilan?**</span><span class="sxs-lookup"><span data-stu-id="2d3fb-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="2d3fb-133">Niiden taustalla olevien palvelujen käytettävyys ja yhteydet, joita voidaan käyttää Microsoft Graphin kautta, voivat vaikuttaa Microsoft Graphin yleiseen käytettävuuteen ja suorituskykyyn.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="2d3fb-134">Tarkista Azure Active Directory -palvelun kuntoa varten Azure-tilasivulla lueteltujen **suojaus-** ja [käyttäjätietopalvelujen tila.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="2d3fb-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="2d3fb-135">Tarkista Microsoft Graphiin osallistuneet Office-palvelut Office Service Health -koontinäytössä lueteltujen [palvelujen tila.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="2d3fb-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="2d3fb-136">Microsoft Graphin valtuutusvirheet voivat johtua useista eri ongelmista, joista useimmat luovat 401- tai 403-virheen.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="2d3fb-137">Esimerkiksi seuraavat voivat johtaa valtuutusvirheisiin:</span><span class="sxs-lookup"><span data-stu-id="2d3fb-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="2d3fb-138">Virheelliset [tunnusoston työnkulut](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="2d3fb-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="2d3fb-139">Huonosti määritetyt [käyttöoikeuksien laajuudet](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="2d3fb-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="2d3fb-140">[puuttuminen](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="2d3fb-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="2d3fb-141">\**_Azure Active Directory -todentamiskirjaston (ADAL) ja Azure AD Graph API:n (AAD Graph) tuen päättyminen_* _</span><span class="sxs-lookup"><span data-stu-id="2d3fb-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="2d3fb-142">_*30. kesäkuuta 2020*\* alkaen uusia ominaisuuksia ei enää lisätä ADAL:een ja Azure AD Graphiin.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="2d3fb-143">Tarjoamme jatkossakin teknistä tukea ja suojauspäivityksiä, mutta emme enää tarjoa ominaisuuspäivityksiä.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="2d3fb-144">**30. kesäkuuta 2022** alkaen microsoft lopettaa ADAL: n ja Azure AD Graphin tuen, eikä se enää tarjoa teknistä tukea tai suojauspäivityksiä.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="2d3fb-145">Sovellukset, jotka käyttävät ADAL:tä nykyisissä käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa *mitään teknistä tukea tai suojauspäivityksiä.*</span><span class="sxs-lookup"><span data-stu-id="2d3fb-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="2d3fb-146">Azure AD Graphia tämän jälkeen käyttävät sovellukset eivät ehkä enää saa vastauksia Azure AD Graph -päätepisteltä.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="2d3fb-147">**ADAL-siirto**</span><span class="sxs-lookup"><span data-stu-id="2d3fb-147">**ADAL Migration**</span></span>

<span data-ttu-id="2d3fb-148">Suosittelemme päivittämistä [Microsoft todentamiskirjastoon (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), jossa on uusimmat ominaisuudet ja suojauspäivitykset.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="2d3fb-149">Jos käytät Microsoft-sovelluksia, tiedät, että Microsoft on parhaillaan muuttamassa sovelluksiaan MSAL-sovelluksiin tuen päättymiseen mennessä, jotta ne hyötyvät MSAL:n käynnissä olevista suojaus- ja ominaisuusparannuksista.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="2d3fb-150">Lue ADAL:ää koskevat usein kysytyt kysymykset</span><span class="sxs-lookup"><span data-stu-id="2d3fb-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="2d3fb-151">Lisätietoja sovellusten siirtämisestä käyttöympäristökohtaisesti</span><span class="sxs-lookup"><span data-stu-id="2d3fb-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="2d3fb-152">Jos tarvitset apua sen ymmärtämiseen, mitkä sovellukset käyttävät ADAL:tä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit ja tarvittaessa ottaa yhteyttä internet-palveluntarjoajiin tai sovellustarjoajiin.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="2d3fb-153">Microsoftin tukipalvelu voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="2d3fb-154">**AAD Graph -siirto**</span><span class="sxs-lookup"><span data-stu-id="2d3fb-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="2d3fb-155">Jos sovellus käyttää Azure AD Graphia, noudata ohjeita azure AD Graph -sovellusten [siirtämiseksi Microsoft Graphiin.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="2d3fb-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="2d3fb-156">[Siirron tarkistusluettelo tarjoaa aloituspisteen](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="2d3fb-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="2d3fb-157">Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="2d3fb-158">Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit. Ota tarvittaessa yhteyttä internet-palveluntarjoajaan tai sovelluksen toimittajaan.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="2d3fb-159">Microsoft-tuki voi myös tarjota sinulle luettelon vuokraajan kaikista AAD Graph -käytöstä.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="2d3fb-160">Jotta sovellus voi käyttää Microsoft Graphin tietoja, käyttäjän tai järjestelmänvalvojan on myönnettävä se oikeat käyttöoikeudet suostumusprosessin kautta.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="2d3fb-161">[Microsoft Graph -käyttöoikeusviittauksessa](https://docs.microsoft.com/graph/permissions-reference) luetellaan kuhunkin Microsoft Graph -ohjelmointirajapintojen pääjoukkoon liittyvät käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="2d3fb-162">Artikkelissa on myös ohjeita käyttöoikeuksien käyttöön.</span><span class="sxs-lookup"><span data-stu-id="2d3fb-162">It also provides guidance about how to use the permissions.</span></span>
