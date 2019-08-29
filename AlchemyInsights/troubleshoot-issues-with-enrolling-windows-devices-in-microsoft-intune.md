---
title: Windows-laitteiden ilmoittautumalla-ongelmien vian määritys Microsoft Intunessa
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665829"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Windows-laitteiden ilmoittautumalla-ongelmien vian määritys Microsoft Intunessa

Tarkista alla luetellut resurssit ongelman ratkaisemiseksi nyt.
  
Yleisiä virhe sanomia ja ratkaisu vaiheita:
  
 **Ohjelmistoa ei voi asentaa, 0x80cf4017:** Tilisi varmenne on vanhentunut. Lataa PC-asiakas ohjelmisto paketti uudelleen Intune admin Consolessa. Saat lisä tietoja tästä dokumentaatiosta.
  
 **Virhe koodi 0x801c0003:** Virhe voi ilmetä seuraavissa tilanteissa:
  
-  Käyttäjällä on enemmän laitteita, jotka on rekisteröity kuin laitteen rajoitus. Voit [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laitteen rajaa](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)näiden asia kirjojen avulla.

-  "Käyttäjät voivat liittyä laitteisiin Azure AD"-arvoksi on määritetty "ei mitään". Aseta se kaikille tai valitse käyttäjät. Saat lisä tietoja [tästä dokumentaatiosta](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Toinen käyttäjä on jo rekisteröitynyt laitteeseen. Jos näin on, Poista laite Azure Intune-konsolista tai rekisteröi laite manuaalisesti, ennen kuin yrität uudelleen.

-  Laite on Windows 10 Home. Vain Windows 10 Pro, koulutus ja yritys yksiköt voivat liittyä Azure Active Directoryyn.

Lisä resursseja ongelman ratkaisemiseen:
  
-  Käytä [Intune-vian määritys portaalia](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) yleisten rekisteröinti virheiden diagnosoimiseen ja ratkaisemiseen. Lisä tietoja [on tämän asia kirjan](https://docs.microsoft.com/intune/help-desk-operators) tarkastelussa.

-  Tarkastele näitä asia kirjoja, joissa on luettelo yleisistä virheistä, jotka estävät rekisteröintiä ja resoluutioita kuhunkin: [vian määritys opas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [vian etsintä doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Lue, miten voit rekisteröidä Windows-laitteita Microsoft Intune-kohteessa](https://docs.microsoft.com/intune/windows-enroll).
