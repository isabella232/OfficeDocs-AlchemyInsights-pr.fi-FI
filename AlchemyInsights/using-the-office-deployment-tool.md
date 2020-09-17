---
title: Officen käyttöönotto työkalun käyttäminen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794908"
---
# <a name="using-the-office-deployment-tool-odt"></a>Officen käyttöönotto työkalun (ODT) käyttäminen

Käytät Officen käyttöönotto työkalua (ODT) Office 365-versioiden käyttöönottoon. Officen käyttöönotto työkalu (setup.exe) suoritetaan komento riviltä, ja sen avulla määritetään, mitkä asetukset otetaan käyttöön Officen käyttöönoton yhteydessä.
  
1. Lataa Officen käyttöönotto työkalun uusin versio [Microsoft Download Centeristä](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Voit valita käyttöönoton asetukset ja luoda määrityksen XML-tiedoston [Officen mukautus työkalun (OCT)](https://config.office.com) avulla. Vie määritys tiedosto ja sijoita se paikallisesti samaan kansioon, jossa setup.exe sijaitsee.

    **Huomautus:** Officen asennus ongelmat tapahtuvat yleensä väärin käytettyjen määritys tiedostojen vuoksi. Jos haluat välttää tällaiset ongelmat, suosittelemme, että luot määritys tiedoston Officen mukautus työkalun avulla. Voit myös tuoda aiemmin luotuja määritys tiedostoja Officen mukautus työkaluun.

3. Siirry laajennetussa komento kehotteessa sijaintiin, jossa setup.exe sijaitsee, ja suorita Officen käyttöönotto työkalu lataus tilassa ja määritä juuri tallentamasi määritys tiedosto. Tässä esimerkissä määritys tiedoston nimi on Configuration.xml:

```setup.exe /download Configuration.xml```

4. Suorita Officen käyttöönotto työkalu Määritä-tilassa ja määritä määritys tiedosto.

```setup.exe /configure Configuration.xml```

**Huomautus:** Sinun on suoritettava tämä vaihe asiakas tieto koneesta, johon haluat asentaa Officen, ja sinulla on oltava paikallisen Järjestelmänvalvoja-oikeudet kyseisessä tieto koneessa.

Lisä tietoja Officen käyttöönotto työkalun käyttämisestä Microsoft 365-sovelluksissa yritys käyttöönoton skenaarioissa on artikkelissa [yleistä Office-käyttöönotto työkalusta](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Lisä tietoja Officen mukautus työkalun käyttämisestä on Ohje aiheessa [Officen mukautus työkalun yleiskatsaus](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
