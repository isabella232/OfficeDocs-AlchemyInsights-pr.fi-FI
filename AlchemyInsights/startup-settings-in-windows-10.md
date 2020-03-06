---
title: Käynnistysasetukset Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409066"
---
# <a name="startup-settings-in-windows-10"></a>Käynnistysasetukset Windows 10:ssä

**Automaattisesti käynnistyksen yhteydessä suoritettavan sovelluksen muuttaminen**

1. Siirry [asetukset > Sovellukset > Käynnistys](ms-settings:startupapps?activationSource=GetHelp).

2. Varmista, että kaikki sovellukset, jotka haluat suorittaa käynnistyksen yhteydessä, ovat **käytössä**.

**Sovelluksen lisääminen suoritettavaksi automaattisesti käynnistyksen yhteydessä**

1. Napsauta tai napauta **Käynnistä** ja etsi sovellus, jonka haluat suorittaa käynnistettäessä.

2. Napsauta sovellusta hiiren kakkospainikkeella, valitse **Lisää**ja valitse sitten **Avaa tiedoston sijainti**. Tämä avaa sijainnin, johon sovelluksen pikakuvake tallennetaan. Jos Avaa tiedostosijainti -asetukselle ei ole vaihtoehtoa, sovellusta ei voi suorittaa käynnistyksen yhteydessä.

3. Kun tiedoston sijainti on avoinna, paina **Windows-näppäintä + R**, kirjoita **shell:startup**ja valitse sitten **OK**. Tämä avaa Käynnistys-kansion.

4. Kopioi ja liitä sovelluksen pikakuvake tiedoston sijainnista Käynnistys-kansioon.

**Käynnistyksen lisäasetukset (mukaan lukien vikasietotila, UEFI-asetukset ja käynnistys toisesta laitteesta)**

1. Tallenna työsi ja sulje avoimet asiakirjat, koska nämä vaiheet käynnistävät tietokoneen uudelleen.

2. Siirry [kohtaan Asetukset > Päivitys & Suojaus > Recovery](ms-settings:recovery?activationSource=GetHelp).

3. Valitse **Käynnistyksen lisäasetukset**-kohdassa **Käynnistä uudelleen nyt**. 

4. Kun tietokone on käynnistynyt uudelleen Valitse vaihtoehto -näyttöön:

    - Jos haluat käynnistää laitteen USB-aseman kaltaiseksi, valitse **Käytä laitetta**.

    - Jos haluat syöttää UEFI-asetukset (joita kutsutaan joskus BIOS-asetuksiksi), valitse **> UEFI-laiteohjelmiston asetukset > Lisäasetukset .** 

    - Jos haluat siirtyä vikasietotilaan tai muuttaa käynnistyksen lisäasetuksia, valitse **Vianmääritys > Lisäasetukset > Käynnistysasetukset**ja valitse sitten **Käynnistä uudelleen**. Sinua saatetaan pyytää antamaan [BitLocker-palautusavain](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Kun tietokone käynnistyy uudelleen, napsauta käynnistysasetusta, jota haluat käyttää.