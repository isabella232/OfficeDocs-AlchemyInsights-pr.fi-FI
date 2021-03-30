---
title: EndPoint Manager – suojauksen perusaikataulut
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420878"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – suojauksen perusaikataulut

Suojauksen perusaikataulut ovat valmiiksi määritettyjä Windows-asetusryhmiä, joiden avulla voit ottaa käyttöön asianomaisten suojausryhmien suosittelemia suojausasetuksia. Näitä perusaikatauluja voidaan mukauttaa toimittamaan vain halutut asetukset ja arvot. Lisätietoja suojauksen perusaikatauluista on ohjeaiheessa Windows 10 -laitteiden määrittäminen [Intunessa suojauksen perusaikataulujen avulla.](https://docs.microsoft.com/mem/intune/protect/security-baselines)

Näiden tuotteiden perusaikatauluja on tällä hetkellä:

- Windowsin MDM-suojausasetukset
- Microsoft Defender for EndPoint Security
- Microsoft Edge

Kukin perusaikataulu päivitetään säännöllisesti ja julkaistaan asteittain. Kukin versio lisää ja poistaa edellisestä versiosta asetukset sen varmistamiseksi, että perusaikataulu vastaa nykyisiä ohjeita. Päätepisteen suojauksen perussolsoleiden avulla eri versioita voidaan verrata tekemällä muutokset versiosta versioon näkyvissä.

Ohjeita perusaikataulun käyttöönottoversion tehokkaimpaan muutokseen on Kohdassa Suojauksen perusaikataulun profiilien hallinta [Microsoft Intunessa.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

Kun olet ottanut suojauksen perusaikataulun käyttöön, voit valvoa käyttöönoton tila ja tarkistaa asetukset laitekohtaisesti.

**Huomautus:** Perusaikataulujen raportointitiedot voivat näkyä 24 tunnin kuluessa käyttöönotosta laitteeseen ja enintään 6 tuntia lisäpäivityksiä varten. 

Perusaikataulun asetuksen ei yleensä tarvitse olla käytössä, koska samaa asetusta käytetään eri profiilissa. Voit tutkia tätä skenaariota tietyssä laitteessa valitsemalla laitteen Security Baseline -profiilin Laitteen tila -solmussa. Lisätietoja on kohdassa [Suojauksen perusaikataulujen ristiriitojen ratkaiseminen.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)