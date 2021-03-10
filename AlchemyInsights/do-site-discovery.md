---
title: Sivuston etsiminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693489"
---
# <a name="do-site-discovery"></a><span data-ttu-id="32dce-102">Sivuston etsiminen</span><span class="sxs-lookup"><span data-stu-id="32dce-102">Do site discovery</span></span>

<span data-ttu-id="32dce-103">Jos organisaatiosi käyttää edelleen vanhoja verkkosovelluksia ja aikoo käyttää Internet Explorer -tilaa (jota useimmat asiakkaat käyttävät), sinun kannattaa tehdä lisää sivuston etsintää.</span><span class="sxs-lookup"><span data-stu-id="32dce-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="32dce-104">**Olet jo ottanut käyttöön Vanhemman Microsoft Edge -version**</span><span class="sxs-lookup"><span data-stu-id="32dce-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="32dce-105">Jos olet jo määrittänyt yrityssivustoluettelon toimimaan Microsoft Edgen vanhan version kanssa, sivuston etsintä on melkein valmis.</span><span class="sxs-lookup"><span data-stu-id="32dce-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="32dce-106">Yksi asia, joka sinun on ehkä lisättävä, on lisätä neutraalit sivustot.</span><span class="sxs-lookup"><span data-stu-id="32dce-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="32dce-107">Neutraalit sivustot ovat yleensä sivustoja, jotka tarjoavat kertakirjautumisen.</span><span class="sxs-lookup"><span data-stu-id="32dce-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="32dce-108">Jos siirryt Microsoft Edgestä neutraaliin sivustoon, haluat pysyä Microsoft Edgessä todennetuksi.</span><span class="sxs-lookup"><span data-stu-id="32dce-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="32dce-109">Jos siirryt neutraaliin sivustoon Internet Explorer -tilassa, haluat pysyä Internet Explorer -tilassa todentaaksesi sen.</span><span class="sxs-lookup"><span data-stu-id="32dce-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="32dce-110">Tunnista kaikki SSO-sivustot tai muut neutraalit sivustot, joita käytät, ja lisää ne yrityssivustoluetteloon.</span><span class="sxs-lookup"><span data-stu-id="32dce-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="32dce-111">**Internet Explorer on oletusselaimesi**</span><span class="sxs-lookup"><span data-stu-id="32dce-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="32dce-112">Jos käytät vain Internet Exploreria nyt, et ehkä tiedä, mitkä sivustot ovat päivitetneet moderneihin verkkostandardeihin ja mitkä edellyttävät edelleen Internet Exploreria.</span><span class="sxs-lookup"><span data-stu-id="32dce-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="32dce-113">Haluat etsiä ja lisätä nämä sivustot yrityssivustoluetteloon, jotta voit käyttää Internet Explorer -tilaa vain kyseisissä sivustoissa.</span><span class="sxs-lookup"><span data-stu-id="32dce-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="32dce-114">[Enterprise Site Discovery löytää](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) sivustot, jotka saattavat tarvita Internet Explorer -tilaa.</span><span class="sxs-lookup"><span data-stu-id="32dce-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="32dce-115">Se voi kerätä tietoja tietokoneista, joissa on Windows Internet Explorer 8 – Internet Explorer 11 Windows 10:ssä, Windows 8.1:ssä tai Windows 7:ssä.</span><span class="sxs-lookup"><span data-stu-id="32dce-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="32dce-116">**Tietojen analysointi**</span><span class="sxs-lookup"><span data-stu-id="32dce-116">**Analyze the data**</span></span>

<span data-ttu-id="32dce-117">Kun olet kerännyt sivustotiedot, suosittelemme tietojen analysoimiseen seuraavaa nelivaiheista prosessia:</span><span class="sxs-lookup"><span data-stu-id="32dce-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="32dce-118">Lajittele tiedot toimialueen ja URL-osoitteen mukaan.</span><span class="sxs-lookup"><span data-stu-id="32dce-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="32dce-119">Määritä internet Explorer -tilaa varten määritettävät sovelluksen rajat.</span><span class="sxs-lookup"><span data-stu-id="32dce-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="32dce-120">Haluat sisällyttää kaikki sovelluksen määrittävät sivustot ja verkko-ohjausobjektit, mutta et halua sisällyttää ylimääräisiä sivustoja ja ohjausobjekteja.</span><span class="sxs-lookup"><span data-stu-id="32dce-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="32dce-121">Jotkin sivustot voivat olla yhtä *https://contoso.com/app1* yksinkertaisia, kun taas toiset saattavat edellyttää useiden sivustojen ja sivujen määrittelemiseen.</span><span class="sxs-lookup"><span data-stu-id="32dce-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="32dce-122">Testaa sovellus sen varmistamiseksi, että se ei toimi natiivisti.</span><span class="sxs-lookup"><span data-stu-id="32dce-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="32dce-123">Monet sivustot tarjoavat modernia sisältöä, kun ne tunnistavat nykyaikaisen selaimen ja tarjoavat vanhaa sisältöä vain, kun ne tunnistavat Internet Explorerin.</span><span class="sxs-lookup"><span data-stu-id="32dce-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="32dce-124">Lisää sovellus yrityssivustoluetteloon, jos sovelluksen testaus epäonnistuu.</span><span class="sxs-lookup"><span data-stu-id="32dce-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="32dce-125">Parhaana käytäntönä voit ryhmitellä kaikki sivustot, jotka muodostavat sovelluksen.</span><span class="sxs-lookup"><span data-stu-id="32dce-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="32dce-126">Näin kun päivität sovelluksen, koko sivusto on helpompi poistaa Internet Explorer -tilasta ja aloittaa sovelluksen modernin selaimen käyttö.</span><span class="sxs-lookup"><span data-stu-id="32dce-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="32dce-127">Kun olet tehnyt sivuston etsinnän ja analysoinut tiedot, voit aloittaa kanavastrategian tarkastelemisen.</span><span class="sxs-lookup"><span data-stu-id="32dce-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

