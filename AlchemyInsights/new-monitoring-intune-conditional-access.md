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
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427426"
---
# <a name="monitor-intune-conditional-access"></a>Intunen ehdollisen käyttöoikeuden valvonta

Käyttäjät, joilla on ehdollinen käyttöoikeus, saavat sähköposti-ilmoituksen, jos he eivät täytä organisaatiosi käyttöoikeusvaatimuksia. Ratkaisua varten suosittelemme vähintään yhtä seuraavista ratkaisuista:

1. Jos laitteen oletetaan olevan rekisteröity, kehota käyttäjää menemään Yritysportaali-sovellukseen ja tarkistamaan, että se näkyy yritysportaalissa. Jos näin ei ole, käyttäjän on rekisteröittävä laite.
1. Valitse Azure-portaalissa **Intune-laitteen**  >  **yhteensopivuus.** 
1. Voit tarkastella laitteen yhteensopivuusraporttia sen varmistamiseksi, että käyttäjän laite on merkitty **yhteensopivaksi,** valitsemalla Seuraa-kohdassa Laitteen yhteensopivuus.
1. Valitse Azure-portaalissa **Intune-laitteen**  >  **yhteensopivuus.** Valitse **Hallinta-kohdassa** **Käytännöt.** Tarkista yhteensopivuuskäytäntöjen luettelosta, että profiili on määritetty käyttäjän laitteelle. Jos profiilia ei ole määritetty, Intune ei voi vahvistaa laitteen yhteensopivuustilaa.
1. Muokkaa käyttäjän ehdollisen käyttöoikeuden määritystä.
1. Siirry Azure-portaalissa **Intune-ehdollisen** käytön käytäntöihin, valitse käytäntö luettelosta ja valitse Käyttäjät  >    >   **ja ryhmät.**
1. Jos haluat kohdistaa tietyn käytännön jollekulle, lisää hänet **Sisällytä-luetteloon.** Jos haluat varmistaa, että henkilö jätetään pois käytännön ulkopuolelle, lisää hänet **Poissulkeminen-luetteloon.**

**Hyödyllisiä linkkejä:**

- [Laitteen yhteensopivuuden yleiskatsaus](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Varmenteiden myöntäjän vianmääritys](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Vianmäärityskäytäntö](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Intune-laitteen yhteensopivuuden valvonta](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Näistä ohjeista on hyötyä vain Azure Active Directory -ominaisuuden ehdollisen käyttöoikeuden vianmäärityksessä. On myös mahdollista asettaa karanteeniin laite, joka estää sähköpostin käytön Exchange-käytännön avulla. Lisätietoja Exchange-laitehallinnasta on [**täällä.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
