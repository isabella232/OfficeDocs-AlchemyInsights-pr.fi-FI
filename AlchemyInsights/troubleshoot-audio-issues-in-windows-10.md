---
title: Windows 10:n ääniongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: f51fd233db5ae068e719f1cf3bc94a0dac82444f
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265013"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Ääniongelmien vianmääritys Windows 10:ssä

**Äänen vianmäärityksen suorittaminen**

1.  Avaa [Vianmääritysasetukset](ms-settings:troubleshoot).

2.  Valitse **Äänen** > **toistaminen Suorita vianmääritys**.

**Oletuslaitteen määrittäminen**

Jos muodostat yhteyden äänilaitteeseen USB- tai HDMI-liitännän avulla, sinun on ehkä asetettava kyseinen laite oletuslaitteeksi:

1. Avaa **Aloita** > **ääni**ja valitse sitten tulosluettelosta **Ääni** tai Muuta **järjestelmän ääniä.**

2.  Valitse **Toisto-välilehdessä** laite, valitse **Aseta oletukseksi**ja valitse sitten **OK**.

**Kaapelien, äänenvoimakkuuden, kaiuttimien ja kuulokkeiden tarkistaminen**

1. Tarkista, ettei kaiutin- ja kuulokeliitännöissä ole irrallisia kaapeleita, ja varmista, että ne on liitetty oikeaan liitäntään.

2. Tarkista teho- ja äänenvoimakkuustasot ja yritä kääntää kaikki äänenvoimakkuuden säätimet ylöspäin.

3. Joillakin kaiuttimilla ja sovelluksilla on omat äänenvoimakkuuden säätimet; sinun on ehkä tarkistettava ne kaikki varmistaaksesi, että ne ovat oikealla tasolla.

4. Yritä muodostaa yhteys toisella USB-portilla.

**Huomautus**: Muista, että kaiuttimet eivät välttämättä toimi, kun kuulokkeet on kytketty.

**Tarkista Laitehallinta**

Voit varmistaa, että ohjaimet ovat ajan tasalla:

1. Valitse **Käynnistä**, kirjoita **Laitehallinta**ja valitse sitten **laitehallinta** tulosluettelosta.

2. Valitse **Ääni-, video- ja peliohjaimet**-kohdassa äänikortti, avaa se, valitse **Ohjain-välilehti** ja valitse **Päivitä ohjain**.

**Huomautus:** Jos Windows ei löydä uutta ohjainta, etsi sellainen laitteen valmistajan sivustosta ja noudata niiden ohjeita.

**Asenna ohjain uudelleen**

Jos et pysty päivittämään Laitehallinnan kautta tai löytämään uuden ohjaimen valmistajan sivustosta, kokeile seuraavia toimia:

1. Napsauta Laitehallinnassa ääniohjainta hiiren kakkospainikkeella (tai pidä sitä painettuna) ja valitse **Poista asennus**. Käynnistä laite uudelleen, niin Windows yrittää asentaa ohjaimen uudelleen.

2. Jos ohjaimen uudelleenasentaminen ei toimi, kokeile Windowsin mukana toimitetun yleisen ääniohjaimen käyttämistä. Napsauta Laitehallinnassa hiiren kakkospainikkeella (tai pidä painettuna) ääniohjainta > **Update-ohjainohjelmisto** > **Selaa tietokonetta ohjainohjelmistoksi** > Haluan valita tietokoneen**laiteohjaimien luettelosta**, valitse High Definition Audio **Device**, valitse **Seuraava**ja asenna se noudattamalla ohjeita.
