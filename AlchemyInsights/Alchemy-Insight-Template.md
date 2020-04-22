---
title: sama kuin tiedostonimi on paras
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676530"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="86d8e-102">Pakollinen Alkemia Header H1, H2: n eivät toimi.</span><span class="sxs-lookup"><span data-stu-id="86d8e-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="86d8e-103">Alkemian kirjoittamisen parhaat käytännöt ja ohjeet:</span><span class="sxs-lookup"><span data-stu-id="86d8e-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="86d8e-104">**Älä pese Alchemy Insights kansioihin**- tämä rikkoo URL-rakenne.</span><span class="sxs-lookup"><span data-stu-id="86d8e-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="86d8e-105">Tutkimme tämän korjaamista.</span><span class="sxs-lookup"><span data-stu-id="86d8e-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="86d8e-106">**AlchemyInsights-kansion** tiedostoissa on oltava pienet tiedostonimet, joissa on välilyöntejä varten välilyöntejä, kuten välilyöntejä varten.</span><span class="sxs-lookup"><span data-stu-id="86d8e-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="86d8e-107">***how-to-enable-litigation-hold***.</span><span class="sxs-lookup"><span data-stu-id="86d8e-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="86d8e-108">Sisällytä [alchemy-kumppaniportaalin](https://alchemyportal.azurewebsites.net) sääntötunnus tai ämpäritunnus ms.custom-kenttään.</span><span class="sxs-lookup"><span data-stu-id="86d8e-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="86d8e-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="86d8e-109">ex.</span></span> <span data-ttu-id="86d8e-110">***Ms.custom: 100021 (suomi)***</span><span class="sxs-lookup"><span data-stu-id="86d8e-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="86d8e-111">Käytä muita metatietoja tämän tiedoston yläosassa mallina.</span><span class="sxs-lookup"><span data-stu-id="86d8e-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="86d8e-112">Siirry [Alchemy Partner -portaalissa](https://alchemyportal.azurewebsites.net)kohtaan **Asiakasnäkökulman otsikko:** ja käytä sitä h1-otsikon lähtökohtana.</span><span class="sxs-lookup"><span data-stu-id="86d8e-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="86d8e-113">Alkemia Oivalluksia on vain yksi H1 yläreunassa tai ne rikkoa tuotannossa.</span><span class="sxs-lookup"><span data-stu-id="86d8e-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="86d8e-114">H2s ei tee joko niin käyttää **lihavoitu** tai muita käytäntöjä merkitä erillisiä osia.</span><span class="sxs-lookup"><span data-stu-id="86d8e-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="86d8e-115">Täytä seuraavaksi leipäteksti käyttämällä luonnosmateriaalia Alchemy Rule -sivun Asiakastilastot-osassa.</span><span class="sxs-lookup"><span data-stu-id="86d8e-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="86d8e-116">Luettelomerkeillä varustetut luettelot ovat hienoja</span><span class="sxs-lookup"><span data-stu-id="86d8e-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="86d8e-117">Myös numeroidut luettelot</span><span class="sxs-lookup"><span data-stu-id="86d8e-117">Numbered lists too</span></span>
    1. <span data-ttu-id="86d8e-118">**Lihavointi** ja *kursivointi* ovat-ok</span><span class="sxs-lookup"><span data-stu-id="86d8e-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="86d8e-119">Linkkien tulisi aina olla joko **"linkkejä web"/ ulkoinen** tai **syvä-linkkejä käyttöliittymän elementtejä**, ei sisäisiä linkkejä.</span><span class="sxs-lookup"><span data-stu-id="86d8e-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="86d8e-120">Kuvia ei tueta virallisesti tällä hetkellä, mutta se on etenemissuunnitelmassa.</span><span class="sxs-lookup"><span data-stu-id="86d8e-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="86d8e-121">Ja tämä on oikeastaan jo hieman liian pitkä.</span><span class="sxs-lookup"><span data-stu-id="86d8e-121">And this is really already a bit too long.</span></span> <span data-ttu-id="86d8e-122">Parhaat käytännöt ovat noin 400 merkkiä ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="86d8e-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="86d8e-123">Kun sisältö on valmis, vedä se live-haaraan.</span><span class="sxs-lookup"><span data-stu-id="86d8e-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="86d8e-124">Siirry sitten [Alchemy Partner -portaaliin](https://alchemyportal.azurewebsites.net) ja kirjoita tiedostonimi URL-kenttään.</span><span class="sxs-lookup"><span data-stu-id="86d8e-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 