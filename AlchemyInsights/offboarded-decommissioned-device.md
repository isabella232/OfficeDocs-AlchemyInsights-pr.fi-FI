---
title: Ongelmia käytöstä poistetun tai käytöstä poistetun laitteen poistamisessa Laitevarastosta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 814301e9cd8197e62dcca68ab3bdde1618d210f73a744b53bb5af7b861eb02bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54076649"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Ongelmia käytöstä poistetun tai käytöstä poistetun laitteen poistamisessa Laitevarastosta

Microsoft Defender for Endpoint ei tällä hetkellä salli käytöstä poistetun tai käytöstä poistetun laitteen laitetietueen poistamista laiteluettelosta manuaalisesti.

Tietoturvasyistä laite säilyy portaalissa historiatietueena jopa 180 päivän ajan. Laitteen tiedot tyhjenee kuitenkin määritetyn säilytysajan mukaan.

**Huomautus:** Käytöstä poistettu tai käytöstä poistettu laite vaihtuu automaattisesti Passiivinen-tilaan **seitsemän** päivän kuluttua. Lisäksi laitteita, jotka eivät ole aktiivisia viimeisten 30 päivän aikana, ei sisällytetä tietoihin, jotka vastaavat organisaatiosi uhkien ja haavoittuvuuksien hallinta tai Microsoft Secure Score for Devices.
 
Jos et edelleenkään halua nähdä tiettyjä laitteita Laitevarasto-näkymässä, kokeile sijoittaa laitetunniste ja suodattaa pois käytöstä poistettu laite Laitevarasto-näkymässä.

Lisätietoja on seuraavissa artikkeleissa:

[Offboard-laitteet Microsoft Defender for Endpoint -palvelusta](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Valotuspisteet uhkien ja haavoittuvuuksien hallinta](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Korjaa huonot tunnistimet Microsoft Defender for Endpointissa](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Tunnisteiden tehokas käyttö (osa 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Tunnisteiden tehokas käyttö (osa 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Tunnisteiden tehokas käyttö (osa 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




