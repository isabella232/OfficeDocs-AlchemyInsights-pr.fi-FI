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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746432"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Sähköpostiviestien etsiminen ja poistaminen organisaatiossa

Toimi seuraavasti:

1. Jos et ole yleinen järjestelmänvalvoja, tilisi on lisättävä **eDiscovery Managerin** rooliryhmään tai yhteensopivuushaun **hallintarooliin,** jotta voit hakea viestejä. Jos haluat poistaa viestejä, sinun täytyy liittyä Organisaation hallinta -rooliryhmään **tai** haku- ja **poisto-hallintarooliin.** Näiden roolien käyttöoikeudet määritetään tietoturva- & [yhteensopivuuskeskuksessa.](https://protection.office.com)
2. [Etsi poistettava viesti](https://docs.microsoft.com/office365/securitycompliance/content-search) luomalla sisältöhaku.
3. [Muodosta yhteys tietoturva- & PowerShelliin.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Jos käytät monimenetelmäistä todentamista, katso seuraavat ohjeet: Muodosta [yhteys tietoturva- & PowerShelliin monimenetelmäisen todentamisen avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Poista viesti: poista viesti `New-ComplianceSearchAction` suorita cmdlet-komento. Poistetut viestit siirretään käyttäjän Palautettavat-kansioon. Esimerkkikomento, katso [vaihe 3: Viestin poistaminen.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
