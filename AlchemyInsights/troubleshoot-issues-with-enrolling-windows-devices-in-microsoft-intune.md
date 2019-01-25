---
title: Rekisteröiminen Windows Microsoft Intune-laitteiden ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29467715"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Rekisteröiminen Windows Microsoft Intune-laitteiden ongelmien vianmääritys

Tarkista ongelman nyt alla luetellut resurssit. 
  
Joitakin yleisiä virhesanomia ja tarkkuutta vaiheet:
  
 **Ei voi asentaa ohjelmiston 0x80cf4017:** Käyttäjän tili on vanhentunut. Lataa uudelleen PC-Client-ohjelmistopaketin Intune hallintakonsolissa. Tarkista tästä lisätietoja ohjeista. 
  
 **0x801c0003-virhekoodi:** Virhe voi ilmetä seuraavissa tilanteissa: 
  
1. Käyttäjä on rekisteröitynyt ylittää laitteen enimmäiskoon laitteita. Tarkasteltava näitä asiakirjoja, voit [poistaa laitteen](https://docs.microsoft.com/en-us/intune/devices-wipe) tai [muuttaa laitteen enimmäiskoon](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. ”Käyttäjät voivat liittää laitteet Azure AD” on määritetty ”none”. Valitse tai määritä se kaikille käyttäjille. Voit tarkastella [näitä ohjeita](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) . 
    
3. Toinen käyttäjä on jo liitetty laite. Jos näin on, poista laite Azure Intune konsolista tai Peruuta laitteen ilmoittautuminen manuaalisesti ennen kuin yrität uudelleen.
    
4. Laite on Windows 10 Home. Vain Windows 10 Pro, koulutus ja Enterprise SKU-tietoja voit liittää Azure Active Directory.
    
Lisätietoja ja resursseja auttaa ratkaisemaan ongelmaasi:
  
1. [Intune vianmääritys-portaalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yhteisen rekisteröinti virheitä. Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/en-us/intune/help-desk-operators) tarkasteleminen. 
    
2. Tarkasteltava näitä asiakirjoja yleisiä virheitä, jotka estävät rekisteröinti ja ratkaisuja jokaiseen luettelo: [Vianetsintä opas](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [vianmääritys doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Rekisteröi Windows Microsoft Intune-laitteiden tietoja](https://docs.microsoft.com/en-us/intune/windows-enroll).
  

