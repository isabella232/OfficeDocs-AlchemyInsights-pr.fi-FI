---
title: iOS-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823460"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>iOS-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa

Ratkaise ongelma nyt alla lueteltujen resurssien avulla. 
  
Yleisiä virhesanomia ja ratkaisuvaiheita:
  
- **Laitteen kapetin saavutettu** Käyttäjällä on laiterajoitusta suurempia laitteita. Tarkista nämä [asiakirjat, jos haluat poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai muuttaa laitteen [rajoitusta.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Tätä palvelua ei tueta. Ei rekisteröintikäytäntöä:** Apple Push Notification Service (APNS) on määritettävä tai uusittava. Katso [ohjeet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) tästä asiakirjasta. 
    
- **Käyttäjäkäyttöoikeustyyppi Virheellinen tai käyttäjänimi ei tunnistettu:** Käyttäjälle on oltava määritetty Intune- tai EMS-käyttöoikeus. Tarkista nämä asiakirjat ja määritä käyttöoikeus [Office-hallintakeskuksen tai](https://docs.microsoft.com/intune/licenses-assign) [Azure-portaalin kautta.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Lisäresursseja ongelman ratkaisemiseksi:
  
1. [Intunen vianmääritysportaalin avulla voit](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tehdä vianmäärityksen ja ratkaista yleisiä rekisteröintivirheitä. Katso [lisätietoja](https://docs.microsoft.com/intune/help-desk-operators) tästä asiakirjasta. 
    
2. Tarkistamalla nämä asiakirjat saat luettelon yleisistä virheistä, jotka estävät kunkin tiedoston rekisteröinnin ja ratkaisut: [Vianmääritysopas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [Tiedoston vianmääritys.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Lue, miten voit rekisteröidä iOS-laitteet Microsoft Intunessa.](https://docs.microsoft.com/intune/ios-enroll)
    

