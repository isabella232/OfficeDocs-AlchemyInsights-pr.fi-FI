---
title: Android-laitteiden rekisteröimisen ongelmien vian määritys Microsoft Intunella
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689951"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Android-laitteiden rekisteröimisen ongelmien vian määritys Microsoft Intunella

Ratkaise ongelma nyt alla lueteltujen resurssien avulla.
  
Yleisiä ongelmia ja ratkaisu vaiheita:
  
 **Laite ei ole salattu virhe yritys portaalissa:** Androidin uudemmat versiot, erityisesti v 7.0:n versiosta alkaen, vaativat käynnistys tunnus koodin, jolla varmistetaan, että laitteesi on täysin salattu. Yleisiä ratkaisuja on ottaa käyttöön käynnistys PIN-koodi tai täysin salata laite. Katso lisä tietoja [tästä asia kirjasta](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .
  
 **Laitteet eivät ole sisäänkuittausta Intune-palvelussa tai ne näkyvät Epäterveinä Intune-hallinta konsolissa:** Jotkin Samsung 4,4-ja 5,5-laitteet eivät välttämättä Tarkista palvelua. Tähän ongelmaan on kolme mahdollista ratkaisua:
  
1. Avaa Intune Company Portal-sovellus manuaalisesti, joka käynnistää automaattisesti laitteen synkronoinnin.

2. Päivitä laite Android 6,0 tai uudempaan versioon.

3. Poista Samsung Smart-hallinta käytöstä Intune-yritys portaalin Hallin nasta. Katso lisä tietoja näistä ongelmista ja ratkaisuista lukemalla [Tämä asia kirja](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) .

 **Käyttö oikeuden tyyppi ei kelpaa** tai **käyttäjä nimi ei tunnista virhettä:** käyttäjälle on määritetään INTUNE-tai EMS-käyttö oikeus. Voit määrittää käyttö oikeuden seuraavien tiedostojen avulla: Office-hallinta keskus tai Azure-portaali.
  
Lisä resursseja ongelman ratkaisemiseen:
  
1. Käytä [Intune-vian määritys portaalia](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) yleisten rekisteröinti virheiden diagnosointiin ja ratkaisemiseen. Katso lisä tietoja [tästä asia kirjasta](https://docs.microsoft.com/intune/help-desk-operators) .

2. Tarkista [Tämä asia kirja](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , jossa on luettelo yleisistä virheistä, jotka estävät rekisteröinnin ja päätös lauselmien kunkin.

3. [Opi rekisteröimään Android-laitteet Microsoft Intunella](https://docs.microsoft.com/intune/android-enroll).
