---
title: Rekisteröiminen Microsoft Intune iOS-laitteiden ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391004"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Rekisteröiminen Microsoft Intune iOS-laitteiden ongelmien vianmääritys

Tarkista ongelman nyt alla luetellut resurssit. 
  
Joitakin yleisiä virhesanomia ja tarkkuutta vaiheet:
  
- **Laitteen Cap saavutettu** Käyttäjä on rekisteröitynyt ylittää laitteen enimmäiskoon laitteita. Tarkasteltava näitä asiakirjoja, voit [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laitteen enimmäiskoon](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **: Tämä palvelu ei tue. Rekisteröintikäytäntö ei:** Apple Push Notification Service (APNS) on määritetty tai uudistaa. Lue [tämän asiakirjan](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) ohjeita tämän tekemisestä. 
    
- **Käyttäjän käyttöoikeuden tyyppi ei kelpaa tai käyttäjänimeä ei tunnisteta:** Käyttäjän on oltava Intune tai EMS-käyttöoikeus. Tarkasteltava näitä asiakirjoja käyttöoikeuden kautta: [Office Admin Centerissä](https://docs.microsoft.com/intune/licenses-assign) tai [Azure portaalin](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Lisätietoja ja resursseja auttaa ratkaisemaan ongelmaasi:
  
1. [Intune vianmääritys-portaalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yhteisen rekisteröinti virheitä. Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/intune/help-desk-operators) tarkasteleminen. 
    
2. Tarkasteltava näitä asiakirjoja yleisiä virheitä, jotka estävät rekisteröinti ja ratkaisuja jokaiseen luettelo: [Vianetsintä opas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [vianmääritys doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Rekisteröi Microsoft Intune iOS-laitteiden tietoja](https://docs.microsoft.com/intune/ios-enroll).
    

