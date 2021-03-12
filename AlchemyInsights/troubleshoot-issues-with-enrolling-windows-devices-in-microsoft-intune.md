---
title: Windows-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708887"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Windows-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa

Ratkaise ongelmasi nyt alla lueteltujen resurssien avulla.
  
Joitakin yleisiä virhesanomia ja ratkaisuvaiheita:
  
 **Ohjelmistoa ei voi asentaa, 0x80cf4017:** Tilivarmenne on vanhentunut. Lataa PC Client -ohjelmistopaketti uudelleen Intune-hallintakonsolissa. Saat lisätietoja tästä ohjeista.
  
 **Virhekoodin 0x801c0003:** Virhe voi ilmetä seuraavissa tilanteissa:
  
-  Käyttäjällä on enemmän laitteita, jotka on rekisteröity laiterajoitusta enemmän. Voit poistaa laitteen [tai muuttaa laiterajoitusta](https://docs.microsoft.com/intune/devices-wipe) [tarkistamalla nämä asiakirjat.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  Käyttäjät voivat liittyä laitteisiin Azure AD:ssä -asetuksena on Ei mitään. Määritä se kaikille tai valitse käyttäjille. Saat [lisätietoja tästä](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) ohjeista.

-  Toinen käyttäjä on jo rekisteröinyt laitteen. Jos näin on, poista laite Azure Intune -konsolista tai poista laitteen tilaus manuaalisesti, ennen kuin yrität uudelleen.

-  Laite on Windows 10 Home. Vain Windows 10 Pro-, Education- ja Enterprise-käyttäjät voivat liittyä Azure Active Directoryyn.

Lisäresursseja ongelman ratkaisemiseen:
  
-  [Intunen vianmääritysportaalin avulla](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) voit diagnosoida ja ratkaista yleisiä rekisteröintivirheitä. Katso [lisätietoja tästä](https://docs.microsoft.com/intune/help-desk-operators) asiakirjasta.

-  Tarkistamalla nämä asiakirjat saat luettelon yleisistä virheistä, jotka estävät rekisteröitymisen ja ratkaisut kuhunkin: [vianmääritysopas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [vianmäärityksen asiakirja.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Opi rekisteröimaan Windows-laitteita Microsoft Intunessa.](https://docs.microsoft.com/intune/windows-enroll)
