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
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662927"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="a5d58-102">Edellyttää asiakkaan Facing H1, H2 ei toimi</span><span class="sxs-lookup"><span data-stu-id="a5d58-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="a5d58-103">Esimerkiksi teksti estä - noudattamalla seuraavia ohjeita:</span><span class="sxs-lookup"><span data-stu-id="a5d58-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="a5d58-104">**AlchemyInsights** -kansiossa olevat tiedostot olisi oltava säännön tunnus ja [Alkemia kumppani portal](https://alchemyportal.azurewebsites.net) -säännön nimi tiedostonimi.</span><span class="sxs-lookup"><span data-stu-id="a5d58-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="a5d58-p101">esimerkiksi ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="a5d58-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="a5d58-p102">Käyttää tämän tiedoston yläosassa metatietojen malli. Mitään muuta ei tarvita.</span><span class="sxs-lookup"><span data-stu-id="a5d58-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="a5d58-109">[Alkemia kumppani portaali](https://alchemyportal.azurewebsites.net)Siirry osioon **Customer Insight-otsikko:** ja käyttö, joka alkavan osoittaa että H1 otsikko insight.</span><span class="sxs-lookup"><span data-stu-id="a5d58-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="a5d58-p103">Alkemia näkemyksistä on oltava vain yksi H1 yläreunassa tai ne lakkaavat toimimasta tuotannossa. H2s ei tehdä, niin Käytä **lihavointia** tai muiden sopimusten kommunikoinnin erillisiä osia.</span><span class="sxs-lookup"><span data-stu-id="a5d58-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="a5d58-112">Täytä seuraavaksi luonnoksesta aines käyttäen Alkemia sääntö-sivun kohdassa asiakkaiden näkemyksistä leipäteksti</span><span class="sxs-lookup"><span data-stu-id="a5d58-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="a5d58-113">Luettelomerkein varustetut luettelot on hieno</span><span class="sxs-lookup"><span data-stu-id="a5d58-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="a5d58-114">Numeroitujen luetteloiden liian</span><span class="sxs-lookup"><span data-stu-id="a5d58-114">Numbered lists too</span></span>
    1. <span data-ttu-id="a5d58-115">**Lihavointi** ja *kursivointi* on a-ok</span><span class="sxs-lookup"><span data-stu-id="a5d58-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="a5d58-116">Linkit on aina oltava joko **linkkejä ”web” tai ulkoisen** tai **syvä linkkejä Käyttöliittymän osat**, ei ole sisäisiä linkkejä.</span><span class="sxs-lookup"><span data-stu-id="a5d58-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="a5d58-p104">Ja tämä on todella jo hieman liian pitkä. Paras käytäntö on noin 400 merkkiä---</span><span class="sxs-lookup"><span data-stu-id="a5d58-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="a5d58-p105">Kun sisältösi on valmiina, erotettu elävään oksaan. Siirry [portal Alkemia kumppani](https://alchemyportal.azurewebsites.net) , ja kirjoita URL-osoite-kenttään tiedoston nimi. Varmista, että tarkistaa ja julkaista Insight sanoo ”Kyllä” ja valitse sitten päivitys. (Tämä näyttää prettier portal - vapauttaa pian uuteen versioon.)</span><span class="sxs-lookup"><span data-stu-id="a5d58-p105">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. (This will look prettier in the new version of the portal - releasing soon.)</span></span>

![URL-kenttä](media/for-content-team.PNG)

