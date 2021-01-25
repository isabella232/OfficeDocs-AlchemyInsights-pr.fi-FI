---
title: Microsoft Graph -ohjelmointirajapinnan kysely
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974418"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="ea2f7-102">Microsoft Graph -ohjelmointirajapinnan kysely</span><span class="sxs-lookup"><span data-stu-id="ea2f7-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="ea2f7-103">Tämä ohjeaihe voi koskea myös kehittäjiä, jotka käyttävät edelleen Azure AD Graph -ohjelmointirajapintaa.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="ea2f7-104">On kuitenkin erittäin **suositeltavaa, että** käytät Microsoft Graphia kaikissa hakemisto-, käyttäjätiedot- ja käytönhallintaskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="ea2f7-105">**Todennus- tai valtuutusongelmat**</span><span class="sxs-lookup"><span data-stu-id="ea2f7-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="ea2f7-106">Jos sovellus  ei voi hankkia tunnuksia Microsoft Graph -kutsumista varten, valitse Ongelma, kun saat käyttöoikeustietueen **(todennuksen)** Microsoft Graph -luokan, niin saat tarkempia ohjeita ja tukea tästä aiheesta.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="ea2f7-107">Jos sovellus saa **401-** tai 403-valtuutusvirheitä Microsoft Graphia kutsuttaessa, valitse Hae käyttö estetty **-virhe (Valtuutus)** Microsoft Graph API -luokka, niin saat tarkempia ohjeita ja tukea tästä aiheesta.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="ea2f7-108">**Haluan käyttää Microsoft Graphia, mutta en tiedä, mistä aloittaa**</span><span class="sxs-lookup"><span data-stu-id="ea2f7-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="ea2f7-109">Lisätietoja Microsoft Graphista on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="ea2f7-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="ea2f7-110">Yleistä Microsoft Graphista</span><span class="sxs-lookup"><span data-stu-id="ea2f7-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="ea2f7-111">Yleistä Käyttäjätietojen ja käytön hallinnasta Microsoft Graphissa</span><span class="sxs-lookup"><span data-stu-id="ea2f7-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="ea2f7-112">Microsoft Graph -sovellusten rakentamisen aloittaminen</span><span class="sxs-lookup"><span data-stu-id="ea2f7-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="ea2f7-113">**Microsoft Graph Explorer** – Microsoft Graph -ohjelmointirajapintojen testaaminen vuokraajassa tai esittely vuokraajassa</span><span class="sxs-lookup"><span data-stu-id="ea2f7-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="ea2f7-114">**Haluan käyttää Microsoft Graphia, mutta tukeeko se tarvitsen v1.0-hakemiston ohjelmointirajapinnat?**</span><span class="sxs-lookup"><span data-stu-id="ea2f7-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="ea2f7-115">Microsoft Graph on hakemiston, käyttäjätietojen ja käytön hallinnan suositeltu ohjelmointirajapinta.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="ea2f7-116">Azure AD Graphin ja Microsoft Graphin välillä on kuitenkin vielä muutamia aukkoja.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="ea2f7-117">Tutustu seuraaviin artikkeleihin, joissa korostetaan uusimpia eroja, jotka auttavat valitsemaan:</span><span class="sxs-lookup"><span data-stu-id="ea2f7-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="ea2f7-118">Resurssityyppierot Azure AD Graphin ja Microsoft Graphin välillä</span><span class="sxs-lookup"><span data-stu-id="ea2f7-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="ea2f7-119">Azure AD Graphin ja Microsoft Graphin ominaisuuden erot</span><span class="sxs-lookup"><span data-stu-id="ea2f7-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="ea2f7-120">Azure AD:n ja Microsoft Graphin väliset menetelmäerot</span><span class="sxs-lookup"><span data-stu-id="ea2f7-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="ea2f7-121">**Kun kyselen *käyttäjäobjektia,* monet sen ominaisuuksista puuttuvat**</span><span class="sxs-lookup"><span data-stu-id="ea2f7-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="ea2f7-122">`GET https://graph.microsoft.com/v1.0/users` palauttaa vain 11 kohdetta, sillä Microsoft Graph valitsee automaattisesti oletusarvoisen *palautettavan käyttäjäominaisuuksien* joukon.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="ea2f7-123">Jos tarvitset muita *käyttäjäominaisuuksia,* $select valita sovelluksen ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="ea2f7-124">Kokeile sitä ensin **Microsoft Graph Explorerissa.**</span><span class="sxs-lookup"><span data-stu-id="ea2f7-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="ea2f7-125">**Jotkin käyttäjän ominaisuusarvot ovat *tyhjiä,* vaikka tiedän, että ne on määritetty**</span><span class="sxs-lookup"><span data-stu-id="ea2f7-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="ea2f7-126">Todennäköisin selitys on se, että sovellukselle oli myönnetty *User.ReadBasic.All-käyttöoikeus.*</span><span class="sxs-lookup"><span data-stu-id="ea2f7-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="ea2f7-127">Näin sovellus voi lukea rajoitetun käyttäjäominaisuuksien joukon ja palauttaa kaikki muut ominaisuudet tyhjäarvoksi, vaikka ne olisi aiemmin määritetty.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="ea2f7-128">Kokeile myöntää sovelluksen *User.Read.All-käyttöoikeus* sen sijaan.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="ea2f7-129">Lisätietoja on kohdassa [Microsoft Graphin käyttöoikeudet.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)</span><span class="sxs-lookup"><span data-stu-id="ea2f7-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="ea2f7-130">**I'm having trouble using OData query parameters to filter data in my requests**</span><span class="sxs-lookup"><span data-stu-id="ea2f7-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="ea2f7-131">Microsoft Graph tukee laajaa valikoimaa OData-kyselyn parametreja, mutta Microsoft Graphin hakemistopalvelut (hakemisto-objektista periytyvät *resurssit)* eivät tue kaikkia näitä parametreja.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="ea2f7-132">Samat rajoitukset, joita Azure AD Graphissa oli, säilyvät suurin piirtin Microsoft Graphissa:</span><span class="sxs-lookup"><span data-stu-id="ea2f7-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="ea2f7-133">**Ei tueta:**$count, $search tyhjäarvot ja $filter  *tyhjäarvot*</span><span class="sxs-lookup"><span data-stu-id="ea2f7-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="ea2f7-134">**Ei tueta:**$filter ominaisuuksista (katso resurssiaiheet, joista ominaisuudet ovat suodatettavissa)</span><span class="sxs-lookup"><span data-stu-id="ea2f7-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="ea2f7-135">**Ei tuettu:** sivutus, suodatus ja lajittelu samanaikaisesti</span><span class="sxs-lookup"><span data-stu-id="ea2f7-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="ea2f7-136">**Ei tuettu:** yhteyden suodattaminen.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="ea2f7-137">Voit esimerkiksi etsiä kaikki Yhdistyneessä kuningaskunnassa sijaitsevat tekniset ryhmän jäsenet.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="ea2f7-138">**Osittainen tuki:**$orderby *(vain* displayName ja userPrincipalName) ja *ryhmä*</span><span class="sxs-lookup"><span data-stu-id="ea2f7-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="ea2f7-139">**Osittainen tuki:** $filter (tukee vain *eq-,* *startswith-* tai ja , ja rajoitettuja) tuki-, $expand (yksittäisen objektin suhteiden laajentaminen palauttaa kaikki yhteydet, mutta objektien suhteiden laajentaminen on rajoitettua)  </span><span class="sxs-lookup"><span data-stu-id="ea2f7-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="ea2f7-140">Lisätietoja on kohdassa Vastausten [mukauttaminen kyselyparametrien avulla.](https://docs.microsoft.com/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="ea2f7-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="ea2f7-141">**Ohjelmointirajapinta, johon soitan, ei toimi – missä voin tehdä enemmän testausta?**</span><span class="sxs-lookup"><span data-stu-id="ea2f7-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="ea2f7-142">**Microsoft Graph Explorer** – Testaa Microsoft Graph -ohjelmointirajapinnat vuokraajassa  tai esittely vuokraajassa ja tutustu myös mallikyselyihin Microsoft Graph Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="ea2f7-143">**Kun kyselen tietoja, näyttää siltä, että saan puutteelliset tiedot takaisin**</span><span class="sxs-lookup"><span data-stu-id="ea2f7-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="ea2f7-144">Jos kyselet kokoelmaa (kuten *käyttäjiä),* Microsoft Graph käyttää palvelinpuolen sivurajoituksia, joten tulokset palautetaan aina oletussivun kokoisena.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="ea2f7-145">Sovelluksen pitäisi aina odottaa näkevän palvelun palauttamia kokoelmia.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="ea2f7-146">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="ea2f7-146">For more information, see:</span></span>

- [<span data-ttu-id="ea2f7-147">Microsoft Graphin parhaat käytännöt</span><span class="sxs-lookup"><span data-stu-id="ea2f7-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="ea2f7-148">Microsoft Graph -tietojen sivutus sovelluksessa</span><span class="sxs-lookup"><span data-stu-id="ea2f7-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="ea2f7-149">**Sovellukseni on liian hidas ja sitä myös käytetään kursivassa. Mitä parannuksia voin tehdä?**</span><span class="sxs-lookup"><span data-stu-id="ea2f7-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="ea2f7-150">Skenaariostasi riippuen käytettävissäsi on useita vaihtoehtoja, joilla voit tehdä sovelluksesta entistä tehokkaammin ja joissakin tapauksissa vähemmän altis palvelun utelle (kun puheluita on liikaa).</span><span class="sxs-lookup"><span data-stu-id="ea2f7-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="ea2f7-151">Lisätietoja on ohjeaiheissa:</span><span class="sxs-lookup"><span data-stu-id="ea2f7-151">To learn more, see:</span></span>

- [<span data-ttu-id="ea2f7-152">Microsoft Graphin parhaat käytännöt</span><span class="sxs-lookup"><span data-stu-id="ea2f7-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="ea2f7-153">Siirtopyynnöt</span><span class="sxs-lookup"><span data-stu-id="ea2f7-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="ea2f7-154">Muutosten jäljitäminen deltakyselyn avulla</span><span class="sxs-lookup"><span data-stu-id="ea2f7-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="ea2f7-155">Saa ilmoituksia muutoksista verkko-osien kautta</span><span class="sxs-lookup"><span data-stu-id="ea2f7-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="ea2f7-156">Kursimisohjeet</span><span class="sxs-lookup"><span data-stu-id="ea2f7-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="ea2f7-157">**Mistä löydän lisätietoja virheistä ja tunnetuista ongelmista?**</span><span class="sxs-lookup"><span data-stu-id="ea2f7-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="ea2f7-158">Microsoft Graphin virhevastaustiedot</span><span class="sxs-lookup"><span data-stu-id="ea2f7-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="ea2f7-159">Microsoft Graphin tunnetut ongelmat</span><span class="sxs-lookup"><span data-stu-id="ea2f7-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="ea2f7-160">**Mistä voin tarkistaa palvelun käytettävyyden ja yhteyden tilan?**</span><span class="sxs-lookup"><span data-stu-id="ea2f7-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="ea2f7-161">Niiden taustalla olevien palvelujen käytettävyys ja yhteydet, joita voidaan käyttää Microsoft Graphin kautta, voivat vaikuttaa Microsoft Graphin yleiseen käytettävuuteen ja suorituskykyyn.</span><span class="sxs-lookup"><span data-stu-id="ea2f7-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="ea2f7-162">Tarkista Azure Active Directory -palvelun kuntoa varten Azure-tilasivulla lueteltujen **suojaus-** ja [käyttäjätietopalvelujen tila.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="ea2f7-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="ea2f7-163">Tarkista Microsoft Graphiin osallistuneet Office-palvelut Office Service Health -koontinäytössä lueteltujen [palvelujen tila.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="ea2f7-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
