---
title: 'Windows 10: n käynnistys asetukset'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751132"
---
# <a name="startup-settings-in-windows-10"></a>Windows 10: n käynnistys asetukset

**Käynnistettäessä automaattisesti käynnistettävien sovellusten muuttaminen**

1. Siirry kohtaan [Asetukset > sovellukset > käynnistys](ms-settings:startupapps?activationSource=GetHelp).

2. Varmista, että jokin sovellus, jonka haluat suorittaa käynnistettäessä **,** on otettu käyttöön.

**Sovelluksen lisääminen suoritettavaksi automaattisesti käynnistettäessä**

1. Napsauta tai napauta **Käynnistä** ja Etsi sovellus, jonka haluat suorittaa käynnistettäessä.

2. Napsauta sovellusta hiiren kakkos painikkeella, valitse **Lisää**ja valitse sitten **Avaa tiedosto sijainti**. Tämä avaa sijainnin, johon sovelluksen pikakuvake tallennetaan. Jos avointa tiedosto sijaintia ei ole, se tarkoittaa, että sovellusta ei voi suorittaa käynnistettäessä.

3. Kun tiedosto sijainti on avattuna, paina **Windows-näppäintä + R**, kirjoita **Shell: Startup**ja valitse sitten **OK**. Käynnistys-kansio avautuu.

4. Kopioi ja Liitä pikakuvake sovellukseen tiedoston sijainnista Startup-kansioon.

**Käynnistyksen lisä asetukset (mukaan lukien vika sieto tila, UEFI-asetukset ja käynnistäminen toisesta laitteesta)**

1. Tallenna työsi ja sulje kaikki avoimet asia kirjat, koska nämä vaiheet käynnistävät tieto koneen uudelleen.

2. Valitse [Asetukset > päivitys & tieto turva > palautus](ms-settings:recovery?activationSource=GetHelp).

3. Valitse **käynnistyksen lisä asetukset**-kohdassa **Käynnistä uudelleen nyt**. 

4. Kun tieto kone on käynnistynyt uudelleen, valitse vaihto ehto-näyttö:

    - Jos haluat käynnistää laitteen, kuten USB-muisti tikun, valitse **Käytä laitetta**.

    - Jos haluat määrittää UEFI-asetukset (joskus BIOS-määritys), valitse **vian määritys > lisä asetukset > UEFI firmware Settings**. 

    - Jos haluat siirtyä vika sieto tilaan tai muuttaa käynnistyksen lisä asetuksia, valitse **vian määritys > lisä asetukset > käynnistys asetukset**ja valitse sitten **Käynnistä uudelleen**. Sinua saatetaan pyytää antamaan [BitLocker-palautus avain](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Kun tieto kone on käynnistynyt uudelleen, valitse käynnistys asetus, jota haluat käyttää.