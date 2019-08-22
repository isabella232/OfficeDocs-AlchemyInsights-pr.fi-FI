---
title: Rekisteröiminen Microsoft Intune Android-laitteiden ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500068"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Rekisteröiminen Microsoft Intune Android-laitteiden ongelmien vianmääritys

Tarkista ongelman nyt alla luetellut resurssit.
  
Joitakin yleisiä ongelmia ja tarkkuutta vaiheet:
  
 **Laite ole salattu virhe yrityksen portaali:** Android, alkaen v7.0, erityisesti uudemmat versiot vaativat käynnistyksen PIN-koodi, varmista, että laite on täysin salattu. Yhteisiä ratkaisuja, jotka käyttöön käynnistyksen PIN-tunnuksen tai laitteen täysin salaa. Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) tarkasteleminen.
  
 **Laitteet eivät Intune palvelu tulee tarkistaa tai näyttää Intune hallintakonsolissa ”Unhealthy”:** Jotkut Samsung 4.4 ja 5.5 laitteet ei välttämättä tarkista palveluun. 3 mahdollisia ratkaisuja tähän ongelmaan on:
  
1. Avaa app Intune yrityksen portaali, jossa laitteen synkronointi automaattisesti aloittaa manuaalisesti.

2. Päivitä laitteen Android 6.0 tai uudempi versio.

3. Samsung Smart hallinnan käytöstä hallitsemasta Intune yrityksen portaaliin. Lue [Tämä asiakirja](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) on lisätietoja näistä ongelmista ja ratkaisuja.

 **Käyttäjän käyttöoikeuden tyyppi ei kelpaa** tai **Virhe käyttäjän nimeä ei tunnistettu:** käyttäjä on varattava Intune tai EMS-käyttöoikeus. Tarkasteltava näitä asiakirjoja käyttöoikeuden kautta: Office Admin Centerissä tai Azure portal.
  
Lisätietoja ja resursseja auttaa ratkaisemaan ongelmaasi:
  
1. [Intune vianmääritys-portaalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yhteisen rekisteröinti virheitä. Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/intune/help-desk-operators) tarkasteleminen.

2. Yleisiä virheitä, jotka estävät rekisteröinti ja ratkaisuja jokaiseen luettelo [tämän asiakirjan](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) tarkasteleminen.

3. [Rekisteröi Microsoft Intune Android-laitteiden tietoja](https://docs.microsoft.com/intune/android-enroll).
