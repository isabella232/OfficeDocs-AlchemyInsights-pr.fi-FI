---
title: iOS-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708959"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>iOS-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa

Ratkaise ongelmasi nyt alla lueteltujen resurssien avulla. 
  
Joitakin yleisiä virhesanomia ja ratkaisuvaiheita:
  
- **Laitteen kapi on saavutettu** Käyttäjällä on enemmän laitteita, jotka on rekisteröity laiterajoitusta enemmän. Voit poistaa laitteen [tai muuttaa laiterajoitusta](https://docs.microsoft.com/intune/devices-wipe) [tarkistamalla nämä asiakirjat.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Tätä palvelua ei tueta. Ei rekisteröintikäytäntöä:** Apple Push Notification Service (APNS) on määritettävä tai uusittava. Katso [ohjeet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) tähän asiakirjaan. 
    
- **Käyttäjäkäyttöoikeustyyppi virheellinen tai käyttäjänimiä ei tunnisteta:** Käyttäjälle on oltava määritetty Intune- tai EMS-käyttöoikeus. Tarkista nämä asiakirjat ja määritä käyttöoikeus Office-hallintakeskuksen tai [Azure-portaalin kautta.](https://docs.microsoft.com/azure/active-directory/license-users-groups) [](https://docs.microsoft.com/intune/licenses-assign)
    
Lisäresursseja ongelman ratkaisemiseen:
  
1. [Intunen vianmääritysportaalin avulla](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) voit diagnosoida ja ratkaista yleisiä rekisteröintivirheitä. Katso [lisätietoja tästä](https://docs.microsoft.com/intune/help-desk-operators) asiakirjasta. 
    
2. Tarkistamalla nämä asiakirjat saat luettelon yleisistä virheistä, jotka estävät rekisteröitymisen ja ratkaisut kuhunkin: [vianmääritysopas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [vianmäärityksen asiakirja.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Lue, miten voit rekisteröidä iOS-laitteita Microsoft Intunessa.](https://docs.microsoft.com/intune/ios-enroll)
    

