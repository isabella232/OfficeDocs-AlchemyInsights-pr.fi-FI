---
title: Moderni sivusto pääsivustona
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713788"
---
# <a name="modern-site-as-root-site"></a>Moderni sivusto pääsivustona

Olemme alkaneet ottaa käyttöön uusi ominaisuus, jonka avulla voit [vaihtaa klassinen sivuston juuri sivuston moderni sivusto](https://docs.microsoft.com/sharepoint/modern-root-site). [Käytä Invoke-SPOSiteSwapia](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) sivuston sijainnin vaihtamiseen toisen sivuston kanssa alkuperäisen sivuston arkistoimisen aikana. Käytettävissä sekä ryhmäsivustossa (ei yhdistettynä ryhmään) että viestintäsivustossa.

>[!Important]
> Älä poista perinteistä pääsivustoasi luodaksesi modernin viestintäsivuston. Microsoft ei tue tätä. Pääsivuston poistaminen tekee kaikista organisaation SharePoint-sivustoista kaikkien käyttäjien käytettävissä, kunnes palautat sivuston tai luot uuden sivuston samaan URL-osoitteeseen. Kommunikoimme tämän ominaisuuden viestikeskuksen kautta. Sinun pitäisi odottaa, että ominaisuus otetaan pian käyttöön vuokraajassasi.

## <a name="known-issues-with-swapping-sites"></a>Sivustojen vaihtamisen tunnetut ongelmat
- Kohdesivusto saattaa palauttaa http 404 (ei löydy) -virheen lyhyeksi ajaksi.
- Hakuindeksin päivittäminen edellyttää sisällön indeksointia uudelleen. Ei ole manuaalista vaihetta tarvitaan täällä, tämä tehdään automaattisesti.
- Kaikki staattisesta linkistä riippuvaiset linkit (kuten Tiedostojen synkronointi ja OneNote-tiedostot) on korjattava manuaalisesti.
- Project Server -sivustot on ehkä vahvistettava, jotta ne voidaan edelleen liittää oikein. 
