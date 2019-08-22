---
title: IP-osoite ja seurantalokeja asiakkaan tunnistaminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539026"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-osoite ja seurantalokeja asiakkaan tunnistaminen

Seurantalokit näkyy IP-osoite, joka vastaa tehtävän Office 365-käyttäjä tai järjestelmänvalvoja. Asiakkaan tiedot kirjataan. Seuraavassa on ohjeita tällaisen tunnistetietoja

1. Kirjautua sisään [Office 365 & noudattamista Tietoturvakeskus](https://protection.office.com/).

2. Siirry **Etsinnän** > **Audit log** etsintäsivun.

   Jos olet kiinnostunut tietyn tehtävän, valitse **tehtävät** luettelosta. Jos näin ei ole, palautetaan kaikki valitun käyttäjän (oletusasetus).

   **Huomautus**: tietyt toimet eivät ole käytettävissä **toimintojen** valikon. kuitenkin ne valvottavat kohteet palautetaan Jos **Näytä tulokset kaikista** on valittuna (oletusasetus).

3. Määritä käyttäjänimi **käyttäjät** -kentässä ja valitse aktiviteetin päivämäärävälin **haku**.

Tulokset näet IP-osoitteen, että toiminnan tulokset-ruudussa. Valitse asiakkuustietueen yksityiskohtaisia lisätietoja **tiedot** valikon avauspainike (esimerkiksi asiakas, käyttäjä, joka suorittaa toiminnon, jne.).

Lisätietoja [tartunnan saaneen tili käyttää tietokoneen IP-osoitteen löytäminen](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
