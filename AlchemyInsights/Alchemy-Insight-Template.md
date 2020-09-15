---
title: sama kuin tiedosto nimi on paras
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664131"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="30671-102">"Required Alchemy header H1, H2:n eivät toimi."</span><span class="sxs-lookup"><span data-stu-id="30671-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="30671-103">Parhaat käytännöt ja ohjeet alkemian luomiseen:</span><span class="sxs-lookup"><span data-stu-id="30671-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="30671-104">**Älä sisäkkäistä Alchemy**-tietoja kansioissa-Tämä murtaa URL-rakenteen.</span><span class="sxs-lookup"><span data-stu-id="30671-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="30671-105">Tarkastelemme korjausta.</span><span class="sxs-lookup"><span data-stu-id="30671-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="30671-106">**Alchemyinsights** -kansion tiedostoissa pitäisi olla pieniä tiedosto nimiä, joissa on tavu viivoja väli lyöntejä varten.</span><span class="sxs-lookup"><span data-stu-id="30671-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="30671-107">***toiminta ohjeet-Ota käyttöön-oikeuden käynnit-pito***.</span><span class="sxs-lookup"><span data-stu-id="30671-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="30671-108">Sisällytä säännön ID tai Bucket ID [Alchemyn partneri portaalista](https://alchemyportal.azurewebsites.net) MS. Custom-kentässä.</span><span class="sxs-lookup"><span data-stu-id="30671-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="30671-109">ex.</span><span class="sxs-lookup"><span data-stu-id="30671-109">ex.</span></span> <span data-ttu-id="30671-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="30671-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="30671-111">Käytä muita metatietoja tämän tiedoston yläosassa mallina.</span><span class="sxs-lookup"><span data-stu-id="30671-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="30671-112">Siirry [Alchemyn partneri portaalissa](https://alchemyportal.azurewebsites.net)alaspäin kohtaan **Customer Insight-otsikko:** ja käytä tätä, kun haluat saada tietoa.</span><span class="sxs-lookup"><span data-stu-id="30671-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="30671-113">Alchemy-tiedoissa on oltava vain yksi H1 yläreunassa tai ne hajoavat tuotannossa.</span><span class="sxs-lookup"><span data-stu-id="30671-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="30671-114">H2s Älä tee näin, vaan käytä **liha vointia** tai muita yleissopimuksia erillisten jaksojen merkiksi.</span><span class="sxs-lookup"><span data-stu-id="30671-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="30671-115">Täytä seuraavaksi leipä teksti käyttäen alkemia-sääntö sivun asiakas tiedot-osion luonnos materiaalia</span><span class="sxs-lookup"><span data-stu-id="30671-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="30671-116">Luettelo merkeillä varustetut luettelot ovat hyviä</span><span class="sxs-lookup"><span data-stu-id="30671-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="30671-117">Myös numero idut luettelot</span><span class="sxs-lookup"><span data-stu-id="30671-117">Numbered lists too</span></span>
    1. <span data-ttu-id="30671-118">**Liha vointi** ja *kursivointi* ovat a-OK</span><span class="sxs-lookup"><span data-stu-id="30671-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="30671-119">Linkkien on aina oltava joko **linkkejä sivustoon/ulkoiset** tai **syvät linkit käyttö liittymän elementteihin**, ei sisäisiä linkkejä.</span><span class="sxs-lookup"><span data-stu-id="30671-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="30671-120">Kuvia ei tällä hetkellä virallisesti tueta, mutta se on etenemis suunnitelmassa.</span><span class="sxs-lookup"><span data-stu-id="30671-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="30671-121">Ja tämä on oikeastaan jo liian pitkä aika.</span><span class="sxs-lookup"><span data-stu-id="30671-121">And this is really already a bit too long.</span></span> <span data-ttu-id="30671-122">Paras käytäntö on noin 400 merkkiä---------------------------------</span><span class="sxs-lookup"><span data-stu-id="30671-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="30671-123">Kun sisältö on valmis, vedä se Live-haaraan.</span><span class="sxs-lookup"><span data-stu-id="30671-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="30671-124">Siirry sitten [Alchemy-kumppanien portaaliin](https://alchemyportal.azurewebsites.net) ja kirjoita tiedosto nimi URL-kenttään.</span><span class="sxs-lookup"><span data-stu-id="30671-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 