---
title: Windows-laitteiden rekisteröimisen ongelmien vian määritys Microsoft Intunella
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
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658875"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Windows-laitteiden rekisteröimisen ongelmien vian määritys Microsoft Intunella

Ratkaise ongelma nyt alla lueteltujen resurssien avulla.
  
Yleisiä virhe sanomia ja ratkaisu vaiheita:
  
 **Ohjelmistoa ei voi asentaa, 0x80cf4017:** Tili varmenne on vanhentunut. Lataa uudelleen PC-asiakas ohjelmisto paketti Intune-hallinta konsolissa. Katso lisä tietoja tästä dokumentaatiosta.
  
 **Virhe koodi 0x801c0003:** Virhe voi ilmetä seuraavissa tilanteissa:
  
-  Käyttäjällä on enemmän laitteita, jotka ovat rekisteröityneet kuin laitteen raja. Tarkista nämä asia kirjat, jos haluat [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laitteen rajoitusta](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Käyttäjät voivat liittyä laitteisiin Azure AD:hen"-asetuksena on "ei mitään". Määritä se kaikille tai valitse käyttäjät. Katso lisä tietoja [tästä dokumentaatiosta](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Toinen käyttäjä on jo rekisteröinyt laitteen. Jos näin on, Poista laite Azure Intune-konsolista tai rekisteröi laite manuaalisesti, ennen kuin yrität uudelleen.

-  Laite on Windows 10 Home. Vain Windows 10 Pro, Education ja Enterprise SKUs voivat liittyä Azure Active Directoryyn.

Lisä resursseja ongelman ratkaisemiseen:
  
-  Käytä [Intune-vian määritys portaalia](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) yleisten rekisteröinti virheiden diagnosointiin ja ratkaisemiseen. Katso lisä tietoja [tästä asia kirjasta](https://docs.microsoft.com/intune/help-desk-operators) .

-  Tutustu näihin asia kirjoihin, jos haluat luettelon yleisistä virheistä, jotka estävät rekisteröinnin ja päätös lauselmien kunkin: [vian määritys opas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [vian määritys-asiak](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Opi rekisteröimään Windows-laitteet Microsoft Intunella](https://docs.microsoft.com/intune/windows-enroll).
