---
title: Ääniongelmien vianmääritys Windows 10:ssä
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
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833288"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Ääniongelmien vianmääritys Windows 10:ssä

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

**Huomautus:** Jos Windows ei löydä uutta ohjainta, etsi ohjain laitteen valmistajan sivustosta ja noudata ohjeita.

**Asenna ohjain uudelleen**

Jos et voi päivittää laitehallinnan kautta tai etsiä uutta ohjainta valmistajan sivustosta, toimi seuraavasti:

1. Napsauta Laitehallinnassa ääniohjainta hiiren kakkospainikkeella (tai paina sitä pitkään) ja valitse **Poista asennus**. Käynnistä laite uudelleen, niin Windows yrittää asentaa ohjaimen uudelleen.

2. Jos ohjaimen uudelleenasentaminen ei toimi, kokeile Windowsin mukana toimitetaan yleistä ääniohjainta. Napsauta laitehallinnassa ääniohjainta hiiren kakkospainikkeella (tai paina sitä pitkään) > Päivitä ohjainohjelmisto Selaa tietokoneeni ohjainohjelmistoa Valitsen laiteohjaimen tietokoneen luettelosta , valitse  >    >   **Teräväpiirtoäänilaite**, valitse **Seuraava** ja asenna se noudattamalla ohjeita.
