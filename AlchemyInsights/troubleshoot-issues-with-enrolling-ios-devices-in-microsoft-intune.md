---
title: IOS-laitteiden rekisteröimisen ongelmien vian määritys Microsoft Intunella
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
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669245"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>IOS-laitteiden rekisteröimisen ongelmien vian määritys Microsoft Intunella

Ratkaise ongelma nyt alla lueteltujen resurssien avulla. 
  
Yleisiä virhe sanomia ja ratkaisu vaiheita:
  
- **Laitteen korkki saavutettu** Käyttäjällä on enemmän laitteita, jotka ovat rekisteröityneet kuin laitteen raja. Tarkista nämä asia kirjat, jos haluat [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laitteen rajoitusta](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Tätä palvelua ei voi käyttää. Ei rekisteröinti käytäntöä:** Applen push-ilmoitus palvelu (APNS) on määritettävä tai uusittava. Lue [Tämä asia kirja](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , jossa kerrotaan, miten se tehdään. 
    
- **Käyttö oikeuden tyyppi ei kelpaa tai käyttäjä nimeä ei tunnisteta:** Käyttäjälle on määritetään Intune-tai EMS-käyttö oikeus. Voit määrittää käyttö oikeuden seuraavien tiedostojen avulla: [Office-hallinta keskus](https://docs.microsoft.com/intune/licenses-assign) tai [Azure-portaali](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Lisä resursseja ongelman ratkaisemiseen:
  
1. Käytä [Intune-vian määritys portaalia](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) yleisten rekisteröinti virheiden diagnosointiin ja ratkaisemiseen. Katso lisä tietoja [tästä asia kirjasta](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Tutustu näihin asia kirjoihin, jos haluat luettelon yleisistä virheistä, jotka estävät rekisteröinnin ja päätös lauselmien kunkin: [vian määritys opas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [vian määritys-asiak](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Opi rekisteröimään iOS-laitteet Microsoft Intunella](https://docs.microsoft.com/intune/ios-enroll).
    

