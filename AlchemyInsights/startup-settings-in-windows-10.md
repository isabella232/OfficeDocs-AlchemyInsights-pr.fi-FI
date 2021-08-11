---
title: Käynnistysasetukset Windows 10
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
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909823"
---
# <a name="startup-settings-in-windows-10"></a>Käynnistysasetukset Windows 10

**Muuta, mitkä sovellukset suoritetaan automaattisesti käynnistyksen yhteydessä**

1. Siirry [Asetukset >-> käynnistys .](ms-settings:startupapps?activationSource=GetHelp)

2. Varmista, että mikä tahansa käynnistettäessä suoritettava sovellus **on** käytössä .

**Sovelluksen lisääminen automaattisesti suoritettavaksi käynnistyksen yhteydessä**

1. Valitse Käynnistä **ja** etsi sovellus, jonka haluat suorittaa käynnistyksen yhteydessä.

2. Napsauta sovellusta hiiren kakkospainikkeella, **valitse Lisää** ja valitse sitten **Avaa tiedostosijainti**. Tämä avaa sijainnin, johon sovelluksen pikakuvake on tallennettu. Jos Avaa tiedostosijainti -vaihtoehtoa ei ole, sovellusta ei voi suorittaa käynnistyksen yhteydessä.

3. Kun tiedostosijainti on auki, paina **Windows -näppäin + R**, kirjoita **shell:startup** ja valitse **SITTEN OK**. Tämä avaa Käynnistys-kansion.

4. Kopioi ja liitä pikakuvake sovellukseen tiedoston sijainnista Käynnistys-kansioon.

**Käynnistyksen lisäasetukset (Lokero, UEFI-asetukset ja käynnistys toisesta laitteesta)**

1. Tallenna työsi ja sulje kaikki avoimet tiedostot, koska nämä vaiheet käynnistävät tietokoneen uudelleen.

2. Siirry [Asetukset >-& suojauspäivitysten > palauttamiseen.](ms-settings:recovery?activationSource=GetHelp)

3. Valitse **Käynnistyksen lisäasetukset**-kohdassa **Käynnistä uudelleen nyt**. 

4. Kun tietokone käynnistyy uudelleen Valitse vaihtoehto -näyttöön:

    - Jos haluat käynnistää laitteen, kuten USB-muistitikun, valitse **Käytä laitetta**.

    - Jos haluat määrittää UEFI-asetukset (jota kutsutaan joskus MYÖS asennukseksi), valitse Vianmääritys > lisäasetukset **> UEFI Firmware Asetukset.** 

    - Siirry Lokero tilaan tai muuta käynnistyksen lisäasetuksia valitsemalla Vianmääritys > lisäasetukset **> Käynnistys Asetukset** ja valitsemalla sitten Käynnistä **uudelleen**. Sinua saatetaan pyytää antamaan [BitLocker-palautusavain.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Kun tietokone käynnistyy uudelleen, valitse käynnistysasetus, jota haluat käyttää.