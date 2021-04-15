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
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782949"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Virhe: Tämän tietokoneen säännöt eivät vastaa toisiaan

Jos haluat nähdä tämän tunnetun ongelman päivitetyn tilan, katso tämän tietokoneen säännöt [eivät vastaa Microsoft Exchangen sääntöjä.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook-työryhmä on tehnyt korjauksen koontiversiossa 12928.10000. Korjaus on jo Insider-kanavan nopeassa käytössä, ja se tulee kuukausittaiseen kanavaan kesäkuun 2020 lopulla. Kun sinulla on korjattu koontiversio, saatat saada vielä kerran kehotteen "Mitkä säännöt haluat säilyttää". Valitse pyydettäessä Palvelin, palaa Sitten Outlookiin ja ota uudelleen käyttöön käytöstä poistetut säännöt.

Käytä seuraavaa vaihtoehtoista tapaa, kunnes korjaus on saatavilla:

**Vaihtoehtoinen menetelmä: Viimeaikaisissa** raporteissa ongelma on ilmennyt niillä raporteissa, jotka ovat vain luoneet asiakassääntöjä Outlookin työpöytäversiossa. Jos ongelma jatkuu, voit poistaa säännöt ja luoda ja muokata sääntöjä vain OWA:ssa (Outlook Web App), kunnes ongelma on ratkaistu.

Jos et voi poistaa sääntöjä manuaalisesti, voit suorittaa Outlook-komennon, kun käynnistät Outlookin suorittamalla komennon /cleanrulesOutlook.exe /cleanrules. Tämä poistaa sekä asiakkaan että palvelimen säännöt. Se poistaa kaikki säännöt kaikista Outlook-profiilin tileistä. Tämä komento on edelleen dokumentoitu Komentorivivalitsimet-artikkelissa.

