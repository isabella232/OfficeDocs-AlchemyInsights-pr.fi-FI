---
title: Käynnistysasetukset Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828149"
---
# <a name="startup-settings-in-windows-10"></a>Käynnistysasetukset Windows 10:ssä

**Muuta, mitkä sovellukset suoritetaan automaattisesti käynnistyksen yhteydessä**

1. Valitse Asetukset [> sovellukset > käynnistys .](ms-settings:startupapps?activationSource=GetHelp)

2. Varmista, että mikä tahansa käynnistettäessä suoritettava sovellus **on** käytössä .

**Sovelluksen lisääminen automaattisesti suoritettavaksi käynnistyksen yhteydessä**

1. Valitse Käynnistä **ja** etsi sovellus, jonka haluat suorittaa käynnistyksen yhteydessä.

2. Napsauta sovellusta hiiren kakkospainikkeella, **valitse Lisää** ja valitse sitten **Avaa tiedostosijainti**. Tämä avaa sijainnin, johon sovelluksen pikakuvake on tallennettu. Jos Avaa tiedostosijainti -vaihtoehtoa ei ole, sovellusta ei voi suorittaa käynnistyksen yhteydessä.

3. Kun tiedostosijainti on auki, paina **näppäinyhdistelmää Windows-näppäin + R,** **kirjoita shell:startup** ja valitse **sitten OK**. Tämä avaa Käynnistys-kansion.

4. Kopioi ja liitä pikakuvake sovellukseen tiedoston sijainnista Käynnistys-kansioon.

**Käynnistyksen lisäasetukset (mukaan lukien vikasietotila, UEFI-asetukset ja käynnistys toisesta laitteesta)**

1. Tallenna työsi ja sulje kaikki avoimet tiedostot, koska nämä vaiheet käynnistävät tietokoneen uudelleen.

2. Siirry kohtaan [Asetukset > päivittäminen & suojausasetusten > palautus.](ms-settings:recovery?activationSource=GetHelp)

3. Valitse **Käynnistyksen lisäasetukset**-kohdassa **Käynnistä uudelleen nyt**. 

4. Kun tietokone käynnistyy uudelleen Valitse vaihtoehto -näyttöön:

    - Jos haluat käynnistää laitteen, kuten USB-muistitikun, valitse **Käytä laitetta**.

    - Jos haluat määrittää UEFI-asetukset (kutsutaan joskus MYÖS -määritykseksi), **valitse Vianmääritys > UEFI-laiteohjelmistoasetusten > lisäasetukset.** 

    - Jos haluat käyttää vikasietotilaa tai muuttaa käynnistyksen lisäasetuksia, **valitse > Käynnistysasetukset >** vianmääritys ja valitse sitten Käynnistä **uudelleen**. Sinua saatetaan pyytää antamaan [BitLocker-palautusavain.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Kun tietokone käynnistyy uudelleen, valitse käynnistysasetus, jota haluat käyttää.