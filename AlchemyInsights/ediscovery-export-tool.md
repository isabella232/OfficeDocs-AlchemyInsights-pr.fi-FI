---
title: eDiscovery-vientityökalu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101299"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Eikö eDiscovery-vientityökalua voi asentaa tai suorittaa?

Jos et voi asentaa tai suorittaa eDiscovery-vientityökalua hakutulosten lataamiseksi, tarkista seuraavat asiat:
  
- Käytössäsi on tietokone, joka täyttää seuraavat vaatimukset:

  - 32- tai 64-bittinen versio Windows 7 tai uudempi versio

  - Microsoft .NET Framework 4.7

  - Tuettu selain:

  - Microsoft Edge

    TAI

  - Internet Explorer 10 ja uudemmat versiot

    Muita selaimia, kuten Google Chromea ja Mozilla Firefoxia, ei tueta.

- Organisaatiosi voi muodostaa yhteyden Azuren päätepisteeseen, joka on **\* .blob.core.windows.net** (yleismerkki edustaa vientityön yksilöllistä tunnistetta).

- Sinulle määritetään vientirooli tietoturva Microsoft 365 &amp; yhteensopivuuskeskuksessa. Tämä rooli määritetään oletusarvoisesti vain eDiscovery Manager -rooliryhmään. Katso [eDiscovery-oikeuksien määrittäminen.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Lisätietoja on kohdassa [Sisältöhaun tulosten vieminen.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Jos viet yli 100 000 000 postilaatikkoa, sinun on ladattava vientitulokset seuraavan PowerShellin avulla: Tulosten vieminen yli [100 000 000 postilaatikosta.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)