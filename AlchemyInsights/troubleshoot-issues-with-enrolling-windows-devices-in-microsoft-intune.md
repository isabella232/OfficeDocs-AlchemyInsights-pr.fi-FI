---
title: Rekisteröiminen Windows Microsoft Intune-laitteiden ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390640"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Rekisteröiminen Windows Microsoft Intune-laitteiden ongelmien vianmääritys

Tarkista ongelman nyt alla luetellut resurssit. 
  
Joitakin yleisiä virhesanomia ja tarkkuutta vaiheet:
  
 **Ei voi asentaa ohjelmiston 0x80cf4017:** Käyttäjän tili on vanhentunut. Lataa uudelleen PC-Client-ohjelmistopaketin Intune hallintakonsolissa. Tarkista tästä lisätietoja ohjeista. 
  
 **0x801c0003-virhekoodi:** Virhe voi ilmetä seuraavissa tilanteissa: 
  
1. Käyttäjä on rekisteröitynyt ylittää laitteen enimmäiskoon laitteita. Tarkasteltava näitä asiakirjoja, voit [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laitteen enimmäiskoon](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. ”Käyttäjät voivat liittää laitteet Azure AD” on määritetty ”none”. Valitse tai määritä se kaikille käyttäjille. Voit tarkastella [näitä ohjeita](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) . 
    
3. Toinen käyttäjä on jo liitetty laite. Jos näin on, poista laite Azure Intune konsolista tai Peruuta laitteen ilmoittautuminen manuaalisesti ennen kuin yrität uudelleen.
    
4. Laite on Windows 10 Home. Vain Windows 10 Pro, koulutus ja Enterprise SKU-tietoja voit liittää Azure Active Directory.
    
Lisätietoja ja resursseja auttaa ratkaisemaan ongelmaasi:
  
1. [Intune vianmääritys-portaalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yhteisen rekisteröinti virheitä. Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/intune/help-desk-operators) tarkasteleminen. 
    
2. Tarkasteltava näitä asiakirjoja yleisiä virheitä, jotka estävät rekisteröinti ja ratkaisuja jokaiseen luettelo: [Vianetsintä opas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [vianmääritys doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Rekisteröi Windows Microsoft Intune-laitteiden tietoja](https://docs.microsoft.com/intune/windows-enroll).
  

