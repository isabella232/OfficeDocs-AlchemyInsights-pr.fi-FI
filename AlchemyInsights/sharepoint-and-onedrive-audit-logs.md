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
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992615"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePointin ja OneDriven valvonta lokit

## <a name="sharepoint-classic-audit-logs"></a>SharePoint Classicin valvonta lokit

SPO Legacy-valvonta siirrettiin yhtenäiseen valvonta lokiin (UAL). Kaikki SPO Legacy-auditointi raportit toimivat nyt UAL-järjestelmän kautta, ja aiemmat auditointi signaalit on siirretty UAL-järjestelmään.

Keskeiset muutokset:

* Trimmaus ei ole käytettävissä ominaisuus.
* Tiettyjen tapahtumien valitseminen valvomatta ei ole käytettävissä. Katso [tästä asia kirjasta](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) täydellinen luettelo tarkastetuista tapahtumista, jotka ovat oletusarvoisesti käytettävissä.
* **Mukautettujen raporttien** **Sijainti** vaihtoehto ei ole käytettävissä.
* **Avaus-tai lataus asiakirjojen** tapahtumat-vaihto ehto ei ole käytettävissä.

[Sivustokokoelman valvonta-asetusten määrittäminen](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePointin ja OneDriven modernit yhtenäiset valvonta lokit vaatimustenmukaisuudesta

* [Yhtenäisen valvonta lokin ottaminen käyttöön ja poistaminen käytöstä](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

SharePointin tai OneDriven sisällä ei tarvita lisä määrityksiä.

Käytä valvonnan kirjaamis hakua tiedostojen, kansioiden, käyttäjien ja käyttö oikeuksien tarkistustyö:

* [Tiedostojen ja sivujen toiminnot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Kansion aktiviteetit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Jakamis-ja käyttö oikeus pyyntöjen toiminnot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkronointi toiminnot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Sivuston hallinta toiminnot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Lisä tietoja näiden tapahtumien hakemista on kohdassa [valvonta lokin](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)hakeminen.
