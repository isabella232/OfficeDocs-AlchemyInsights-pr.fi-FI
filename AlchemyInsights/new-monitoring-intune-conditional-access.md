---
title: Intunen ehdollisen käyttöoikeuden valvonta
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327554"
---
# <a name="monitor-intune-conditional-access"></a>Intunen ehdollisen käyttöoikeuden valvonta

Käyttäjät, joilla on ehdollinen käyttöoikeus, saavat sähköposti-ilmoituksen, jos he eivät täytä organisaatiosi käyttöoikeusvaatimuksia. Ratkaisua varten suosittelemme vähintään yhtä seuraavista ratkaisuista:

1. Jos laitteen oletetaan olevan rekisteröity, kehota käyttäjää menemään Yritysportaali-sovellukseen ja tarkistamaan, että se näkyy Yritysportaali. Jos näin ei ole, käyttäjän on rekisteröittävä laite.
1. Valitse Azure-portaalissa **Intune** Device compliance  >  **(Intune-laitteen yhteensopivuus).** 
1. Voit tarkistaa laitteen yhteensopivuusraportin ja varmistaa, että käyttäjän laite on merkitty yhteensopivaksi valitsemalla Näyttö **-kohdassa** **Laitteen yhteensopivuus**.
1. Valitse Azure-portaalissa **Intune** Device compliance  >  **(Intune-laitteen yhteensopivuus).** Valitse **Hallinta-kohdassa** **Käytännöt**. Tarkista yhteensopivuuskäytäntöjen luettelosta, että profiili on määritetty käyttäjän laitteelle. Jos profiilia ei ole määritetty, Intune ei voi vahvistaa laitteen yhteensopivuustilaa.
1. Muokkaa käyttäjän ehdollisen käyttöoikeuden määritystä.
1. Siirry Azure-portaalissa **kohtaan Intune**  >  Conditional access Policies **(Intune-ehdollisen** käyttöoikeuden käytännöt), valitse käytäntö  >  luettelosta ja valitse Käyttäjät **ja ryhmät**.
1. Jos haluat kohdistaa tietyn käytännön jollekulle, lisää hänet **Sisällytä-luetteloon.** Jos haluat varmistaa, että henkilö jätetään pois käytännön perusteella, lisää hänet Jätä **pois -luetteloon.**

**Hyödyllisiä linkkejä:**

- [Laitteen yhteensopivuuden yleiskatsaus](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Varmenteiden myöntäjän vianmääritys](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Vianmäärityskäytäntö](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Intune-laitteen yhteensopivuuden valvonta](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Huomautus:** Nämä vaiheet ovat hyödyllisiä vain ehdollisen Azure Active Directory vianmäärityksessä. Sähköpostin käytön estävät laitteet voidaan asettaa karanteeniin myös Exchange mukaisesti. Lisätietoja laitteiden Exchange löydät [**täältä**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
