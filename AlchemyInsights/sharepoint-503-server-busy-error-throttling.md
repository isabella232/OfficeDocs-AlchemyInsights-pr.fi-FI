---
title: SharePoint Onlinen rajoitus
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931223"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Onlinen rajoitus

**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan. Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut. Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.

Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan. Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina. Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.

**503 palvelin on varattu virhe**

Käyttäjät saattavat saada 503-palvelimen olevan varattu virhe yritettäessä siirtyä SharePoint- tai OneDrive-sivustoihin. 

Tämä virhe voi johtua sharepoint-palvelun kuristamisesta. SharePoint Online käyttää rajoitusta SharePoint Online -palvelun optimaalisen suorituskyvyn ja luotettavuuden ylläpitämiseen. Kuristus rajoittaa käyttäjän toimintojen tai samanaikaisten kutsujen määrää (komentosarjan tai koodin mukaan) resurssien liikakäytön estämiseksi. 

Lisätietoja kuristamisesta on [ohjeaiheessa Vältä kuristamisen tai estymisen estäminen SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Jos uskot, että tämä virhe ei liity kuristukseen, voit tarkistaa, onko vuokraajassa aktiivista ylläpitoa, siirtymällä [Viestikeskukseen](https://portal.office.com/adminportal/home#/MessageCenter).

 Varmista lopuksi, että käyt [Palvelun kunto -sivulla](https://portal.office.com/adminportal/home#/servicehealth) ja tarkistat mahdolliset tiedotteet/tapahtumat.

