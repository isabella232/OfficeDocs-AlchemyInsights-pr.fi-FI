---
title: eDiscoveryn vienti työkalu
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277939"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Etkö voi asentaa tai suorittaa eDiscoveryn vienti työkalua?

Jos et voi asentaa tai käyttää eDiscoveryn vienti työkalua haku tulosten lataamiseen, tarkista seuraavat asiat:
  
- Käyttämäsi tieto kone täyttää seuraavat vaatimukset:

  - 32-tai 64-bittiset Windows 7-versiot ja uudemmat versiot

  - Microsoft .NET Framework 4.7

  - Tuetulla selaimella:

  - Microsoft Edge

    TAI

  - Internet Explorer 10 ja uudemmat versiot

    Muita selaimia, kuten Google Chromea ja Mozilla Firefoxia, ei voi tukea.

- Organisaatiosi voi muodostaa yhteyden Azure-pääte pisteeseen, joka on ** \* . blob.Core.Windows.net** (Yleismerkki vastaa vienti työn yksilöllistä tunnistetta).

- Olet määrittänyt vienti roolin Microsoft 365-tieto turva &amp; yhteensopivuus keskuksessa. Oletusarvoisesti tämä rooli määritetään vain eDiscoveryn hallinta-rooli ryhmälle. Lisä tietoja on Ohje aiheessa [eDiscoveryn käyttö oikeuksien määrittäminen](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Lisä tietoja on Ohje aiheessa [sisältö haun tulosten vieminen](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Jos viet yli 100 000 posti laatikkoa, sinun on ladattava vienti tulokset seuraavan PowerShellin avulla: vie  [tulokset yli 100k posti laatikosta](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).