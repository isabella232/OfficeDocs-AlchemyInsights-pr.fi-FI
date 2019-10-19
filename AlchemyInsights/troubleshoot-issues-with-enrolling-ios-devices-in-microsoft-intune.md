---
title: IOS-laitteiden ilmoittautumalla-ongelmien vian määritys Microsoft Intune
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506922"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>IOS-laitteiden ilmoittautumalla-ongelmien vian määritys Microsoft Intune

Tarkista alla luetellut resurssit ongelman ratkaisemiseksi nyt. 
  
Yleisiä virhe sanomia ja ratkaisu vaiheita:
  
- **Laitteen suojus saavutettu** Käyttäjällä on enemmän laitteita, jotka on rekisteröity kuin laitteen rajoitus. Voit [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laitteen rajaa](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)näiden asia kirjojen avulla.
    
- **Tätä palvelua ei tueta. Ei rekisteröinti käytäntöä:** Applen push-ilmoitus palvelu (APNS) on määritettävä tai uusittava. Tarkastele [tätä asia kirjaa](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , niin saat ohjeita. 
    
- **Käyttö oikeus tyyppi ei kelpaa, tai käyttäjä nimeä ei tunnistettu:** Käyttäjälle on määritettävä Intune-tai EMS-lisenssi. Voit määrittää käyttö oikeuden näiden asia kirjojen avulla [Office-hallinta keskukseen](https://docs.microsoft.com/intune/licenses-assign) tai [Azure-portaaliin](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Lisä resursseja ongelman ratkaisemiseen:
  
1. Käytä [Intune-vian määritys portaalia](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) yleisten rekisteröinti virheiden diagnosoimiseen ja ratkaisemiseen. Lisä tietoja [on tämän asia kirjan](https://docs.microsoft.com/intune/help-desk-operators) tarkastelussa. 
    
2. Tarkastele näitä asia kirjoja, joissa on luettelo yleisistä virheistä, jotka estävät rekisteröintiä ja resoluutioita kuhunkin: [vian määritys opas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [vian etsintä doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Lue, miten voit rekisteröidä iOS-laitteita Microsoft Intunessa](https://docs.microsoft.com/intune/ios-enroll).
    

