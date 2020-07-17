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
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750967"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="49b61-102">"Pakollinen Alchemy Header H1, H2: n eivät toimi."</span><span class="sxs-lookup"><span data-stu-id="49b61-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="49b61-103">Alchemyn luontia koskevat parhaat käytännöt ja ohjeet:</span><span class="sxs-lookup"><span data-stu-id="49b61-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="49b61-104">**Älä pesä Alchemy Oivalluksia kansioihin**- tämä rikkoo url-rakenne.</span><span class="sxs-lookup"><span data-stu-id="49b61-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="49b61-105">Tutkimme tämän korjaamista.</span><span class="sxs-lookup"><span data-stu-id="49b61-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="49b61-106">**AlchemyInsights-kansion** tiedostoissa on oltava pienet tiedostonimet, joissa on välilyöntejä ex.</span><span class="sxs-lookup"><span data-stu-id="49b61-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="49b61-107">***miten-to-enable-riita-oikeus -pidä***.</span><span class="sxs-lookup"><span data-stu-id="49b61-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="49b61-108">Sisällytä sääntötunnus tai säilötunnus [Alchemy Partner -portaalista](https://alchemyportal.azurewebsites.net) ms.custom-kenttään.</span><span class="sxs-lookup"><span data-stu-id="49b61-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="49b61-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="49b61-109">ex.</span></span> <span data-ttu-id="49b61-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="49b61-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="49b61-111">Käytä mallina muita tämän tiedoston yläosassa olevia metatietoja.</span><span class="sxs-lookup"><span data-stu-id="49b61-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="49b61-112">Siirry [Alchemy Partner -portaalissa](https://alchemyportal.azurewebsites.net) **asiakastietojen otsikko** -osioon ja käytä sitä H1-otsikon lähtökohtana.</span><span class="sxs-lookup"><span data-stu-id="49b61-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="49b61-113">Alkemia Oivalluksia on oltava vain yksi H1 yläreunassa tai ne rikkovat tuotannossa.</span><span class="sxs-lookup"><span data-stu-id="49b61-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="49b61-114">H2s ei hahmonnu, joten käytä **lihavointia** tai muita käytäntöjä eri osien merkitsemiseen.</span><span class="sxs-lookup"><span data-stu-id="49b61-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="49b61-115">Täytä seuraavaksi leipäteksti käyttämällä Alchemy-sääntö-sivun Asiakastiedot-osion luonnosmateriaalia.</span><span class="sxs-lookup"><span data-stu-id="49b61-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="49b61-116">Luettelomerkeillä varustetut luettelot ovat kunnossa</span><span class="sxs-lookup"><span data-stu-id="49b61-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="49b61-117">Myös numeroidut luettelot</span><span class="sxs-lookup"><span data-stu-id="49b61-117">Numbered lists too</span></span>
    1. <span data-ttu-id="49b61-118">**Lihavoitu** ja *kursivoitu* ovat-ok</span><span class="sxs-lookup"><span data-stu-id="49b61-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="49b61-119">Linkkien pitäisi aina olla joko **"linkkejä web"/ ulkoinen** TAI **syvä-linkkejä käyttöliittymän elementtejä,** ei sisäisiä linkkejä.</span><span class="sxs-lookup"><span data-stu-id="49b61-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="49b61-120">Kuvia ei virallisesti tueta tällä hetkellä, mutta se on etenemissuunnitelmassa.</span><span class="sxs-lookup"><span data-stu-id="49b61-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="49b61-121">Ja tämä on todella jo hieman liian pitkä.</span><span class="sxs-lookup"><span data-stu-id="49b61-121">And this is really already a bit too long.</span></span> <span data-ttu-id="49b61-122">Paras käytäntö on noin 400 merkkiä ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="49b61-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="49b61-123">Kun sisältö on valmis, vedä se live-haaraan.</span><span class="sxs-lookup"><span data-stu-id="49b61-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="49b61-124">Siirry sitten [Alchemy Partner -portaaliin](https://alchemyportal.azurewebsites.net) ja kirjoita tiedostonimi URL-kenttään.</span><span class="sxs-lookup"><span data-stu-id="49b61-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 