---
title: EndPointin hallinta – Suojauksen perustasot
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
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923551"
---
# <a name="endpoint-manager---security-baselines"></a>EndPointin hallinta – Suojauksen perustasot

Suojauksen perustasot ovat valmiiksi määritettyjä Windows-asetusryhmiä, joiden avulla voit ottaa käyttöön niitä suojausasetuksia, joita asianomaiset suojausryhmät suosittelevat. Näitä perustasoja voidaan mukauttaa toimittamaan vain halutut asetukset ja arvot. Lisätietoja suojauksen perustasoista on ohjeaiheessa [Windows 10 -laitteiden määrittäminen Intunessa](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Perustasoja on tällä hetkellä näissä tuotteissa:

- Windows mobiililaitteidenhallinen suojausasetukset
- Microsoft Defender for EndPoint Security
- Microsoft Edge

Jokainen perustaso päivitetään säännöllisesti ja julkaistaan asteittaisina versioina. Jokainen versio lisää ja poistaa edellisestä versiosta asetuksia sen varmistamiseksi, että perustaso täyttää nykyiset ohjeet. Päätepisteen suojauksen perustason konsoli sallii eri versioiden vertailun tekemällä muutokset versiosta versioon näkyviksi.

Ohjeita siitä, miten voit tehokkaasti muuttaa sitä, mikä perustason versio on käytössä, on kohdassa [Suojauksen perustason profiilien hallinta Microsoft Intunessa](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Kun olet ottanut suojauksen perustasokäyttöön, voit valvoa käyttöönoton tilaa ja tarkastella asetuksia laitekohtaisesti.

Koska suojauksen perusaikatauluissa on useita asetuksia, on tärkeää tarkistaa määritysmuutokset ja testata, että kaikki asetukset sopivat laitteisiisi ja liiketoimintatarpeisiisi.

**Huomautus:** Perustasojen raportointitietojen tuleminen näkyviin ensimmäisen käyttöönoton jälkeen laitteeseen voi kestää jopa 24 tuntia ja lisäpäivityksiä varten enintään 6 tuntia. 

Yleisin syy perustason määrittämisen epäonnistumiseen on, että samaa asetusta käytetään eri profiilissa. Tämä skenaario voidaan tutkia tietyssä laitteessa valitsemalla tämä laite Suojauksen perustaso -profiilin Laitteen tila -solmusta. Lisätietoja on kohdassa [Suojauksen perustasojen ristiriitojen ratkaiseminen](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).