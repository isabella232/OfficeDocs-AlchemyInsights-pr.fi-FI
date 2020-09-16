---
title: SharePoint Onlinen rajoittaminen perinteiseen tilaan
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751419"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>SharePoint Onlinen rajoittaminen perinteiseen tilaan

Jotkin organisaatiot vaativat edelleen perinteisen tilan käyttö kokemusta. Vaikka perinteistä tilaa ei ole tarkoitus poistaa rakeisella tasolla, koko organisaatiota (vuokraaja) ei voi enää rajoittaa luetteloiden ja kirjastojen perinteiseen tilaan.

Järjestelmänvalvojalla on seuraavat asetukset, joilla hallitaan yksittäisiä luetteloita ja kirjastoja perinteisessä tilassa käyttämällä rakeisia kieltäytymis valitsimia, jotka tarjoamme seuraavilla tasoilla:

- sivustokokoelma
- sivuston
- luettelo
- kirjaston

Lisäksi luettelot, jotka käyttävät tiettyjä ominaisuuksia ja mukautuksia, joita moderni ei tue, kytketään automaattisesti perinteiseen tilaan.

1. huhtikuuta 2019 lähtien prosessi, joka poistaa vuokra ajan tason jättäytymisen pois modernista luettelosta ja kirjastot alkavat ja jatkuvat 31. toukokuuta 2019.  Luettelot ja kirjastot, jotka ovat perinteisessä tilassa vuokra ajan käytöstä poisjäämisen seura uksena, siirtyvät automaattisesti moderniin.

Jos tarvitset perinteistä tilaa, Katso lisä tietoja [täältä](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ja PnP-PowerShell [-Ohje,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) jossa kerrotaan vaihto ehdoista ja työkaluista, joilla voit käyttää perinteistä tila kokemusta.
