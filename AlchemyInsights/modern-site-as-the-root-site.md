---
title: Moderni sivusto pääsivustona
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
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666867"
---
# <a name="modern-site-as-root-site"></a>Moderni sivusto pääsivustona

Olemme alkaneet ottaa käyttöön uuden ominaisuuden, jonka avulla voit [vaihtaa perinteisen sivuston pääsivustoa modernilla sivustolla](https://docs.microsoft.com/sharepoint/modern-root-site). Käytä [Invoke-SPOSiteSwap-](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) vaihto pistettä, jos haluat vaihtaa sivuston sijainnin toiseen sivustoon arkistoitaessa alkuperäistä sivustoa. Saatavilla sekä Ryhmäsivustolle (ei yhdistetty ryhmään) että Viestintäsivustoon.

>[!Important]
> Älä poista perinteistä pääsivustoa nykyaikaisen Viestintäsivuston luomi seksi. Microsoft ei tue tätä. Kun pääsivusto poistetaan, kaikki organisaation SharePoint-sivustot eivät ole kaikkien käyttäjien käytettävissä, ennen kuin palautat sivuston tai luot uuden sivuston samaan URL-osoitteeseen. Ilmoitamme tästä ominaisuudesta viesti keskuksen kautta. Sinun pitäisi odottaa, että ominaisuus otetaan käyttöön vuokra ajassa pian.

## <a name="known-issues-with-swapping-sites"></a>Sivuston vaihtamisen tunnetut ongelmat
- Kohdesivusto voi palauttaa lyhyen ajan "not found" (HTTP 404)-virheen.
- Sisältö on määritettävä uudelleen, jotta haku indeksiä voi päivittää. Tässä ei tarvita manuaalista vaihetta, tämä tapahtuu automaattisesti.
- Kaikki staattisista linkeistä riippuvat (kuten tiedostojen synkronointi ja OneNote-tiedostot) on korjattava manuaalisesti.
- Project Server-sivustot on ehkä vahvistettava sen varmistamiseksi, että ne liitetään edelleen oikein. 
