---
title: Ilmaisimet eivät toimi Edge-selaimessa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: ff7a2ee4c97c579422c7679c461f6fb288a9235ff9056be1c56e80b1d6379723
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887437"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Ilmaisimet eivät toimi Edge-selaimessa

Kun olet luonut ilmaisimen, Edge (Smartscreen) ei ota sitä mukaan. Lisätietoja on kohdassa ILMAISIMIEN [LUOMINEN IP-osoitteille ja URL-osoitteille/toimialueille.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Vaihe 1: Varmista seuraavat asiat

- Varmista, että ilmaisin on oikein (IP-/URL-osoitteessa ei ole kirjoitusvirheitä, oikea toiminto, oikeat RBAC-ryhmät).
- Odota vähintään 2 tuntia ilmaisimen luomisen jälkeen, jotta mahdolliset viiveet otetaan huomioon.
- Varmista, että järjestelmät onboarded Microsoft Defender for Endpointiin.
- Varmista, että järjestelmät voivat viestiä pilvipalvelun kanssa.
- Varmista testisivustosta, että Smartscreen on otettu käyttöön ja [tavoitettavissa.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>Vaihe 2: Mahdollisen ongelman vianmääritys

- Varmista, että asiakas täyttää vaatimukset. Lisätietoja on kohdassa [ILMAISIMIEN LUOMINEN IP-osoitteille ja URL-osoitteille/toimialueille.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Varmista, että käytössäsi on Edge-selaimen uusin versio. Lisätietoja uusimmasta versiosta on kohdassa [Käytössäsi Microsoft Edge version etsiminen.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Käynnistä Edge-selain uudelleen.
- Siirry sivustoon, johon olet lisännyt ilmaisimen. Jos sivusto ei näy odotetulla tavalla, jatka vaiheeseen 3. 

## <a name="step-3-collect-data"></a>Vaihe 3: Tietojen kerääminen

- Kerää **MDEClientAnalyzerin** diagnostiikkatietoja. Katso ohjeet ohjeista [Onboarding machines to Microsoft Defender for Endpoint (Onboarding Machinesin ja Microsoft Defender for Endpointin ongelmat).](issues-with-onboarding-machines.md)
- Jos olet tutustunut Fiddler-seurantatietojen asentamiseen ja keräämiseen, katso [Telerik Fiddler](http://www.telerik.com/fiddler).
- Jos haluat ohjeita Microsoft-tuesta, avaa tukipyyntö valitsemalla alla oleva Tuki-kuvake.
