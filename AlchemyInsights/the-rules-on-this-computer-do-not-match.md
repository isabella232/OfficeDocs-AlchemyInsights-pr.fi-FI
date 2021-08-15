---
title: 'Virhe: Tämän tietokoneen säännöt eivät vastaa toisiaan'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981110"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Virhe: Tämän tietokoneen säännöt eivät vastaa toisiaan

Jos haluat nähdä tämän tunnetun ongelman päivitetyn tilan, katso tämän tietokoneen säännöt eivät vastaa [Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Työryhmä Outlook on tehnyt korjauksen koontiversiossa 12928.10000. Korjaus on jo Insider-kanavan nopeassa käytössä, ja se tulee kuukausittaiseen kanavaan kesäkuun 2020 lopulla. Kun sinulla on korjattu koontiversio, saatat saada vielä kerran kehotteen "Mitkä säännöt haluat säilyttää". Valitse pyydettäessä Palvelin, palaa sitten Outlook ja ota uudelleen käyttöön kaikki käytöstä poistetut säännöt.

Käytä seuraavaa vaihtoehtoista tapaa, kunnes korjaus on saatavilla:

**Vaihtoehtoinen menetelmä:** Viimeaikaisissa raporteissa ongelma on ilmennyt niillä raporteissa, jotka ovat vain luoneet asiakassääntöjä Outlook työpöytäversiossa. Jos ongelma jatkuu, harkitse sääntöjen poistamista ja luo ja muokkaa sitten sääntöjä vain OWA:ssa (Outlook Web App), kunnes ongelma on ratkaistu.

Jos et voi poistaa sääntöjä manuaalisesti, voit suorittaa Outlook-komennon, kun käynnistät Outlook /cleanrulesOutlook.exe komennon. Tämä poistaa sekä asiakkaan että palvelimen säännöt. Se poistaa kaikki profiilin kaikkien tilien säännöt Outlook. Tämä komento on edelleen dokumentoitu Komentorivivalitsimet-artikkelissa.

