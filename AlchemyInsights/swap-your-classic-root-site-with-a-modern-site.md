---
title: Vaihda perinteinen pääsivusto modernilla sivustolla
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749257"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Vaihda perinteinen pääsivusto modernilla sivustolla

Jos ympäristösi on määritetty ennen huhtikuun 2019, voit muuttaa pääsivuston nykyaikaiseen sivustoon Microsoft PowerShellin avulla:

- Jos sinulla on eri sivusto, jota haluat käyttää pääsivustoosi, voit korvata [(swap) pääsivuston](https://docs.microsoft.com/sharepoint/modern-root-site) sen kanssa. 
    - Käytä [Kutsu-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , jos haluat vaihtaa sivuston sijainnin toisen sivuston kanssa arkistoitaessa alkuperäistä sivustoa. Käytettävissä sekä ryhmäsivustoon (ei yhdistetty ryhmään) että viestintä sivustoon. 

- Pian otetaan käyttöön lisä ominaisuuksia, joiden avulla voit jatkaa sivuston sisällön käyttämistä, mutta muuntaa olemassa olevan sivuston viestintä sivustoksi. 
>[!Important]
>Nämä ominaisuudet otetaan käyttöön vähitellen. Jatka Office 365-Message Center-päivitysten tarkistaminen. 

## <a name="known-issues-with-swapping-sites"></a>Sivustojen vaihtamisen tunnetut ongelmat

- Kohde sivusto saattaa palauttaa virheen "ei löytynyt" (HTTP 404), joka on lyhyt ajan jakso.
- Sisältö on indeksoida uudelleen, jotta haku indeksi voidaan päivittää. Manuaalista vaihetta ei tarvita-tämä tapahtuu automaattisesti.
- Kaikki, jotka ovat riippuvaisia "staattisista" linkeistä (kuten tiedostojen synkronointi ja OneNote-tiedostot), on korjattava manuaalisesti.
- Jos lähdesivusto oli organisaation uutisivusto, Päivitä URL-osoite.Hanki luettelo kaikista organisaation uutis sivustoista.
- Project Server-sivustot on ehkä validoitava sen varmistamiseksi, että ne liittyvät edelleen oikein.





