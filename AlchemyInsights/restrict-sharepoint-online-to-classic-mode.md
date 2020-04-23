---
title: SharePoint Onlinen rajoittaminen perinteiseen tilaan
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742466"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>SharePoint Onlinen rajoittaminen perinteiseen tilaan

Jotkin organisaatiot tarvitsevat edelleen Classic-tilan. Vaikka ei ole suunnitelmia poistaa perinteistä tilaa rakeisen tasolla, koko organisaatiota (vuokraajaa) ei voi enää rajoittaa perinteiseen tilaan luetteloita ja kirjastoja varten.

Admin on seuraavat vaihtoehdot hallita yksittäisiä luetteloita ja kirjastoja klassisessa tilassa käyttämällä rakeinen opt-out kytkimet, että tarjoamme seuraavilla tasoilla:

- sivuston kokoelma
- Sivuston
- Luettelo
- Kirjasto

Lisäksi luettelot, jotka käyttävät tiettyjä ominaisuuksia ja mukautuksia, joita moderni ei tue, siirtyvät edelleen automaattisesti perinteiseen tilaan.

1.4.2019 alkaen prosessi, jossa vuokraajan taso poistetaan käytöstä, ja kirjastot alkavat ja jatkuvat 31.5.2019 asti.  Luettelot ja kirjastot, jotka ovat perinteisessä tilassa vuokraajan kieltäytymisen seurauksena, siirretään automaattisesti moderniin.

Jos tarvitset klassista tilaa, katso lisätietoja [täältä](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ja PnP Powershell [-ohje,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) joka kuvaa vaihtoehtoja ja työkaluja, joita voit käyttää tänään perinteisen tilan käyttökokemuksen käyttämiseen.
