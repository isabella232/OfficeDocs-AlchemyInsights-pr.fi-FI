---
title: Ehdollisen käyttöoikeuden valvonta
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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708671"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Ehdollisen käyttöoikeuden valvonta Exchangessa

Käyttäjät, joilla on ehdollinen käyttöoikeus, saavat sähköposti-ilmoituksen, jos he eivät täytä organisaatiosi käyttöoikeusvaatimuksia. Ratkaisua varten suosittelemme vähintään yhtä seuraavista ratkaisuista:

- Jos laitteen oletetaan olevan rekisteröity, kehota käyttäjää menemään Yritysportaali-sovellukseen ja tarkistamaan, että se näkyy yritysportaalissa. Jos näin ei ole, käyttäjän tulisi rekisteröidä laite.
- Valitse Azure-portaalissa Intune > laitteen yhteensopivuus. Valitse Näyttö-kohdassa Laitteen yhteensopivuus. Tarkista laitteen yhteensopivuusraportista, että käyttäjän laite on merkitty yhteensopivaksi.
- Valitse Azure-portaalissa Intune > laitteen yhteensopivuus. Valitse Hallinta-kohdassa Käytännöt. Tarkista yhteensopivuuskäytäntöjen luettelosta, että profiili on määritetty käyttäjän laitteelle. Jos profiilia ei ole määritetty, Intune ei voi vahvistaa laitteen yhteensopivuustilaa.
- Muokkaa käyttäjän ehdollisen käyttöoikeuden määritystä.

1. Valitse Azure-portaalissa   >  **Intune-ehdollisen käytön**  >  **käytännöt.**
2. Valitse käytäntö luettelosta.
3. Valitse Käyttäjät ja ryhmät.
4. Jos haluat kohdistaa tietyn käytännön jollekulle, lisää hänet Sisällytä-luetteloon. Jos haluat varmistaa, että henkilö jätetään pois käytännön ulkopuolelle, lisää hänet Poissulkeminen-luetteloon.

Hyödyllisiä linkkejä:

[Laitteen yhteensopivuuden yleiskatsaus](https://docs.microsoft.com/intune/device-compliance-get-started)

[Varmenteiden myöntäjän vianmääritys](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Vianmäärityskäytäntö](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Intune-laitteen yhteensopivuuden valvonta](https://docs.microsoft.com/intune/compliance-policy-monitor)

Huomautus: näistä ohjeista on hyötyä vain Azure Active Directory -ominaisuuden ehdollisen käyttöoikeuden vianmäärityksessä. On myös mahdollista asettaa karanteeniin laite, joka estää sähköpostin käytön Exchange-käytännön avulla. Lisätietoja Exchange-laitehallinnasta on [täällä]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
