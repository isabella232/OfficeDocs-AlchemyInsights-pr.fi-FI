---
title: Linkkeihin ja URL-osoitteisiin liittyvät ongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974464"
---
# <a name="issues-with-links-and-urls"></a>Linkkeihin ja URL-osoitteisiin liittyvät ongelmat

Redirect URI/reply URLLs (both expressions are interchangeable) are the URLLs used by the Microsoft identity platform to return app-requested tokens. Lisätietoja näistä URL-osoitteista on seuraavissa artikkeleissa:

- [Todennusvirrat ja sovellusskenaariot](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – Tietoja uudelleenohjauksen URL-osoitteista sovelluksen **rekisteröintisivulla** kullekin skenaariolle.
- [Uudelleenohjauksen URI-osoite/ vastauksen URL-osoitteen rajoitukset](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**En tiedä, miten rekisteröityä oikea uudelleenohjauksen URI / vastauksen URL-osoite sovellukselle**

Kun kirjaudut sisään kehittämälläsi sovelluksella, jos kirjautumisvalintaikkunassa näkyy **AADSTS50011: <your app ID>** Pyynnössä määritetty vastauksen URL-osoite ei vastaa sovellukselle määritettyjä vastaus-URL-osoitteita, sinun on lisättävä sovelluksen rekisteröintiin uudelleenohjauksen URI, jota koodisi käytti tunnuspyynnössä Microsoftin käyttäjätietoympäristöön.

Jos haluat lisätä vastauksen URL-osoitteen,  siirry Azure-portaalin sovelluksen rekisteröintisivun Todennus-välilehteen ja lisää merkintä Uudelleenohjauksen **URL-osoitteet -osaan.**  Uudelleenohjauksen URL-osoitteet kirjoitetaan (verkko tai mobiili/työpöytä). Syöttyvät arvot määräytyvät sen mukaan, minkä tyyppistä sovellusta olet rakentamassa, kuten alla on kuvattu:

- Yksisivuisissa sovelluksissa ja verkkosovelluksissa vastauksen URL-osoite on sovelluksesi URL-osoite. Katso Yhden sivun sovelluksen rekisteröinti tai [Verkkosovelluksen rekisteröiminen Azure-portaalin avulla](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal) [](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri)
- Työpöytäsovelluksissa valittava arvo määräytyy:
    - käyttöympäristö (MacOS eroaa Windowsista tai Linuxista)
    - tapa, jolla hankit tunnuksen (vuorovaikutteisesti laitekoodin työnkulun, integroidun Windows-todennuksen [IWA] tai käyttäjänimen/salasanan avulla).
    Lisätietoja on kohdassa [Työpöytäsovellukset – sovelluksen rekisteröinti – URi:n uudelleenohjaus](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Mobiilisovelluksissa uudelleenohjauksen URI-arvo määräytyy:
    - käyttöympäristö (iOS/Android/UWP)
    - tietoja, joita käytetään sovelluksen rakentamiseen, kuten pakettitunnus iOS:ssä, ja paketin nimi ja allekirjoituksen hash Androidissa Azure-portaalisovelluksen rekisteröinti auttavat sinua. Lisätietoja on kohdassa [Käyttöympäristön määritys ja uudelleenohjaus- URIs.](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)

> [!NOTE]
> Verkkorajapintojen ja joidenkin tunnusten (IWA ja käyttäjänimi/salasana) äänettömien hankintatapoihin ei tarvita uudelleenohjauksen URI-tunnusta.

**Olen ottanut verkkosovelluksen käyttöön, ja kun testaan käyttöön otettua sovellusta, näyttöön tulee vastauksen URL-osoitteen ristiriitasanoma**

Lisää uudelleenohjauksen URL-osoitteet kaikkiin sijainneihin, joissa otat verkkosovelluksen käyttöön. Lisätietoja on kohdassa [Verkkosovellussovelluksen rekisteröiminen Azure-portaalin avulla.](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)

> [!NOTE]
> Lisää uudelleenohjauksen URI-osoite sijaintiin heti, kun olet ottanut sovelluksen käyttöön tässä sijainnissa.

**En pysty rekisteröimään tarpeeksi vastaus-URL-osoitteita**

Olet isv ja sinulla on yksi tai useampi uudelleenohjauksen URIs jokaiselle asiakkaallesi. Haluat siirtää ADAL/Azure AD v1.0:sta MSAL:sta tai Microsoftin käyttäjätietoympäristöön ja voit käyttää uudelleenohjaus- [URIstojen enimmäismäärää.](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris) Voit ratkaista ongelman lisäämällä [uudelleenohjauksen URL-osoitteet palvelun päätoiminnille,](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) jotka vastaavat kutakin asiakastasi.
