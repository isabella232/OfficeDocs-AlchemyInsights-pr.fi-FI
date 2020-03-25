---
title: SharePointin siirron rajoittaminen 503-virheillä
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931655"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a>SharePointin siirron rajoittaminen 503-virheillä

**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan. Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut. Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.

Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan. Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina. Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.

**503 virheitä siirryttäessä SharePoint Onlineen**

Näyttää siltä, että olet siirtymässä SharePoint Onlineen ja saat 503-virheitä. Noudata alla olevia ohjeita, jotta voimme auttaa sinua mahdollisimman pian. 

1. Valitse **Ota yhteyttä tukeen**ja sitten Uusi **palvelupyyntö**.
2. Kirjoita otsikkoa ja kuvausta varten **SharePoint Migration Throttling with 503**.
3. Kun lippu on lähetetty, päivitä se seuraavilla tiedoilla:
    - Kuinka paljon muuttoa on jäljellä (esimerkiksi kuinka monta pbs?).
    - Siirron alkamis- ja päättymispäivä.
    - Kuvaile, mistä siirrät sisältöä, kuten SharePoint Serveristä, Boxista, GDrivesta, jaetuista tiedostorekiveistä jne..
    - Arvioi rajoitusvirheiden määrä (esimerkiksi x kaasuviputinti tunnissa?) ja milloin rajoitus tapahtui.
    - Käyttämäsi siirtotyökalu (esimerkiksi SPMT tai ShareGate).


