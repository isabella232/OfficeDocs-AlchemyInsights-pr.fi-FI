---
title: Perinteisen pääsivuston vaihtaminen modernilla sivustolla
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691176"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Perinteisen pääsivuston vaihtaminen modernilla sivustolla

Jos ympäristösi on määritetty ennen huhtikuun 2019, voit vaihtaa pääsivuston moderniin sivustoon Microsoft PowerShellin avulla:

- Jos sinulla on jokin muu sivusto, jota haluat käyttää pääsivustona, voit vaihtaa [pääsivustoa](https://docs.microsoft.com/sharepoint/modern-root-site) sen kanssa. 
    - Käytä [Invoke-SPOSiteSwap-](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) vaihto pistettä, jos haluat vaihtaa sivuston sijainnin toiseen sivustoon arkistoitaessa alkuperäistä sivustoa. Saatavilla sekä Ryhmäsivustolle (ei yhdistetty ryhmään) että Viestintäsivustoon. 

- Saat pian käyttöön lisä ominaisuuksia, joiden avulla voit jatkaa sivuston sisällön käyttöä, mutta muuntaa aiemmin luodun sivuston viestintä sivustoksi. 
>[!Important]
>Nämä ominaisuudet otetaan käyttöön asteittain. Jatka Tarkista viesti keskus päivitysten varalta. 

## <a name="known-issues-with-swapping-sites"></a>Sivuston vaihtamisen tunnetut ongelmat

- Kohdesivusto voi palauttaa lyhyen ajan "not found" (HTTP 404)-virheen.
- Sisältö on määritettävä uudelleen, jotta haku indeksiä voi päivittää. Manuaalista vaihetta ei tarvita-tämä tapahtuu automaattisesti.
- Kaikki staattisista linkeistä riippuvat (kuten tiedostojen synkronointi ja OneNote-tiedostot) on korjattava manuaalisesti.
- Jos lähdesivusto oli organisaation uutissivusto, Päivitä URL-osoite.Saat luettelon kaikista organisaation uutis sivuista.
- Project Server-sivustot on ehkä vahvistettava sen varmistamiseksi, että ne liitetään edelleen oikein.
