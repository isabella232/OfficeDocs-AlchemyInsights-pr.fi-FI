---
title: Rekisteröiminen Microsoft Intune iOS-laitteiden ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29468003"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Rekisteröiminen Microsoft Intune iOS-laitteiden ongelmien vianmääritys

Tarkista ongelman nyt alla luetellut resurssit. 
  
Joitakin yleisiä virhesanomia ja tarkkuutta vaiheet:
  
- **Laitteen Cap saavutettu** Käyttäjä on rekisteröitynyt ylittää laitteen enimmäiskoon laitteita. Tarkasteltava näitä asiakirjoja, voit [poistaa laitteen](https://docs.microsoft.com/en-us/intune/devices-wipe) tai [muuttaa laitteen enimmäiskoon](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **: Tämä palvelu ei tue. Rekisteröintikäytäntö ei:** Apple Push Notification Service (APNS) on määritetty tai uudistaa. Lue [tämän asiakirjan](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) ohjeita tämän tekemisestä. 
    
- **Käyttäjän käyttöoikeuden tyyppi ei kelpaa tai käyttäjänimeä ei tunnisteta:** Käyttäjän on oltava Intune tai EMS-käyttöoikeus. Tarkasteltava näitä asiakirjoja käyttöoikeuden kautta: [Office Admin Centerissä](https://docs.microsoft.com/en-us/intune/licenses-assign) tai [Azure portaalin](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).
    
Lisätietoja ja resursseja auttaa ratkaisemaan ongelmaasi:
  
1. [Intune vianmääritys-portaalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yhteisen rekisteröinti virheitä. Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/en-us/intune/help-desk-operators) tarkasteleminen. 
    
2. Tarkasteltava näitä asiakirjoja yleisiä virheitä, jotka estävät rekisteröinti ja ratkaisuja jokaiseen luettelo: [Vianetsintä opas](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [vianmääritys doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Rekisteröi Microsoft Intune iOS-laitteiden tietoja](https://docs.microsoft.com/en-us/intune/ios-enroll).
    

