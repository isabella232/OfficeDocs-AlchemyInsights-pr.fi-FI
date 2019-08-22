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
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506922"
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
    

