---
title: Laitteiden rekisteröintiongelmien Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981038"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Laitteiden rekisteröintiongelmien Windows Microsoft Intune

Ratkaise ongelma nyt alla lueteltujen resurssien avulla.
  
Yleisiä virhesanomia ja ratkaisuvaiheita:
  
 **Ohjelmistoa ei voi asentaa, 0x80cf4017:** Tilivarmenne on vanhentunut. Lataa PC-asiakasohjelman ohjelmistopaketti uudelleen Intune-hallintakonsolissa. Katso lisätietoja tästä ohjeista.
  
 **Virhekoodin 0x801c0003:** Virhe voi ilmetä seuraavissa tilanteissa:
  
-  Käyttäjällä on laiterajoitusta suurempia laitteita. Tarkista nämä [asiakirjat, jos haluat poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai muuttaa laitteen [rajoitusta.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  Käyttäjät voivat liittyä laitteisiin Azure AD:ssä -asetuksena on Ei mitään. Määritä se kaikille tai valitse käyttäjille. Katso [lisätietoja tästä](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) ohjeista.

-  Toinen käyttäjä on jo rekisteröinyt laitteen. Poista tällöin laite Azure Intune -konsolista tai poista laitteen tilaus manuaalisesti ennen uudelleen yrittämistä.

-  Laite on Windows 10 Home. Vain Windows 10 Pro, Education ja Enterprise -SKU:t voivat liittyä Azure Active Directory.

Lisäresursseja ongelman ratkaisemiseksi:
  
-  [Intunen vianmääritysportaalin avulla voit](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tehdä vianmäärityksen ja ratkaista yleisiä rekisteröintivirheitä. Katso [lisätietoja](https://docs.microsoft.com/intune/help-desk-operators) tästä asiakirjasta.

-  Tarkistamalla nämä asiakirjat saat luettelon yleisistä virheistä, jotka estävät kunkin tiedoston rekisteröinnin ja ratkaisut: [Vianmääritysopas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [Tiedoston vianmääritys.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Opi rekisteröimaan Windows laitteisiin Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
