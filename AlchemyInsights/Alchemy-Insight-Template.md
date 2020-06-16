---
title: sama kuin tiedostonimi on paras
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750967"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Pakollinen Alchemy Header H1, H2: n eivät toimi."
Alchemyn luontia koskevat parhaat käytännöt ja ohjeet:

1. **Älä pesä Alchemy Oivalluksia kansioihin**- tämä rikkoo url-rakenne. Tutkimme tämän korjaamista.
1. **AlchemyInsights-kansion** tiedostoissa on oltava pienet tiedostonimet, joissa on välilyöntejä ex. ***miten-to-enable-riita-oikeus -pidä***.
    1. Sisällytä sääntötunnus tai säilötunnus [Alchemy Partner -portaalista](https://alchemyportal.azurewebsites.net) ms.custom-kenttään. Ex. ***ms.custom: 100021***
1. Käytä mallina muita tämän tiedoston yläosassa olevia metatietoja.
1. Siirry [Alchemy Partner -portaalissa](https://alchemyportal.azurewebsites.net) **asiakastietojen otsikko** -osioon ja käytä sitä H1-otsikon lähtökohtana. 
    > [!NOTE]
    > Alkemia Oivalluksia on oltava vain yksi H1 yläreunassa tai ne rikkovat tuotannossa. H2s ei hahmonnu, joten käytä **lihavointia** tai muita käytäntöjä eri osien merkitsemiseen.
1. Täytä seuraavaksi leipäteksti käyttämällä Alchemy-sääntö-sivun Asiakastiedot-osion luonnosmateriaalia.
    1. Luettelomerkeillä varustetut luettelot ovat kunnossa
    1. Myös numeroidut luettelot
    1. **Lihavoitu** ja *kursivoitu* ovat-ok
    1. Linkkien pitäisi aina olla joko **"linkkejä web"/ ulkoinen** TAI **syvä-linkkejä käyttöliittymän elementtejä,** ei sisäisiä linkkejä.
    1. Kuvia ei virallisesti tueta tällä hetkellä, mutta se on etenemissuunnitelmassa.

Ja tämä on todella jo hieman liian pitkä. Paras käytäntö on noin 400 merkkiä ---------------------------------

Kun sisältö on valmis, vedä se live-haaraan. Siirry sitten [Alchemy Partner -portaaliin](https://alchemyportal.azurewebsites.net) ja kirjoita tiedostonimi URL-kenttään. 