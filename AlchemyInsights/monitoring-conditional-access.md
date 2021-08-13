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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975098"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Ehdollisen käyttöoikeuden valvonta Exchange

Käyttäjät, joilla on ehdollinen käyttöoikeus, saavat sähköposti-ilmoituksen, jos he eivät täytä organisaatiosi käyttöoikeusvaatimuksia. Ratkaisua varten on suositeltavaa käyttää vähintään yhtä seuraavista ratkaisuista:

- Jos laitteen oletetaan olevan rekisteröity, kehota käyttäjää menemään Yritysportaali ja tarkistamaan, että se näkyy Yritysportaali. Jos näin ei ole, käyttäjän tulisi rekisteröidä laite.
- Valitse Azure-portaalissa Intune > laitteen yhteensopivuus. Valitse Näyttö-kohdassa Laitteen yhteensopivuus. Tarkista laitteen yhteensopivuusraportista, että käyttäjän laite on merkitty yhteensopivaksi.
- Valitse Azure-portaalissa Intune > laitteen yhteensopivuus. Valitse Hallinta-kohdassa Käytännöt. Tarkista yhteensopivuuskäytäntöjen luettelosta, että profiili on määritetty käyttäjän laitteelle. Jos profiilia ei ole määritetty, Intune ei voi vahvistaa laitteen yhteensopivuustilaa.
- Muokkaa käyttäjän ehdollisen käyttöoikeuden määritystä.

1. Valitse Azure-portaalissa **Intune Conditional** access Policies  >  **(Intune-ehdollisen käyttöoikeuden**  >  **käytännöt).**
2. Valitse käytäntö luettelosta.
3. Valitse Käyttäjät ja ryhmät.
4. Jos haluat kohdistaa tietyn käytännön jollekulle, lisää hänet Sisällytä-luetteloon. Jos haluat varmistaa, että henkilö jätetään pois käytännön perusteella, lisää hänet Jätä pois -luetteloon.

Hyödyllisiä linkkejä:

[Laitteen yhteensopivuuden yleiskatsaus](https://docs.microsoft.com/intune/device-compliance-get-started)

[Varmenteiden myöntäjän vianmääritys](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Vianmäärityskäytäntö](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Intune-laitteen yhteensopivuuden valvonta](https://docs.microsoft.com/intune/compliance-policy-monitor)

Huomautus: nämä vaiheet ovat hyödyllisiä vain ehdollisen Azure Active Directory vianmäärityksessä. Sähköpostin käytön estävät laitteet voidaan asettaa karanteeniin myös Exchange mukaisesti. Lisätietoja laitteiden Exchange löytyy [tästä]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
