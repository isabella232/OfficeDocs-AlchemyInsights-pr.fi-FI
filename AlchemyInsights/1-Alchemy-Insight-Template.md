---
title: 'sama tiedostonimi on paras [sääntö #-kuvaus]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697127"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="b3670-102">Edellyttää Alkemia otsikon H1, H2 ja eivät toimi.</span><span class="sxs-lookup"><span data-stu-id="b3670-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="b3670-103">Parhaita käytäntöjä ja ohjeita Alkemia authoring:</span><span class="sxs-lookup"><span data-stu-id="b3670-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="b3670-p101">**Alkemia asuun kansioihin ei luoda sisäkkäisiä**- se hajottaa url-rakenteen. Näkymä korjataan tämä levy.</span><span class="sxs-lookup"><span data-stu-id="b3670-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="b3670-106">**AlchemyInsights** -kansiossa olevat tiedostot olisi oltava säännön tunnus ja [Alkemia kumppani portal](https://alchemyportal.azurewebsites.net) -säännön nimi tiedostonimi.</span><span class="sxs-lookup"><span data-stu-id="b3670-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="b3670-p102">esimerkiksi ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="b3670-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="b3670-p103">Käyttää tämän tiedoston yläosassa metatietojen malli. Mitään muuta ei tarvita.</span><span class="sxs-lookup"><span data-stu-id="b3670-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="b3670-111">[Alkemia kumppani portaali](https://alchemyportal.azurewebsites.net)Siirry osioon **Customer Insight-otsikko:** ja käyttö, joka alkavan osoittaa että H1 otsikko insight.</span><span class="sxs-lookup"><span data-stu-id="b3670-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="b3670-p104">Alkemia näkemyksistä on oltava vain yksi H1 yläreunassa tai ne lakkaavat toimimasta tuotannossa. H2s ei tehdä, niin Käytä **lihavointia** tai muiden sopimusten kommunikoinnin erillisiä osia.</span><span class="sxs-lookup"><span data-stu-id="b3670-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="b3670-114">Täytä seuraavaksi luonnoksesta aines käyttäen Alkemia sääntö-sivun kohdassa asiakkaiden näkemyksistä leipäteksti</span><span class="sxs-lookup"><span data-stu-id="b3670-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="b3670-115">Luettelomerkein varustetut luettelot on hieno</span><span class="sxs-lookup"><span data-stu-id="b3670-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="b3670-116">Numeroitujen luetteloiden liian</span><span class="sxs-lookup"><span data-stu-id="b3670-116">Numbered lists too</span></span>
    1. <span data-ttu-id="b3670-117">**Lihavointi** ja *kursivointi* on a-ok</span><span class="sxs-lookup"><span data-stu-id="b3670-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="b3670-118">Linkit on aina oltava joko **linkkejä ”web” tai ulkoisen** tai **syvä linkkejä Käyttöliittymän osat**, ei ole sisäisiä linkkejä.</span><span class="sxs-lookup"><span data-stu-id="b3670-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="b3670-p105">Ja tämä on todella jo hieman liian pitkä. Paras käytäntö on noin 400 merkkiä---</span><span class="sxs-lookup"><span data-stu-id="b3670-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="b3670-p106">Kun sisältösi on valmiina, erotettu elävään oksaan. Siirry [portal Alkemia kumppani](https://alchemyportal.azurewebsites.net) , ja kirjoita URL-osoite-kenttään tiedoston nimi. Varmista, että tarkistaa ja julkaista Insight sanoo ”Kyllä” ja valitse sitten päivitys. **(Tämä näyttää prettier portal - vapauttaa pian uuteen versioon.)** 
 ![url-kenttä](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="b3670-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

