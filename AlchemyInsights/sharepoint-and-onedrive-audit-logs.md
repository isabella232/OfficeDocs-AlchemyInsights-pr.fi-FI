---
title: Perinteiset SharePoint-valvontalokiraportit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509597"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint- ja OneDrive-valvontalokit

## <a name="sharepoint-classic-audit-logs"></a>SharePointin perinteiset valvontalokit

SPO:n vanha valvonta siirrettiin yhtenäiseen valvontalokiin (UAL). Kaikki SPO:n vanhat auditointiraportit saavat nyt virtaa UAL:n kautta, ja vanhat valvontasignaalit on siirretty UAL-ilmoitukseen.

Keskeiset muutokset:

* Trimmaus ei ole käytettävissä lisävarusteena.
* Tiettyjen tarkettavissa olevien tapahtumien valitseminen ei ole käytettävissä. Tässä [asiakirjassa](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) on täydellinen luettelo oletusarvoisesti käytettävissä olevista valvotuista tapahtumista.
* **Mukautetut raportit -kohdan** **Sijainti-vaihtoehto** ei ole käytettävissä.
* **Asiakirjojen avaaminen tai lataaminen** -vaihtoehto ei ole käytettävissä.

[Sivustokokoelman valvonta-asetusten määrittäminen](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint- ja OneDrive Modern Unified Audit -lokit vaatimustenmukaisuudesta

* [Yhtenäisen valvonnan kirjaamisen ottaminen käyttöön tai poistaminen käytöstä](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Lisämäärityksiä ei tarvita SharePointissa tai OneDrivessa.

Valvontalokihaun avulla voit tarkistaa tiedostojen, kansioiden, käyttäjien ja käyttöoikeuksien aktiviteetit:

* [Tiedosto- ja sivutoiminnot](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Kansion aktiviteetit](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Pyyntöaktiviteettien jakaminen ja käyttäminen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkronointiaktiviteetit](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Sivuston hallintatoiminnot](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Lisätietoja näiden tapahtumien noutamisesta on kohdassa [Valvontalokista etsiminen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
