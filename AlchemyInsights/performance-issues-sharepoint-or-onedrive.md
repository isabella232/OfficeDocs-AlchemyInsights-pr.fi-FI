---
title: Suorituskyky ongelmat-SharePoint tai OneDrive
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
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771898"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePointin tai OneDriven hidas, saavuttamattomissa tai poissa käytöstä useille käyttäjille

SharePoint tai OneDrive voi olla hidas, käyttökelvoton tai ei käytettävissä tai se voi näyttää palvelua ei ole käytettävissä tai 503-virheitä useista syistä:
  
- Jos SharePoint-tai OneDrive-sivustosi on hidas tai viivästynyt useille käyttäjille, kyseessä saattaa olla väliaikainen palvelu ongelma, jossa käyttäjät saavat ajoittaisia viiveitä tai siirtymis virheitä SharePoint-sivustoja tai OneDrive-sisältöä käytettäessä. Tarkista [palvelun kunnon koonti näytöstä](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , onko organisaatiosi vaikuttanut siihen.
  
- Käyttäjät voivat saada *503-palvelin on varattu* -virhe, kun yrität siirtyä SharePoint-tai OneDrive-sivustoihin. Tämä virhe voi johtua siitä, että SharePoint-palvelussa käytetään rajoitusta. SharePoint Online käyttää rajoittamista SharePoint Online -palvelun optimaalisen suorituskyvyn ja luotettavuuden ylläpitämiseen. Rajoittaminen rajoittaa käyttäjien toimien tai samanaikaisten kutsujen määrää (komentosarjojen tai koodin avulla), jotta resurssien liikakäyttö estetään. Lisä tietoja rajoittimen käyttämisestä on Ohje aiheessa [SharePoint Onlinessa ei saa estää tai estää niiden käytön estämistä](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Jos suoritus kyky on hidas **perinteisen** tai **modernin** SharePoint-sivuston tai-sivun avulla, analysoi sivut käyttämällä [sivun diagnostiikka-työkalua](https://aka.ms/perftool) .
  
- Jos sinulla on edelleen yleinen hidas suoritus kyky, tutustu tämän artikkelin lopussa oleviin resursseihin: [SharePoint Onlinen suoritus kyvyn](https://go.microsoft.com/fwlink/?linkid=2024334) parantaminen
  