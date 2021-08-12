---
title: Sähköpostiviestien etsiminen ja poistaminen organisaatiossa
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948880"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Sähköpostiviestien etsiminen ja poistaminen organisaatiossa

Toimi seuraavasti:

1. Jos et ole yleinen järjestelmänvalvoja, sinun on lisättävä **eDiscovery Manager** -rooliryhmään tai yhteensopivuushaun hallintarooliin, jotta voit hakea **viestejä.** Jos haluat poistaa viestejä, sinun  täytyy liittyä Organisaation hallinta -rooliryhmään tai Haku- ja **poisto-hallintarooliin.** Näiden roolien käyttöoikeudet määritetään tietoturva- & [yhteensopivuuskeskuksessa.](https://protection.office.com)
2. [Etsi poistettava viesti](https://docs.microsoft.com/office365/securitycompliance/content-search) luomalla sisältöhaku.
3. [Näyttöyhteys tietoturva- & PowerShelliin.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Jos käytät monimenetelmäistä todentamista, katso seuraavat [ohjeet: Näyttöyhteys tietoturva- & Yhteensopivuuskeskuksen PowerShellin käyttäminen monimenetelmäisen todentamisen avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Poista viesti: poista viesti `New-ComplianceSearchAction` cmdlet-komentoa suoritamalla. Poistetut viestit siirretään käyttäjän Palautettavat-kansioon. Esimerkkikomento on kohdassa [Vaihe 3: Viestin poistaminen.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
