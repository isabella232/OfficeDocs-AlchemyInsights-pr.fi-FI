---
title: Nykyaikainen sivusto pääsivustona
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000389"
---
# <a name="modern-site-as-root-site"></a>Nykyaikainen sivusto pääsivustona

Olemme aloittaneet uuden ominaisuuden käytön, jonka avulla voit vaihtaa perinteisen [sivuston pääsivuston nykyaikaiseen sivustoon.](https://docs.microsoft.com/sharepoint/modern-root-site) [Invoke-SPOSiteSwap-toiminnon](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) avulla voit vaihtaa sivuston sijainnin toiseen sivustoon samalla, kun arkistoit alkuperäistä sivustoa. Käytettävissä sekä ryhmäsivustolle (ei ole yhteydessä ryhmään) että viestintäsivustolle.

>[!Important]
> Älä poista perinteistä pääsivustoa uuden viestintäsivuston luomiseen. Microsoft ei tue tätä. Pääsivuston poistaminen poistaa kaikki SharePoint organisaation sivustot eivät ole kaikkien käyttäjien käytettävissä, kunnes palautat sivuston tai luot uuden sivuston samaan URL-osoitteeseen. Lähetämme tämän toiminnon viestikeskuksen kautta. Ominaisuuden pitäisi pian olla käytössä vuokraajassasi.

## <a name="known-issues-with-swapping-sites"></a>Tunnetut ongelmat sivustojen vaihtamisessa
- Kohdesivusto saattaa palauttaa "ei löydy" (HTTP 404) -virheen lyhyen aikaa.
- Sisältö on päivitettävä uudelleen, jotta hakuindeksi voidaan päivittää. Tässä ei tarvita manuaalista vaihetta, tämä tehdään automaattisesti.
- Kaikki, mikä riippuu staattisista linkeistä (kuten tiedostojen synkronoinnista ja OneNote-tiedostoista), on korjattava manuaalisesti.
- Project Palvelinsivustot on ehkä vahvistettava, jotta ne voidaan liittää oikein. 
