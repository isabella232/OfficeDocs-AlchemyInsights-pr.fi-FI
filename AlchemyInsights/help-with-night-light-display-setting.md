---
title: Ohjeita yövalon näyttöasetukseen
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404400"
---
# <a name="help-with-the-night-light-display-setting"></a>Ohjeita yövalon näyttöasetukseen

Lisätietoja yönäytön asetuksista on ohjeaiheessa Näytön [määrittäminen yöksi Windows 10:ssä.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Jos yövalon asetukset näkyvät harmaina Asetuksissa, tarkista näyttöohjain: 

1. Napsauta tehtäväpalkin hakuruutua, kirjoita **Laitehallinta** ja valitse sitten **hakutuloksista** Laitehallinta.
1. Laajenna **näyttösovittimet.** 

Yövalotoiminto ei valitettavasti ole käytettävissä, jos laitteessasi on DisplayLink-ohjain tai perusnäyttöohjain.

Yövalo-ominaisuus käyttää viimeaikaista grafiikkatekniikkaa, joten sinun on ehkä päivitettävä näyttöohjain:  

- Tarkista päivitykset valitsemalla Windows  >  Updaten **suojauspäivityksen**  >  **&**  >  **aloitusasetusten**  >  **päivitys.**  

TAI

- Siirry laitteistovalmistajan tukisivustoon ja lataa ja asenna uusimmat näytönohjaimet manuaalisesti.

## <a name="reset-night-light-in-the-registry"></a>Rekisterin yövalon nollaaminen

Jos näytönohjaimen päivittäminen ei toiminut, sinun on ehkä palautettava rekisterin yövalo.  

**Varoitus:** Tätä vianmääritysvaihetta suositellaan vain kokeneille käyttäjille. Rekisterin virheellinen muokkaaminen voi aiheuttaa vakavia ongelmia. Jos haluat suojauksen, varmuuskopioi rekisteri ennen sen muokkaamista, jotta voit palauttaa sen, jos ongelmia ilmenee.

1. Kirjoita hakuruutuun **regedit ja** valitse **sitten** hakutuloksista Rekisterieditori.

1. Siirry seuraavaan rekisteriavaimeen: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Vie ja poista seuraava aliavain:$$windows.data.bluelightred disclaimer.bluelightredstate

1. Vie ja poista seuraava aliavain:$$windows.data.bluelightred disclaimer.settings

1. Käynnistä Windows uudelleen ja tarkista, onko yövaloasetukset käytettävissä.


