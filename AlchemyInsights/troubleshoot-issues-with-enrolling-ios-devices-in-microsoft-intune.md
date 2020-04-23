---
title: iOS-laitteiden rekisteröiminen Microsoft Intunen ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736155"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>iOS-laitteiden rekisteröiminen Microsoft Intunen ongelmien vianmääritys

Ratkaise ongelma nyt alla olevien resurssien avulla. 
  
Joitakin yleisiä virhesanomia ja ratkaisuvaiheita:
  
- **Laitteen korkki saavutettu** Käyttäjällä on enemmän laitteita kuin laiteraja. Poista [laite](https://docs.microsoft.com/intune/devices-wipe) tai muuta [laitteen rajaa](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)tarkastelemalla näitä asiakirjoja.
    
- **Tätä palvelua ei tueta. Ei ilmoittautumiskäytäntöä:** Applen push-ilmoituspalvelu (APNS) on määritettävä tai uusittava. Tässä [asiakirjassa](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) on ohjeet sen käyttämiseen. 
    
- **Käyttöoikeustyyppi ei kelpaa tai käyttäjänimeä ei tunnisteta:** Käyttäjälle on annettava Intune- tai EMS-lisenssi. Tarkista nämä asiakirjat ja määritä käyttöoikeus: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) tai [Azure-portaali](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Lisäresursseja ongelman ratkaisemiseen:
  
1. [Intune Troubleshooting Portalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yleisiä rekisteröintivirheitä. Lisätietoja on [tässä asiakirjassa.](https://docs.microsoft.com/intune/help-desk-operators) 
    
2. Näissä asiakirjoissa on luettelo yleisistä virheistä, jotka estävät rekisteröitymisen ja tarkkuuden kuhunkin: [Vianmääritysopas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [Vianmääritysasiakirja](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Lue, miten voit rekisteröidä iOS-laitteet Microsoft Intuneen](https://docs.microsoft.com/intune/ios-enroll).
    

