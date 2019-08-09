---
title: Vaihda Classic pääkansio sivuston Moderni sivusto
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
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270741"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Vaihda Classic pääkansio sivuston Moderni sivusto

Jos ympäristösi on määritetty ennen huhtikuuta 2019, voit muuttaa päätason sivustossa Moderni sivustoon käyttämällä Microsoft PowerShell:

- Jos sinulla on toinen sivusto, jota haluat käyttää oman pääsivusto, jonka korvaava (swap) pääkansio sivuston. 
    - [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) avulla sivuston toisen sivuston kanssa vaihdettava tallennettaessa alkuperäiseen sivustoon. Sekä ryhmän (ei yhteyttä ryhmään) ja tiedonannon sivustojen käytettävissä. 

- Lisäominaisuuksia se esitellään pian, joka mahdollistaa sivuston sisällön avulla pitää, mutta sivusto muuntaminen Viestimissivusto. 
>[!Important]
>Näitä toimintoja toteutetaan vielä vähitellen. Tarkista päivitykset Office 365 Message Center jatkaa. 

## <a name="known-issues-with-swapping-sites"></a>Tunnettuja ongelmia vaihtamisen sivustot

- Kohdesivuston saattaa palauttaa (HTTP 404) ”ei löydy” virhe lyhyen ajan kuluessa.
- Sisältöä täytyy päivittää hakuindeksin tehdään uudelleen. On manuaalinen vaihe, ei pakollinen – tämä tehdään automaattisesti.
- Mitään riippuvainen ”staattinen” linkkejä (kuten tiedoston synkronointiin ja OneNote-tiedostoja) on korjattava manuaalisesti.
- Jos lähde on organisaation uutissivuston, Päivitä URL-osoite.Näyttöön tulee luettelo sivustoja organisaatiota koskevia uutisia.
- Project Server-sivustoja on ehkä tarkistettava sen varmistamiseksi, että ne liittyvät yhä oikein.





