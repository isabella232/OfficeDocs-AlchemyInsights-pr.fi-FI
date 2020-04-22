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
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741962"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePointin ja OneDriven valvontalokit

## <a name="sharepoint-classic-audit-logs"></a>SharePointin perinteiset valvontalokit

SPO:n vanha valvonta siirrettiin Yhdistettyyn valvontalokiin (UAL). Kaikki spo:n vanhat auditointiraportit toimitetaan nyt UAL:n kautta ja vanhat auditointisignaalit on siirretty UAL:hen.

Tärkeimmät muutokset:

* Trimmaus ei ole käytettävissä ominaisuutena.
* Tiettyjen valvottavien tapahtumien valitseminen ei ole käytettävissä. Tässä [asiakirjassa](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) on täydellinen luettelo oletusarvoisesti käytettävissä olevista valvotuista tapahtumista.
* **Mukautetut raportit** -kohdan **Sijainti-vaihtoehto** ei ole käytettävissä.
* **Asiakirjojen avaaminen tai lataaminen** -vaihtoehto ei ole käytettävissä.

[Sivustokokoelman valvonta-asetusten määrittäminen](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePointin ja OneDriven nykyaikaiset yhdistetyt valvontalokit yhteensopivuudesta

* [Yhdistetyn valvonnan kirjaamisen ottaminen käyttöön tai poistaminen käytöstä](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Lisämäärityksiä ei tarvita SharePointissa tai OneDrivessa.

Tarkista tiedostojen, kansioiden, käyttäjien ja käyttöoikeuksien toiminta valvontalokihaun avulla:

* [Tiedostojen ja sivujen aktiviteetit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Kansion toiminnot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Jakamis- ja käyttöoikeuspyyntöaktiviteetit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkronointiaktiviteetit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Sivuston hallintatoiminnot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Lisätietoja näiden tapahtumien noutamisesta on kohdassa [Haku valvontalokista](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
