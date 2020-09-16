---
title: Sähkö posti profiilien käyttäminen Intunella
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653285"
---
# <a name="using-email-profiles-with-intune"></a>Sähkö posti profiilien käyttäminen Intunella

Intunella voi luoda ja ottaa käyttöön Sähkö posti profiileja, jotka koskevat alkuperäistä (sisäänrakennettua) sähkö posti ohjelmaa useilla laite alustoilla.

Lisä tietoja Sähkö posti profiileihin liittyvistä rajoituksista, kuten olemassa olevien profiilien käytöstä ja Sähkö posti profiilien poistamisesta, on Ohje aiheessa [Sähkö posti asetusten lisääminen laitteisiin Intune-toiminnon avulla](https://docs.microsoft.com/intune/email-settings-configure).

Lisä tietoja Sähkö posti profiilien luomisesta kullekin laite alustalle on kohdassa:

[Android-laitteen asetukset sähkö postin, todennuksen ja synkronoinnin määrittämiseen Intunella](https://docs.microsoft.com/intune/email-settings-android)  
[Sähkö posti asetusten lisääminen iOS-ja iPadOS-laitteille Microsoft Intunella](https://docs.microsoft.com/intune/email-settings-ios)  
[Sähkö posti profiilin asetukset Microsoft Intunella Windows Phone 8,1-laitteita varten](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Windows 10: n laitteiden Sähkö posti profiilin asetukset Microsoft Intunella](https://docs.microsoft.com/intune/email-settings-windows-10)

**Yleinen synkronointi ongelma**

**Android-Sähkö posti profiilissa oleva KNOX estää käyttäjä kontakteja, kalenteria ja tehtäviä synkronoimasta käyttäjän laitteisiin.**

Android-KNOX-Sähkö posti profiilissa oleva KNOX tarjoaa järjestelmänvalvojalle mahdollisuuden määrittää, mitkä sisältö tyypit synkronoidaan laitteeseen, määrittämällä kukin käyttöön.

Jos minkä tahansa sisältö tyypin asetusta **ei ole määritetty** (oletus arvo), kyseistä sisältö tyyppiä ei synkronoida automaattisesti. Käyttäjä voi ottaa käyttöön sisältö tyypin, jonka he haluavat suoraan laitteeseen manuaalisesti, mutta tämä kokoonpano korvataan Intune-asetuksella ja sisältö tyypin synkronointi pysähtyy.

