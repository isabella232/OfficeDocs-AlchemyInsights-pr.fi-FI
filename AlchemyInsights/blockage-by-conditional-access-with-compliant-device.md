---
title: Ehdollinen käyttöoikeus estää minua yhteensopivalla laitteella
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035372"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Ehdollinen käyttöoikeus estää minua yhteensopivalla laitteella

**Erittäin suositellut työkalut**

- [Laitteen rekisteröinnin vianmääritystyökalu](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – kattava työkalu, joka auttaa vianmäärityksessä yleisimpiä laitteen rekisteröintiongelmia.
- [Test Device Registration Connectivity -komentosarja](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – työkalu, jonka avulla voidaan varmistaa, että laite voi käyttää järjestelmätilin laitteen rekisteröinnin päätepisteitä.
- [Azure AD Device Cleanup -komentosarja](https://github.com/mzmaili/AzureADDeviceCleanup) – työkalu, jonka avulla voit etsiä ja hallita ympäristösi staattisia laitteita.

Seuraavassa on joitakin yleisiä syitä, miksi ehdollinen käyttöoikeus saattaa epäonnistua  yhteensopivan laitteen kanssa tai miksi käyttäjät saattavat saada Sinut eivät pääse sinne tästä viestistä organisaatioresurssiin kirjautumispyynnön aikana.

1. **Laite ei ole pakollisessa laitteessa, jossa on MDM:**

Vahvista, että laite on rekisteröity hyväksyttyyn MDM-palveluun, kuten Intuneen, *ja että laite on merkitty yhteensopivaksi.* Lisätietoja Intunesta on tässä [asiakirjassa.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Lisätietoja laitteen yhteensopivuudesta ja Intunesta on Kohdassa Yhteensopivuuskäytännön avulla voit määrittää sääntöjä laitteille, joita [hallitset Intunella.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Jos sinulla on ongelmia laitteen rekisteröinnissä Intunen kanssa, etsi vianmääritystietoja microsoftin laitteen [rekisteröinnin vianmäärityksestä.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Jos haluat lisää Intune-tukea, luo tukipyyntö. Voit tehdä tämän [Intunen ohje- ja tukisivulla.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Laitetta ei ole liitetty organisaatioiden verkkoon:**

Jotta voit käyttää organisaation resursseja, laite on yhdistettynä organisaation verkkoon joko suoran yhteyden tai VPN-yhteyden kautta ja myös paikalliseen tai Azure Active Directoryyn. Jos haluat liittyä työlaitteeseen organisaation verkkoon, katso kohta Liity [työlaitteeseen organisaatiosi verkkoon.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Jos haluat rekisteröidä henkilökohtaisen/BYOD-laitteen, katso kohta [Henkilökohtaisen laitteen rekisteröiminen organisaatiosi verkkoon.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Voit tarkistaa, onko laite liitetty verkkoon, noudattamalla rekisteröityjen [](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) laitteiden ohjeita tai työlaitteita [täällä.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Voit ratkaista ongelman organisaation verkkoyhteydessä noudattamalla seuraavia ohjeita:

    1. Kirjaudu Windowsiin käyttämällä esimerkiksi työ- tai alain@contoso.com.
    2. Muodosta yhteys organisaatiosi verkkoon VPN- tai DirectAccess-yhteyden kautta.
    3. Kun olet muodostanut yhteyden, lukitse **laite painamalla näppäinyhdistelmää Windows-näppäin+L.**
    4. Poista laitteen lukitus käyttämällä työ- tai koulutiliä ja yritä sitten käyttää ongelmallista sovellusta tai palvelua uudelleen.

Jos näet Et pääse tänne **-virheilmoituksen** uudelleen, ongelma on todennäköisesti jossakin muualla.

3. **Käyttöjärjestelmää ei tueta:**

Varmista, että käytössäsi on käyttöjärjestelmän tuettu versio, mukaan lukien:

- **Windows-asiakasohjelma:** Windows 7 tai uudempi

- **Windows Server:** Windows Server 2008 R2 tai uudempi

- **macOS:** macOS X tai uudempi

- **Android ja iOS:** Android- ja iOS-mobiilikäyttöjärjestelmien uusin versio

4. **Selainta ei tueta:**

Alla on tuettuja selaimia. Windows 1703:n tai sitä uudempien versioiden Chrome-tuki edellyttää Windows 10 -tililaajennuksia. Edge 85+:ssä käyttäjän on kirjauduttava sisään, jotta laitteen yhteensopivuustiedot voidaan välittää oikein. Lisätietoja on [täällä.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1:** Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intunen hallittu selain, Safari
- **Android:** **Microsoft Edge:** Intunen hallittu selain, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Lisätietoja on **täällä:** Et voi saada sitä -sanoma ja [vianmääritysvaiheet.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
