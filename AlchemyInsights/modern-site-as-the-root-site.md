---
title: Moderni sivusto kuin pääsivusto
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054699"
---
# <a name="modern-site-as-root-site"></a>Moderni sivusto pääsivusto

Olemme alkaneet ottaa käyttöön uuden ominaisuuden, jonka avulla voit [vaihtaa klassisen sivuston juuri sivuston modernilla sivustolla](https://docs.microsoft.com/sharepoint/modern-root-site). Käytä [Kutsu-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , jos haluat vaihtaa sivuston sijainnin toisen sivuston kanssa arkistoitaessa alkuperäistä sivustoa. Käytettävissä sekä ryhmäsivustoon (ei yhdistetty ryhmään) että viestintä sivustoon.

>[!Important]
> Älä poista klassista pääsivustoa, jotta voit luoda nykyaikaisen viestintä paikan. Microsoft ei tue tätä. Pääsivuston poistaminen tekee kaikista organisaatioosi kuuluvista SharePoint-sivustoista kaikkien käyttäjien käytettävissä, kunnes palautat sivuston tai luot uuden sivuston samaan URL-osoitteeseen. Viestimme tästä ominaisuudesta viesti keskuksen kautta. Odota, että ominaisuus on käytössä vuokraajassasi lähiaikoina.

## <a name="known-issues-with-swapping-sites"></a>Sivustojen vaihtamisen tunnetut ongelmat
- Kohde sivusto saattaa palauttaa virheen "ei löytynyt" (HTTP 404), joka on lyhyt ajan jakso.
- Sisältö on indeksoida uudelleen, jotta haku indeksi voidaan päivittää. Tässä ei ole manuaalista vaihetta, tämä tapahtuu automaattisesti.
- Kaikki, jotka ovat riippuvaisia "staattisista" linkeistä (kuten tiedostojen synkronointi ja OneNote-tiedostot), on korjattava manuaalisesti.
- Project Server-sivustot on ehkä validoitava sen varmistamiseksi, että ne liittyvät edelleen oikein. 
