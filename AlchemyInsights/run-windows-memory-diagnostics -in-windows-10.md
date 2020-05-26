---
title: Windowsin muistin diagnostiikan suorittaminen Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357514"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Windowsin muistin diagnostiikan suorittaminen Windows 10:ssä

Jos tietokoneen Windows ja sovellukset kaatuvat, jäädyttävät tai toimivat epävakaalla tavalla, tietokoneen muistissa (RAM) saattaa olla ongelma. Voit tarkistaa tietokoneen RAM-muistin ongelmat suorittamalla Windowsin muistin diagnostiikan.

Kirjoita tehtäväpalkin hakuruutuun **muistin diagnostiikka**ja valitse sitten **Windowsin muistin diagnostiikka**. 

Jotta voit suorittaa vianmäärityksen, tietokoneen on käynnistettävä uudelleen. Voit käynnistää tietokoneen uudelleen välittömästi (tallenna työsi ja sulje ensin avoimet asiakirjat ja sähköpostiviestit) tai ajoittaa diagnostiikan käynnistymään automaattisesti, kun tietokone käynnistetään seuraavan kerran uudelleen:

![Windowsin muistin diagnostiikka](media/windows-memory-diagnostic.png)

Kun tietokone käynnistyy uudelleen, **Windowsin muistin diagnostiikkatyökalu** käynnistyy automaattisesti. Tila ja edistyminen näytetään diagnostiikan suorittamisen ajona, ja voit peruuttaa diagnostiikan painamalla näppäimistön **ESC-näppäintä.**

Kun diagnostiikka on valmis, Windows käynnistyy normaalisti.
Heti uudelleenkäynnistyksen jälkeen, kun työpöytä tulee näkyviin, **Action Center** näyttöön tulee ilmoitus (tehtäväpalkin Toimintokeskus-kuvakkeen vieressä), joka ilmaisee, onko muistivirheitä löytynyt. Esimerkiksi:

Tässä on Toimintokeskus-kuvake: ![Toimintokeskuksen kuvake](media/action-center-icon.png) 

Ja näyte ilmoitus: ![Ei muistivirheitä](media/no-memory-errors.png)

Jos et huomannut ilmoitusta, voit tuoda **toimintokeskuksen** näkyviin valitsemalla tehtäväpalkin **Toimintokeskus-kuvakkeen** ja nähdä vieritettävän ilmoitusluettelon.

Voit tarkastella yksityiskohtaisia tietoja kirjoittamalla **tehtäväpalkin** hakuruutuun tapahtuman ja valitsemalla sitten **Tapahtumienvalvonta**. Siirry **Tapahtumienvalvonnan**vasemmanpuoleisessa ruudussa **Windowsin lokit-> järjestelmä**. Skannaa oikeanpuoleisessa ruudussa luettelo alaspäin, kun tarkastelet **Lähde-saraketta,** kunnes näet tapahtumat, joiden **Lähde-arvo on MemoryDiagnostics-Results**. Korosta jokainen tällainen tapahtuma ja katso tulostiedot luettelon alapuolella olevan **Yleiset-välilehden** alla olevasta ruudusta.
