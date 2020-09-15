---
title: Perinteiset SharePoint-valvonta loki raportit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662205"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePointin ja OneDriven valvonta lokit

## <a name="sharepoint-classic-audit-logs"></a>SharePointin perinteiset valvonta lokit

SPO-vanha valvonta on siirretty yhdistettyyn valvonta lokiin (UAL). Kaikki SPO:N aiemmat valvonta raportit käynnistetään nyt UAL-tilassa, ja vanhat valvonta signaalit on siirretty UAL-kohteeseen.

Keskeiset muutokset:

* Rajaus ei ole käytettävissä valmiutensa mukaan.
* Tiettyjen tapahtumien valitseminen tarkastusta varten ei ole käytettävissä. Katso [tästä asia kirjasta](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) täydellinen luettelo tarkastetuista tapahtumista, jotka ovat käytettävissä oletusarvoisesti.
* **Mukautetut raportit** -kohdan **Sijainti** -vaihto ehto ei ole käytettävissä.
* **Tiedostojen avaaminen tai lataaminen** -tapahtumat-vaihto ehto ei ole käytettävissä.

[Sivustokokoelman valvonta-asetusten määrittäminen](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePointin ja OneDriven nykyaikaiset yhtenäiset valvonta lokit vaatimustenmukaisuudesta

* [Yhdistetyn valvonta kirjauksen ottaminen käyttöön/poistaminen käytöstä](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

SharePointin tai OneDriven sisällä ei tarvita lisä määrityksiä.

Valvonta loki haun avulla voit tarkistaa, onko tiedosto (a), kansio tai käyttäjä, käyttö oikeudet:

* [Tiedostojen ja sivujen toiminnot](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Kansio toiminnot](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Jakamis-ja yhteys pyyntö aktiviteetit](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkronointi toiminnot](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Sivuston hallinta toiminnot](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Lisä tietoja näiden tapahtumien hakemisesta on kohdassa [valvonta lokista hakeminen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
