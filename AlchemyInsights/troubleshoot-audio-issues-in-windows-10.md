---
title: Ääniongelmien vianmääritys Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 81a7f77bd6565c52ec9d752934a872e59cc11e89b90a646d17c3549d72e8a69f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039423"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Ääniongelmien vianmääritys Windows 10

**Äänen vianmäärityksen käynnistäminen**

1.  Avaa [Vianmääritysasetukset](ms-settings:troubleshoot).

2.  Valitse **Äänen**  >  **toistaminen Suorita vianmääritys**.

**Oletuslaitteen asetukset**

Jos olet yhdistänyt äänilaitteeseen USB- tai HDMI-liitännällä, sinun on ehkä määritettävä tämä laite oletuslaitteeksi:

1. Avaa **Aloita**  >  **ääni** ja valitse sitten **tulosluettelosta** Ääni tai Muuta  järjestelmän ääniä.

2.  Valitse **Toisto-välilehdessä** laite, valitse **Aseta oletus** ja valitse sitten **OK**.

**Tarkista kaapelit, äänenvoimakkuus, kaiuttimet ja kuulokkeet**

1. Tarkista, ettei kaiuttimen ja kuulokkeiden yhteyksissä ole irtonaista kaapeleita, ja varmista, että ne on yhdistetty oikeaan liitäntään.

2. Tarkista virta- ja äänenvoimakkuustasot ja yritä kääntää kaikki äänenvoimakkuuden säätimet ylöspäin.

3. Joillakin kaiuttimillä ja sovelluksilla on omat äänenvoimakkuuden säätimet. sinun on ehkä tarkistamaan ne kaikki, jotta ne ovat oikealla tasolla.

4. Yritä muodostaa yhteys käyttämällä toista USB-porttia.

**Huomautus:** Muista, että kaiuttimet eivät ehkä toimi, kun kuulokkeet on kytketty.

**Tarkista Laitehallinta**

Voit varmistaa, että ohjaimet ovat ajan tasalla:

1. Valitse **Käynnistä**, **kirjoita Laitehallinta** ja valitse **sitten** tulosluettelosta Laitehallinta.

2. Valitse **Ääni-, video- ja peliohjaimet**-kohdassa äänikortti, avaa se, valitse **Ohjain-välilehti** ja valitse **Päivitä ohjain**.

**Huomautus:** Windows ei löydä uutta ohjainta, etsi ohjain laitteen valmistajan sivustosta ja noudata ohjeita.

**Asenna ohjain uudelleen**

Jos et voi päivittää laitehallinnan kautta tai etsiä uutta ohjainta valmistajan sivustosta, toimi seuraavasti:

1. Napsauta Laitehallinnassa ääniohjainta hiiren kakkospainikkeella (tai paina sitä pitkään) ja valitse **Poista asennus**. Käynnistä laite uudelleen Windows laite yrittää asentaa ohjaimen uudelleen.

2. Jos ohjaimen uudelleenasentaminen ei toimi, kokeile yleisen ääniohjaimen Windows. Napsauta laitehallinnassa ääniohjainta hiiren kakkospainikkeella (tai paina sitä pitkään) > Päivitä ohjainohjelmisto Selaa tietokoneeni ohjainohjelmistoa Valitsen laiteohjaimen tietokoneen luettelosta , valitse  >    >   **Teräväpiirtoäänilaite**, valitse **Seuraava** ja asenna se noudattamalla ohjeita.
