---
title: Suorita Windows vianmääritys Windows 10
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
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922538"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Suorita Windows vianmääritys Windows 10

Jos Windows ja tietokoneesi sovellukset kaatuvat, jäädyvät tai toimivat epävakaalla tavalla, ongelma saattaa olla tietokoneen muistissa (RAM). Voit tarkistaa tietokoneen RAM Windows ongelmat suoritat muistiongelman vianmäärityksen avulla.

Kirjoita tehtäväpalkin hakuruutuun muistin **vianmääritys** ja valitse sitten Windows **muistidiagnostiikka**. 

Jotta voit suorittaa vianmäärityksen, tietokone on käynnistettävä uudelleen. Voit käynnistää vianmäärityksen heti uudelleen (tallenna työsi ja sulje ensin avoimet asiakirjat ja sähköpostiviestit) tai ajoita vianmääritys toimimaan automaattisesti, kun tietokone seuraavan kerran käynnistyy uudelleen:

![Windows Muistin vianmääritys](media/windows-memory-diagnostic.png)

Kun tietokone käynnistyy uudelleen, **Windows muistidiagnostiikkatyökalu** toimii automaattisesti. Tila ja edistyminen näytetään diagnostiikan suorittamisen aikana, ja voit peruuttaa diagnostiikan  painamalla ESC-näppäintä.

Kun diagnostiikka on valmis, Windows käynnistyy normaalisti.
Heti uudelleenkäynnistyksen jälkeen näyttöön tulee työpöytä-ilmoitus (tehtäväpalkin Toimintokeskus-kuvakkeen vieressä) sen merkiksi, löytyikö muistivirheitä.  Esimerkiksi:

Tässä on Toimintokeskus-kuvake: ![Toimintokeskuksen kuvake](media/action-center-icon.png) 

Esimerkkiilmoitus: ![Ei muistivirheitä](media/no-memory-errors.png)

Jos et saanut ilmoitusta, voit  tuoda toimintokeskuksen näkyviin ja  tarkastella vieritettävää ilmoitusluetteloa valitsemalla tehtäväpalkista Toimintokeskus-kuvakkeen.

Voit tarkastella yksityiskohtaisia tietoja **kirjoittamalla tapahtuman** tehtäväpalkin hakuruutuun ja valitsemalla sitten **Tapahtumienvalvonta**. Siirry **Tapahtumienvalvonnan** vasemmanpuoleisessa ruudussa kohtaan Windows **lokit > järjestelmä.** Etsi oikeanpuoleisessa ruudussa luetteloa samalla,  kun tarkastelet Lähde-saraketta, kunnes näet Tapahtumat, joiden arvo on **Lähdearvo MemoryDiagnostics-Results.** Korosta kukin tapahtuma ja katso tulostiedot luettelon alapuolella olevassa **Yleiset-välilehden** ruudussa.
