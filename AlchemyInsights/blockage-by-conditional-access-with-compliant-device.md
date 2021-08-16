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
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019145"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Ehdollinen käyttöoikeus estää minua yhteensopivalla laitteella

**Erittäin suositellut työkalut**

- [Laitteen rekisteröinnin vianmääritystyökalu](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – kattava työkalu, joka auttaa laitteen yleisimmät rekisteröintiongelmat vianmäärityksessä.
- [Test Device Registration Connectivity -komentosarja](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – työkalu, jonka avulla voidaan varmistaa, että laite voi käyttää järjestelmätilin Device Registration -päätepisteitä.
- [Azure AD Device Cleanup -komentosarja](https://github.com/mzmaili/AzureADDeviceCleanup) – työkalu, jonka avulla voit etsiä ja hallita ympäristön staattisia laitteita.

Seuraavassa on joitakin yleisiä syitä, miksi ehdollinen käyttöoikeus saattaa epäonnistua  yhteensopivan laitteen vuoksi tai miksi käyttäjät saattavat saada Et voi tästä eteenpäin saada tätä viestiä organisaatioresurssille kirjautumispyynnön aikana.

1. **Laite ei ole pakollisessa laitetilassa, jossa on MDM:**

Vahvista, että laitteeseen on rekisteröity hyväksytty MDM-palveluntarjoaja, kuten Intune, ja *merkitty yhteensopivaksi.* Lisätietoja Intunesta on tässä [asiakirjassa.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Lisätietoja laitteen yhteensopivuudesta ja Intunesta on kohdassa Yhteensopivuuskäytännön käyttäminen sääntöjä varten [hallittavissa laitteissa Intunella.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Jos sinulla on ongelmia laitteen rekisteröinnissä Intunen kanssa, katso vianmääritysohjeita kohdassa [Laitteen rekisteröinnin vianmääritys Microsoftissa.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Jos haluat lisää Intune-tukea, luo tukipyyntö. Siirry Intunen Ohje ja [tuki -sivulle.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Laitetta ei ole liitetty organisaatioiden verkkoon:**

Jotta voit käyttää organisaation resursseja, laitteen on oltava yhteydessä organisaation verkkoon joko suoran yhteyden kautta tai VPN-yhteyden kautta ja oltava yhteydessä myös paikalliseen verkkoon tai Azure Active Directory. Jos haluat liittyä työlaitteeseen organisaation verkkoon, katso [kohta Työlaitteen liittyminen organisaatiosi verkkoon.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Jos haluat rekisteröidä henkilökohtaisen/BYOD-laitteen, katso rekisteröi henkilökohtainen laitteesi [organisaatiosi verkkoon.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Voit tarkistaa, onko laite liitetty verkkoon, noudattamalla rekisteröityjen [](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) laitteiden ohjeita täällä tai [työlaitteilla.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Jos haluat ratkaista ongelman organisaation verkkoyhteydessä, noudata seuraavia ohjeita:

    1. Kirjaudu sisään Windows käyttämällä esimerkiksi työ- tai alain@contoso.com.
    2. Näyttöyhteys yhteyden organisaatiosi verkkoon VPN-yhteyden tai DirectAccessin kautta.
    3. Kun yhteys on muodostettu, lukitse **Windows painamalla näppäinyhdistelmää Windows -näppäin+L.**
    4. Poista laitteen lukitus käyttämällä työ- tai koulutiliä ja yritä sitten käyttää ongelmallista sovellusta tai palvelua uudelleen.

Jos näet Et **pääse siihen tästä -virheilmoituksen** uudelleen, ongelma on todennäköisesti jossakin muualla.

3. **Käyttöjärjestelmää ei tueta:**

Varmista, että käytössäsi on käyttöjärjestelmän tuettu versio, mukaan lukien:

- **Windows-asiakasohjelma:** Windows 7 tai uudempi versio

- **Windows Server:** Windows Server 2008 R2 tai uudempi

- **macOS:** macOS X tai uudempi

- **Android ja iOS:** Android- ja iOS-mobiilikäyttöjärjestelmien uusimmat versiot

4. **Selainta ei tueta:**

Etsi tuetut selaimet alla. Jos sinulla on Chrome-tuki Windows 1703-versiossa tai sitä uudemmassa versiossa, Windows 10 edellyttää Tilit-laajennusta. Edge 85+:ssa käyttäjän on kirjauduttava sisään, jotta hän voi välittää laitteen yhteensopivuustiedot oikein. Lisätietoja on [täällä.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10:** Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS:** Microsoft Edge, Intune Managed Browser, Safari
- **Android:** **Microsoft Edge**: Intune Managed Browser, Chrome
- **Windows Phone:** Microsoft Edge Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016:** Internet Explorer
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2:** Internet Explorer
- **macOS:** Chrome, Safari

Lisätietoja on tässä **kohdassa Et voi käyttää viestiä** ja [vianmääritysohjeita.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
