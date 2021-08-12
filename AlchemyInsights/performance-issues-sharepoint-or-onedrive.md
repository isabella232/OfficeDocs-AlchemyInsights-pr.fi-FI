---
title: Suorituskykyongelmat SharePoint tai OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911839"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint tai OneDrive, ei voi käyttää tai olla useiden käyttäjien käytettävissä

SharePoint tai OneDrive voi olla hidas, ei käytettävissä tai poissa käytöstä, tai palvelu ei ehkä ole käytettävissä tai 503 virhettä useista syistä:
  
- Jos SharePoint tai OneDrive-sivusto on hidas tai sitä viivytetty useille käyttäjille, voi olla olemassa tilapäinen palveluongelma, jossa käyttäjillä ilmenee ajoittain viiveitä tai siirtymisvirheitä, kun he SharePoint sivustoja tai OneDrive sisältöä. Tarkista Palvelun [kunto -koontinäytöstä,](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) vaikuttaako se organisaatioosi.
  
- Käyttäjät saattavat saada *503-palvelimen on varattu* -virheilmoituksen, kun he yrittävät siirtyä SharePoint tai OneDrive sivustoihin. Tämä virhe voi johtua palvelun SharePoint. SharePoint Online käyttää rajoittamista SharePoint Online -palvelun optimaalisen suorituskyvyn ja luotettavuuden ylläpitämiseen. Rajoittaminen rajoittaa käyttäjien toimien tai samanaikaisten kutsujen määrää (komentosarjojen tai koodin avulla), jotta resurssien liikakäyttö estetään. Lisätietoja estosta on kohdassa Estäminen tai estäminen [SharePoint Onlinessa.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Jos käytät hidasta suorituskykyä perinteisessä **tai** nykyaikaisessa **SharePoint** sivustossa [](https://aka.ms/perftool) tai sivulla, analysoi sivut Sivun vianmääritys -työkalulla.
  
- Jos suorituskyky on yleisesti hidas, tutustu resursseihin tämän artikkelin alareunassa: Johdanto SharePoint [Onlinen suorituskyvyn parantamiseen](https://go.microsoft.com/fwlink/?linkid=2024334)
  