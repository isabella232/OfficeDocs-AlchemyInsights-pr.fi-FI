---
title: OIDC-pohjaisten Saumattoman kertakirjautumisen ongelmien vianmääritys
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105775"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>OIDC-pohjaisten Saumattoman kertakirjautumisen ongelmien vianmääritys

- Lisätietoja OIDC-pohjaisen sovelluksen lisäästä Azure-vuokraajaan on kohdassa [Pika-aloitus: OIDC-pohjaisen](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)kertakirjautumisen (SSO) luominen Azure Active Directory (Azure AD) -vuokraajan sovellukselle.
- Lisätietoja sovelluksista, jotka käyttävät OpenID-Näyttöyhteys kertakirjautumista, on kohdassa [Tietoja OIDC-pohjaista kertakirjaaminen -sovelluksesta.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Jos haluat lisätietoja siitä, että kirjoitat koodin lähettämällä ja käsitellessäsi HTTP-pyyntöjä suoraan tai käyttämällä kolmannen osapuolen avoimen lähdekoodin kirjastoa avoimen lähdekoodin kirjaston sijaan, katso [OAuth 2.0 ja OpenID Näyttöyhteys -protokollia Microsoftin käyttäjätietoympäristö.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)

**Protokollat**

1. Microsoftin käyttäjätietoympäristö ja [implisiittinen](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) grant flow – Implisiittisen myöntämisen ominaisuuden määrittelevä ominaisuus on se, että tunnukset (tunnustunnukset tai käyttöoikeustunnukset) palautetaan suoraan /authorize-päätepisteistä /token-päätepisteen sijaan. Tätä käytetään usein osana valtuutuskoodin kulkua yhdistelmävuossa , joka noutaa /authorize-pyynnössä olevan tunnustietueen ja **valtuutuskoodin.** Tässä artikkelissa kerrotaan, miten voit ohjelmoida suoraan sovelluksesi protokollaa vastaan ja pyytää tunnuksia Azure AD:stä.
2. Microsoftin käyttäjätietoympäristö ja [OAuth 2.0-valtuutuskoodin](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) kulku – OAuth 2.0 -valtuutuskoodin grant-käyttöoikeuksien myöntämistä voidaan käyttää sovelluksissa, jotka on asennettu laitteeseen ja jotka saavat pääsyn suojattuihin resursseihin, kuten verkkorajapintojen. Käyttämällä Microsoftin käyttäjätietoympäristö OAuth 2.0:n käyttöönottoa voit lisätä kirjautumis- ja ohjelmointirajapinnan käytön **mobiili- ja työpöytäsovelluksiin.** Tässä artikkelissa kerrotaan, miten voit ohjelmoida suoraan protokollaa vastaan sovelluksessa millä tahansa kielellä.
3. [Microsoftin käyttäjätietoympäristö OpenID Näyttöyhteys -protokolla](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – Kun käytät Microsoftin käyttäjätietoympäristö:n OpenID Näyttöyhteys -käyttöönottoa, voit lisätä sovellusten kirjautumis- ja ohjelmointirajapintakäyttöliittymän. Tässä artikkelissa kerrotaan, miten voit tehdä tämän kielestä riippumatta ja miten HTTP-viestit lähetetään ja vastaanotaan ilman Microsoftin avoimen **lähdekoodin kirjastoja.**
4. Microsoftin käyttäjätietoympäristö ja [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -asiakasohjelman tunnistetiedot – Voit käyttää verkossa isännöityjä resursseja käyttämällä RFC 6749:ssä määritettyä OAuth 2.0 -asiakastunnusten myöntämistä, jota kutsutaan joskus kaksikirjaimiseksi **OAuth-ohjelmaksi,** ja käyttää verkossa isännöityjä resursseja sovelluksen käyttäjätietojen avulla. Tätä grant-tyyppiä käytetään usein palvelinten välillä käytettynä vuorovaikutuksessa taustalla ilman, että käyttäjän kanssa toimitaan välittömästi. Tällaisia sovelluksia kutsutaan usein nimellä **daemons tai** **palvelutilejä.** Tässä artikkelissa kerrotaan, miten voit ohjelmoida suoraan sovelluksesi protokollaa vastaan.
