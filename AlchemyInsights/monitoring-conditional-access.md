---
title: Ehdollisen käytön valvominen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366425"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Ehdollisen Exchange-yhteyden valvonta

Ehdolliseen käyttöön kohdistetut käyttäjät saavat ilmoitus Sähkö posti viestin, jos he eivät täytä organisaatiosi käyttö oikeus vaatimuksia. Ratkaisu on suositeltava vähintään yksi seuraavista ratkaisuista:

- Jos laitteen oletetaan olevan rekisteröity, kehota käyttäjää siirtymään yritys portaali-sovellukseen ja vahvistamaan, että se näkyy yritys portaalissa. Jos näin ei tapahdu, käyttäjän on rekisteröitävä laite.
- Valitse Azure-portaalissa Intune-> laite yhteensopivuus. Valitse näyttö-kohdassa laitteen yhteensopivuus. Tarkastele laitteesi yhteensopivuus raporttia varmistaaksesi, että käyttäjän laite on merkitty yhteensopivaksi.
- Valitse Azure-portaalissa Intune-> laite yhteensopivuus. Valitse hallinta-kohdassa käytännöt. Varmista yhteensopivuus käytäntöjen luettelosta, että profiili on määritetty käyttäjän laitteelle. Jos profiilia ei ole määritetty, Intune ei pysty vahvistamaan laitteen yhteensopivuus tilaa.
- Muokkaa käyttäjän ehdollisen käytön määritystä.

1. Valitse Azure-portaalissa **Intune**-  >  **ehdollisen käytön**  >  **käytännöt**.
2. Valitse luettelosta haluamasi käytännöt.
3. Valitse käyttäjät ja ryhmät.
4. Jos haluat kohdentaa tiettyyn käytäntöön jollekulle, lisää ne Sisällytä-luetteloon. Jos haluat varmistaa, että henkilö jätetään pois käytännöstä, Lisää hänet jätä pois-luetteloon.

Hyödyllisiä linkkejä:

[Laitteen yhteensopivuuden yleiskatsaus](https://docs.microsoft.com/intune/device-compliance-get-started)

[Varmenteiden myöntäjän vian määritys](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Vian määritys käytännöt](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Intune-laitteen yhteensopivuuden valvonta](https://docs.microsoft.com/intune/compliance-policy-monitor)

Huomautus: näistä vaiheista on hyötyä vain Azure Active Directory-ominaisuus ehdollisen käytön vian määrityksessä. On myös mahdollista eristää laite, joka estää sähkö postin käytön Exchange-käytännöllä. Lisä tietoja Exchange Device managementä on [täällä](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
