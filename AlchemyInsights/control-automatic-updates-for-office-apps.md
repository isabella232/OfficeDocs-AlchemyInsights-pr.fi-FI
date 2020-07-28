---
title: Office-sovellusten automaattisten päivitysten hallinta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439331"
---
# <a name="control-automatic-updates-for-office-apps"></a>Office-sovellusten automaattisten päivitysten hallinta

Oletusarvon mukaan Office-sovellusten päivitykset ladataan automaattisesti ja otetaan käyttöön taustalla ilman käyttäjän toimia. Järjestelmänvalvojat voivat kuitenkin hallita päivitysten asennusta Office Update -asetusten avulla. Päivitysasetusten avulla järjestelmänvalvojat voivat ottaa automaattiset päivitykset käyttöön tai poistaa ne käytöstä, näyttää tai piilottaa **Päivitä nyt** -painikkeen Officessa, asettaa päivityksen määräajat ja paljon muuta. Lisätietoja on seuraavissa ohjeissa:

- [Officen päivitysasetusten määrittäminen](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Officen automaattinen päivitys ei ole käytössä](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Officen päivitystavan määrittäminen asennuksen jälkeen](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Voit tarkistaa asiakastietokoneeseen käytetyt päivitysasetukset seuraavasti:

1. Auki Arkisto Julkaisija luona astuva jotta **Alku**  >  **Ajelu**  >  **holhoojahallitus**.
2. Siirry seuraavaan sijaintiin ja tarkista Office Update -asetukset:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\\\-kansio  
    b. ClickToRun\Configuration (ValitseToRun\Configuration)

**Huomautus**  Jos OfficeMgmtCOM-avain on määritetty, **Office**  >  **Office-tilin**  >  **Office-päivitykset**-kohdassa saattaa näkyä Päivitykset, joita järjestelmänvalvoja hallitsee. Lisätietoja on [ohjeaiheessa Microsoft 365 -sovellusten päivitysten hallinta Microsoft Endpoint Configuration Managerin avulla](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  