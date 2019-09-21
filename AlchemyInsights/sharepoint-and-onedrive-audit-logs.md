---
title: Perinteisen SharePointin valvonta lokin raportit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068020"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePointin ja OneDriven valvonta lokit

**SharePointin ja OneDriven modernit yhtenäiset valvonta lokit vaatimustenmukaisuudesta**

- [Yhtenäisen valvonta lokin ottaminen käyttöön ja poistaminen käytöstä](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

SharePointin tai OneDriven sisällä ei tarvita lisä määrityksiä.

- Käytä valvonnan kirjaamis hakua tiedostojen, kansioiden, käyttäjien ja käyttö oikeuksien tarkistustyö:

    - [Tiedostojen ja sivujen toiminnot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Kansion aktiviteetit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Jakamis-ja käyttö oikeus pyyntöjen toiminnot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Synkronointi toiminnot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Sivuston hallinta toiminnot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Lisä tietoja näiden tapahtumien hakemista on kohdassa [valvonta lokin](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)hakeminen.

**SharePoint Classicin valvonta lokit**

Siirsimme SPO Legacy Audit-valvonnan yhtenäiseen valvonta lokiin (UAL). Tämä tarkoittaa lähinnä sitä, että kaikki SPO Legacy-auditointi raportit ovat nyt powered by UAL, ja vanhoja valvonta signaaleja on siirretty UAL.

Keskeiset muutokset:

- Ominaisuuksien rajaaminen ei ole mahdollista.
- Osa, jossa valitset tiettyjä valvonta tapahtumia, ei ole käytettävissä. Katso [tästä asia kirjasta](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) täydellinen luettelo tarkastetuista tapahtumista, jotka ovat oletusarvoisesti käytettävissä.
- **Mukautetut raportit** -kohdan sijainti-vaihto ehto ei ole käytettävissä. 
- "Asia kirjojen avaaminen tai lataaminen"-tapahtumat eivät ole käytettävissä. 

