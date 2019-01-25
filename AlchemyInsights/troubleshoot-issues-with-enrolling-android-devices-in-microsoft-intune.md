---
title: Rekisteröiminen Microsoft Intune Android-laitteiden ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29467578"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Rekisteröiminen Microsoft Intune Android-laitteiden ongelmien vianmääritys

Tarkista ongelman nyt alla luetellut resurssit.
  
Joitakin yleisiä ongelmia ja tarkkuutta vaiheet:
  
 **Laite ole salattu virhe yrityksen portaali:** Android, alkaen v7.0, erityisesti uudemmat versiot vaativat käynnistyksen PIN-koodi, varmista, että laite on täysin salattu. Yhteisiä ratkaisuja, jotka käyttöön käynnistyksen PIN-tunnuksen tai laitteen täysin salaa. Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) tarkasteleminen. 
  
 **Laitteet eivät Intune palvelu tulee tarkistaa tai näyttää Intune hallintakonsolissa ”Unhealthy”:** Jotkut Samsung 4.4 ja 5.5 laitteet ei välttämättä tarkista palveluun. 3 mahdollisia ratkaisuja tähän ongelmaan on: 
  
1. Avaa app Intune yrityksen portaali, jossa laitteen synkronointi automaattisesti aloittaa manuaalisesti.
    
2. Päivitä laitteen Android 6.0 tai uudempi versio.
    
3. Samsung Smart hallinnan käytöstä hallitsemasta Intune yrityksen portaaliin. Lue [Tämä asiakirja](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) on lisätietoja näistä ongelmista ja ratkaisuja. 
    
 **Käyttäjän käyttöoikeuden tyyppi ei kelpaa** tai **Virhe käyttäjän nimeä ei tunnistettu:** käyttäjä on varattava Intune tai EMS-käyttöoikeus. Tarkasteltava näitä asiakirjoja käyttöoikeuden kautta: Office Admin Centerissä tai Azure portal. 
  
Lisätietoja ja resursseja auttaa ratkaisemaan ongelmaasi:
  
1. [Intune vianmääritys-portaalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yhteisen rekisteröinti virheitä. Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/en-us/intune/help-desk-operators) tarkasteleminen. 
    
2. Yleisiä virheitä, jotka estävät rekisteröinti ja ratkaisuja jokaiseen luettelo [tämän asiakirjan](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) tarkasteleminen. 
    
3. [Rekisteröi Microsoft Intune Android-laitteiden tietoja](https://docs.microsoft.com/en-us/intune/android-enroll).
    

