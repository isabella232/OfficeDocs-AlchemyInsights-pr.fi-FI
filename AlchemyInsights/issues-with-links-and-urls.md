---
title: Linkkien ja URL-osoitteiden ongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707879"
---
# <a name="issues-with-links-and-urls"></a>Linkkien ja URL-osoitteiden ongelmat

Uudelleenohjauksen URI-tunnus / vastauksen URL-osoite (kummatkin lausekkeet ovat vaihdettavissa) ovat Microsoftin käyttäjätietoympäristön käyttämiä URL-osoitteita, joita käytetään sovelluksen pyytämien tunnusten palauttamiseen. Lisätietoja näistä URL-osoitteista on seuraavissa artikkeleissa:

- [Todennusvirrat ja sovellusskenaariot](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – Tietoa uudelleenohjauksen URI-tunnuksista kunkin skenaarion **Sovelluksen rekisteröinti** -sivulla.
- [Uudelleenohjauksen URI-tunnusten / vastauksen URL-osoitteiden rajoitukset](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**En osaa rekisteröidä sovellukselleni oikeaa uudelleenohjauksen URI-tunnusta / vastauksen URL-osoitetta**

Kirjautuessasi sisään kehittämälläsi sovelluksella ja jos sisäänkirjautumisikkuna näyttää koodin **AADSTS50011: Pyynnössä määritetty vastauksen URL-osoite ei vastaa sovellukselle määritettyä vastauksen URL-osoitetta<your app ID>**. Sinun tulee lisätä sovelluksesi rekisteröintiin uudelleenohjauksen URI, jota koodisi käytti tunnuspyynnössä Microsoftin käyttäjätietoympäristöön.

Jos haluat lisätä vastauksen URL-osoitteen, siirry Azure-portaalissa **sovelluksen rekisteröinti** -sivun **Todennus**-välilehdelle ja lisää merkintä **Uudelleenohjauksen URI:t** -osioon. Syötettävä arvo määräytyy kehitettävän sovelluksen tyypin mukaan alla kuvatun mukaisesti:

- Yksisivuisissa sovelluksissa ja verkkosovelluksissa vastauksen URL-osoite on sovelluksen URL-osoite. Katso lisätietoja artikkelista [Yksisivuisen sovelluksen rekisteröinti](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) tai [Verkkosovelluksen rekisteröinti Azure-portaalilla](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Työpöytäsovelluksissa valittava arvo riippuu:
    - käyttöympäristöstä (MacOS eroaa Windowsista tai Linuxista)
    - tunnuksen hankintatavasta (vuorovaikutteisesti laitteen koodivirralla, integroidulla Windows-todennuksella [IWA] tai käyttäjänimellä/salasanalla).
    Lisätietoja on kohdassa [Työpöytäsovellukset – Sovelluksen rekisteröinti – Uudelleenohjauksen URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Mobiilisovelluksissa uudelleenohjauksen URI riippuu:
    - käyttöympäristöstä (iOS/Android/ANDREWP)
    - sovelluksen kehittämiseen käytetyistä tiedoista, kuten iOS:n nipputunnuksesta sekä paketin nimestä ja allekirjoituksen hajautuksesta Androidissa. Azure-portaalin sovelluksen rekisteröinti auttaa sinua. Lisätietoja on kohdassa [Käyttöympäristön määritys ja uudelleenohjauksen URI:t](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Web-ohjelmointirajapinnat ja jotkin hiljaiset tunnusten hankintatavat (IWA ja käyttäjänimi/salasana) eivät vaadi uudelleenohjauksen URI:ta.

**Olen kehittänyt oman verkkosovelluksen ja kun testaan käyttöönotettua sovellusta, saan vastauksen URL-osoitteen ristiriitaviestin**

Lisää uudelleenohjauksen URI kaikkiin sijainteihin, joissa käytät verkkosovellustasi. Lisätietoja on kohdassa [Verkkosovellusten rekisteröiminen Azure-portaalilla](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Lisää uudelleenohjauksen URI sijaintiin heti, kun olet ottanut sovelluksen käyttöön tässä sijainnissa.

**En pysty rekisteröimään riittävästi vastauksen URL-osoitteita**

Olet riippumaton ohjelmistokehitysyritys ja sinulla on yksi tai useampi uudelleenohjauksen URI asiakkaillesi. Haluat siirtää ADAL/Azure AD v1.0:stä MSAL:iin / Microsoftin käyttäjätietoympäristöön, ja olet saavuttanut [URL-osoitteiden enimmäismäärän](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Voit ratkaista ongelman [lisäämällä uudelleenohjauksen URI:t palvelun päänimiin](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals), jotka vastaavat kutakin asiakastasi.
