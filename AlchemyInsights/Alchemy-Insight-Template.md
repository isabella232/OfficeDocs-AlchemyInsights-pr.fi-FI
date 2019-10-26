---
title: sama kuin tiedosto nimi on paras
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "35800042"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="cf0fb-102">Vaadittu Alchemy header H1, H2's ei toimi.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="cf0fb-103">Alchemy authoring-sivuston parhaat käytännöt ja ohjeet:</span><span class="sxs-lookup"><span data-stu-id="cf0fb-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="cf0fb-104">**Älä tuo Alchemy Insights-tietoja kansioihin**-tämä rikkoo URL-rakenteen.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="cf0fb-105">Pyrimme korjaamaan tämän.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="cf0fb-106">**Alchemyinnähtävyydet** -kansiossa olevilla tiedostoilla pitäisi olla pieniä tiedosto nimiä, joissa on yhdysmerkkejä (Spaces ex).</span><span class="sxs-lookup"><span data-stu-id="cf0fb-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="cf0fb-107">***toiminta ohjeet-oikeuden käynti-pito***.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="cf0fb-108">Sisällytä säännön tunnus tai kauhan tunnus [Alchemy-kumppani portaalista](https://alchemyportal.azurewebsites.net) MS. Custom-kenttään.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="cf0fb-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-109">ex.</span></span> <span data-ttu-id="cf0fb-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="cf0fb-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="cf0fb-111">Käytä loput metatiedot tämän tiedoston yläosassa mallina.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="cf0fb-112">Siirry [Alchemy-kumppani portaalissa](https://alchemyportal.azurewebsites.net)kohtaan **asiakas tiedon otsikko:** ja käytä sitä lähtö kohtana H1-otsikolla.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="cf0fb-113">Alchemy Insights-tiedoissa on oltava vain yksi H1 ylhäällä tai ne hajoavat tuotannossa.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="cf0fb-114">H2s Älä Hahmonna myöskään käytä **Lihavoidut** tai muut yleissopimukset, jotka merkitsevät erillisiä osia.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="cf0fb-115">Täytä seuraavaksi leipä teksti käyttämällä Alchemy-sääntö sivun Customer Insights-osan luonnos materiaalia.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="cf0fb-116">Luettelo merkeillä varustetut luettelot ovat hienoja</span><span class="sxs-lookup"><span data-stu-id="cf0fb-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="cf0fb-117">Myös numero idut luettelot</span><span class="sxs-lookup"><span data-stu-id="cf0fb-117">Numbered lists too</span></span>
    1. <span data-ttu-id="cf0fb-118">**Lihavoidut** ja *kursivat* ovat-OK</span><span class="sxs-lookup"><span data-stu-id="cf0fb-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="cf0fb-119">Linkkien tulee aina olla joko **"linkit Web-linkkejä"/ulkoisia** tai **syviä linkkejä käyttö liittymän elementteihin**, ei sisäisiin linkkeihin.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="cf0fb-120">Kuvia ei virallisesti tueta tällä hetkellä, mutta se on etenemis suunnitelmassa.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="cf0fb-121">Ja tämä on oikeastaan jo hieman liian pitkä aika.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-121">And this is really already a bit too long.</span></span> <span data-ttu-id="cf0fb-122">Paras käytäntö on noin 400 merkkiä---------------------------------</span><span class="sxs-lookup"><span data-stu-id="cf0fb-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="cf0fb-123">Kun sisältö on valmis, vedä se Live-haaraan.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="cf0fb-124">Siirry sitten [Alchemy-kumppani portaaliin](https://alchemyportal.azurewebsites.net) ja kirjoita tiedosto nimi URL-kenttään.</span><span class="sxs-lookup"><span data-stu-id="cf0fb-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 