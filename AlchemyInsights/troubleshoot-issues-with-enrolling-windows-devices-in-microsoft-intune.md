---
title: Windows-laitteiden rekisteröimiseen Microsoft Intuneen liittyvien ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665829"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Windows-laitteiden rekisteröimiseen Microsoft Intuneen liittyvien ongelmien vianmääritys

Tarkastele alla lueteltuja resursseja ratkaistaksesi ongelman nyt.
  
Joitakin yleisiä virhesanomia ja ratkaisuvaiheita:
  
 **Ohjelmistoa ei voi asentaa, 0x80cf4017:** Tilisi varmenne on vanhentunut. Lataa PC Client -ohjelmistopaketti uudelleen Intune Admin Consolessa. Lisätietoja on näissä ohjeissa.
  
 **Virhekoodi 0x801c0003:** Virhe voi ilmetä seuraavissa tilanteissa:
  
-  Käyttäjällä on enemmän laitteita, jotka on rekisteröity laiterajaa suuremmaksi. Näiden asiakirjojen avulla voit [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laiterajoitusta](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Käyttäjät voivat liittyä laitteisiin Azure AD:hen" -asetuksena on ei mitään. Aseta se kaikille tai valitse käyttäjät. Lisätietoja [on näissä ohjeissa.](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)

-  Toinen käyttäjä on jo rekisteröinyt laitteen. Jos näin on, poista laite Azure Intune -konsolista tai poista laite manuaalisesti käytöstä ennen kuin yrität uudelleen.

-  Laite on Windows 10 Home. Azure Active Directoryyn voi liittyä vain Windows 10 Pro-, Education- ja Enterprise SKU -käyttöyksiköt.

Muita resursseja ongelman ratkaisemiseen:
  
-  [Intune Troubleshooting Portalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yleisiä rekisteröintivirheitä. Lisätietoja on [tässä asiakirjassa.](https://docs.microsoft.com/intune/help-desk-operators)

-  Näiden asiakirjojen on luettelo yleisistä virheistä, jotka estävät rekisteröitymisen ja ratkaisut kuhunkin: [Vianmääritysopas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [Vianmääritys-asiakirja](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Tietoja Windows-laitteiden rekisteröimisestä Microsoft Intutiin.](https://docs.microsoft.com/intune/windows-enroll)
