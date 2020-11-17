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
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085829"
---
# <a name="using-the-office-deployment-tool-odt"></a>Officen käyttöönotto työkalun (ODT) käyttäminen

Käytät Officen käyttöönotto työkalua (ODT) Office 365-versioiden käyttöönottoon. Officen käyttöönotto työkalu (setupodt.exe) suoritetaan komento riviltä, ja sen avulla määritetään, mitkä asetukset otetaan käyttöön Officen käyttöönoton yhteydessä.
  
1. Lataa Officen käyttöönotto työkalun uusin versio [Microsoft Download Centeristä](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Voit valita käyttöönoton asetukset ja luoda määrityksen XML-tiedoston [Officen mukautus työkalun (OCT)](https://config.office.com) avulla. Vie määritys tiedosto ja sijoita se paikallisesti samaan kansioon, jossa setupodt.exe sijaitsee.

    **Huomautus:** Officen asennus ongelmat tapahtuvat yleensä väärin käytettyjen määritys tiedostojen vuoksi. Jos haluat välttää tällaiset ongelmat, suosittelemme, että luot määritys tiedoston Officen mukautus työkalun avulla. Voit myös tuoda aiemmin luotuja määritys tiedostoja Officen mukautus työkaluun.

3. Siirry laajennetussa komento kehotteessa sijaintiin, jossa setupodt.exe sijaitsee, ja suorita Officen käyttöönotto työkalu lataus tilassa ja määritä juuri tallentamasi määritys tiedosto. Tässä esimerkissä määritys tiedoston nimi on Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Suorita Officen käyttöönotto työkalu Määritä-tilassa ja määritä määritys tiedosto.

```setupodt.exe /configure Configuration.xml```

**Huomautus:** Sinun on suoritettava tämä vaihe asiakas tieto koneesta, johon haluat asentaa Officen, ja sinulla on oltava paikallisen Järjestelmänvalvoja-oikeudet kyseisessä tieto koneessa.

Lisä tietoja Officen käyttöönotto työkalun käyttämisestä Microsoft 365-sovelluksissa yritys käyttöönoton skenaarioissa on artikkelissa [yleistä Office-käyttöönotto työkalusta](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Lisä tietoja Officen mukautus työkalun käyttämisestä on Ohje aiheessa [Officen mukautus työkalun yleiskatsaus](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
