---
title: Perinteisen pääsivuston vaihtaminen nykyaikaisella sivustolla
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940816"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Perinteisen pääsivuston vaihtaminen nykyaikaisella sivustolla

Jos ympäristö on määritetty ennen huhtikuuta 2019, voit muuttaa pääsivuston nykyaikaiseksi sivustoksi Microsoft PowerShellin avulla:

- Jos haluat käyttää pääsivustona toista sivustoa, voit korvata [pääsivuston (vaihtaa) sen](https://docs.microsoft.com/sharepoint/modern-root-site) tilalle. 
    - [Invoke-SPOSiteSwap-toiminnon](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) avulla voit vaihtaa sivuston sijainnin toiseen sivustoon samalla, kun arkistoit alkuperäistä sivustoa. Käytettävissä sekä ryhmäsivustolle (ei ole yhteydessä ryhmään) että viestintäsivustolle. 

- Lisäominaisuudet otetaan käyttöön pian, jotta voit jatkaa sivuston sisällön käytön, mutta muuntaa nykyisen sivuston viestintäsivustoksi. 
>[!Important]
>Nämä ominaisuudet tulevat käyttöön vaiheittain. Jatka päivitysten tarkistamista viestikeskuksesta. 

## <a name="known-issues-with-swapping-sites"></a>Tunnetut ongelmat sivustojen vaihtamisessa

- Kohdesivusto saattaa palauttaa "ei löydy" (HTTP 404) -virheen lyhyen aikaa.
- Sisältö on päivitettävä uudelleen, jotta hakuindeksi voidaan päivittää. Manuaalista vaihetta ei tarvita – tämä tehdään automaattisesti.
- Kaikki, mikä riippuu staattisista linkeistä (kuten tiedostojen synkronoinnista ja OneNote-tiedostoista), on korjattava manuaalisesti.
- Jos lähdesivusto oli organisaation uutissivusto, päivitä URL-osoite. Hanki luettelo kaikista organisaation uutissivustoista.
- Project Palvelinsivustot on ehkä vahvistettava, jotta ne voidaan liittää oikein.
