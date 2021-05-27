---
title: Defender endpointin tarkistustunnistimen tila
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676181"
---
# <a name="defender-endpoint-check-sensor-status"></a>Defender endpointin tarkistustunnistimen tila

Laitteet, **joissa on tunnistimen ongelmat** -ruutu, on Security Operations -koontinäytössä. Tässä ruudussa on tietoja siitä, miten yksittäinen laite voi tarjota tunnistimen tietoja ja viestiä Defender for Endpoint -palvelun kanssa. Se ilmoittaa, kuinka moneen laitteeseen on kiinnitettävä huomiota, auttaa tunnistamaan ongelmalaitteet ja korjaamaan tunnetut ongelmat.

Ruudussa on kaksi tilailmaisinta, jotka ilmoittavat siitä, kuinka monta laitetta ei ole ilmoittanut asianmukaisesti palvelulle:

- **Määritetty väärin** Laitteet, jotka saattavat raportoida tunnistimen tiedoista osittain Defender for Endpoint -palveluun ja joissa voi olla kokoonpanovirheitä, jotka on korjattava.
- **Passiivinen** Laitteet, jotka ovat lopenneet raportoinnin Defender for Endpoint -palveluun yli seitsemän päivän ajan viimeisen kuukauden aikana.

Kun napsautat mitä tahansa ryhmää, sinut ohjataan Laitteet-luetteloon valintojen mukaan suodatettuna. Laitteet-luettelossa voit suodattaa kuntotilaluettelon seuraavan tilan mukaan:

- **Aktiivinen** Laitteet, jotka raportoivat aktiivisesti Defender for Endpoint -palveluun.
- **Määritetty väärin** Laitteet, jotka saattavat raportoida tunnistimen tiedoista osittain Defender for Endpoint -palveluun, mutta joissa on kokoonpanovirheitä, jotka on korjattava. Virheellisesti määritetyt laitteet voivat sisältää joko yhden seuraavista ongelmista tai niiden yhdistelmän:

    - Ei tunnistintietoja – Laitteet ovat lopetta tunnistimen tietojen lähettämisen. Laitteesta voidaan käynnistää rajoitettuja ilmoituksia.
    - Heikentynyt viestintä – Viestintä laitteen kanssa on heikentynyt. Tiedostojen lähettäminen syvällistä analyysia varten, tiedostojen estäminen, laitteen eristäminen verkosta ja muut toiminnot, jotka edellyttävät viestintää laitteen kanssa, eivät ehkä toimi.
- **Passiivinen** Laitteet, jotka ovat lopetta raportoinnin Defender for Endpoint -palveluun.

Voit ladata koko luettelon CSV-muodossa Vie-toiminnolla.

Lisätietoja on kohdassa [Sensorin tilan tarkastaminen Microsoft Defender for Endpointissa.](/microsoft-365/security/defender-endpoint/check-sensor-status)

Lisätietoja siitä, mikä aiheutti laitteen passiivisen tai virheellisen määrityksen, on kohdassa Korjaa huonosti toimivat tunnistimet [Microsoft Defender for Endpointissa.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)
