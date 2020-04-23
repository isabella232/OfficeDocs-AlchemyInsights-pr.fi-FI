---
title: Vaihda Classic juuri sivuston modernin sivuston
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741541"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Vaihda Classic juuri sivuston modernin sivuston

Jos ympäristöon määritetty ennen huhtikuuta 2019, voit muuttaa pääsivuston moderniksi sivustoksi Microsoft PowerShellin avulla:

- Jos sinulla on eri sivusto, jota haluat käyttää pääsivustona, voit korvata [(vaihtaa) juurisivuston](https://docs.microsoft.com/sharepoint/modern-root-site) sillä. 
    - [Käytä Invoke-SPOSiteSwapia](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) sivuston sijainnin vaihtamiseen toisen sivuston kanssa alkuperäisen sivuston arkistoimisen aikana. Käytettävissä sekä ryhmäsivustossa (ei yhdistettynä ryhmään) että viestintäsivustossa. 

- Pian otetaan käyttöön lisäominaisuuksia, joiden avulla voit jatkaa sivuston sisällön käyttämistä, mutta muuntaa aiemmin luodun sivuston viestintäsivustoksi. 
>[!Important]
>Nämä ominaisuudet otetaan käyttöön vähitellen. Jatka päivitysten tarkistamista Viestikeskuksesta. 

## <a name="known-issues-with-swapping-sites"></a>Sivustojen vaihtamisen tunnetut ongelmat

- Kohdesivusto saattaa palauttaa http 404 (ei löydy) -virheen lyhyeksi ajaksi.
- Hakuindeksin päivittäminen edellyttää sisällön indeksointia uudelleen. Manuaalista vaihetta ei tarvita - tämä tehdään automaattisesti.
- Kaikki staattisesta linkistä riippuvaiset linkit (kuten Tiedostojen synkronointi ja OneNote-tiedostot) on korjattava manuaalisesti.
- Jos lähdesivusto oli organisaation uutissivusto, päivitä URL-osoite.Saat luettelon kaikista organisaation uutissivustoista.
- Project Server -sivustot on ehkä vahvistettava, jotta ne voidaan edelleen liittää oikein.
