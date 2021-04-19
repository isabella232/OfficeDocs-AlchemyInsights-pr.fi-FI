---
title: Windowsin muistin diagnostiikan käyttö Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826664"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Windowsin muistin diagnostiikan käyttö Windows 10:ssä

Jos tietokoneesi Windows ja sovellukset kaatavat, jäädyvät tai toimivat epävakaalla tavalla, tietokoneen muistissa (RAM-muistissa) voi olla ongelma. Voit tarkistaa tietokoneen RAM-muistiongelmat Windowsin muistin diagnostiikan avulla.

Kirjoita tehtäväpalkin hakuruutuun muistin **vianmääritys** ja valitse sitten **Windowsin muistin vianmääritys**. 

Jotta voit suorittaa vianmäärityksen, tietokone on käynnistettävä uudelleen. Voit käynnistää vianmäärityksen heti uudelleen (tallenna työsi ja sulje ensin avoimet asiakirjat ja sähköpostiviestit) tai ajoita vianmääritys toimimaan automaattisesti, kun tietokone seuraavan kerran käynnistyy uudelleen:

![Windowsin muistin vianmääritys](media/windows-memory-diagnostic.png)

Kun tietokone käynnistyy uudelleen, **Windowsin muistin diagnostiikkatyökalu** toimii automaattisesti. Tila ja edistyminen näytetään diagnostiikan suorittamisen aikana, ja voit peruuttaa diagnostiikan  painamalla ESC-näppäintä.

Kun diagnostiikka on valmis, Windows käynnistyy normaalisti.
Heti uudelleenkäynnistyksen jälkeen näyttöön tulee työpöytä-ilmoitus (tehtäväpalkin Toimintokeskus-kuvakkeen vieressä) sen merkiksi, löytyikö muistivirheitä.  Esimerkkejä:

Tässä on Toimintokeskus-kuvake: ![Toimintokeskuksen kuvake](media/action-center-icon.png) 

Esimerkkiilmoitus: ![Ei muistivirheitä](media/no-memory-errors.png)

Jos et saanut ilmoitusta, voit  tuoda toimintokeskuksen näkyviin ja  tarkastella vieritettävää ilmoitusluetteloa valitsemalla tehtäväpalkista Toimintokeskus-kuvakkeen.

Voit tarkastella yksityiskohtaisia tietoja **kirjoittamalla tapahtuman** tehtäväpalkin hakuruutuun ja valitsemalla sitten **Tapahtumienvalvonta**. Siirry **Tapahtumienvalvonnan** vasemmanpuoleisessa ruudussa kohtaan **Windows-lokit > järjestelmä**. Etsi oikeanpuoleisessa ruudussa luetteloa samalla,  kun tarkastelet Lähde-saraketta, kunnes näet Tapahtumat, joiden arvo on **Lähdearvo MemoryDiagnostics-Results.** Korosta kukin tapahtuma ja katso tulostiedot luettelon alapuolella olevassa **Yleiset-välilehden** ruudussa.
