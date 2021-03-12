---
title: OIDC-pohjaisten saumattomien kertakirjautumisongelmien vianmääritys
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
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745020"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>OIDC-pohjaisten saumattomien kertakirjautumisongelmien vianmääritys

- Lisätietoja OIDC-pohjaisen sovelluksen lisäästä Azure-vuokraajaan [on pika-aloitustoiminnossa: OIDC-pohjaisen](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)kertakirjautumisen (SSO) asentaminen Azure Active Directory (Azure AD) -vuokraajan sovellukseen.
- Lisätietoja sovelluksista, jotka käyttävät OpenID Connect -standardia kertakirjaamiseksi, on kohdassa [Tietoja OIDC-pohjaista kertakirjaaminen -sovelluksesta.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Jos haluat lisätietoja siitä, että lähetät ja käsittelet suoraan HTTP-pyyntöjä tai käytät kolmannen osapuolen avoimen lähdekoodin kirjastoa avoimen lähdekoodin kirjaston käyttämisen sijaan, tutustu Microsoftin käyttäjätietoympäristön [OAuth 2.0-](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)ja OpenID Connect -protokolliin.

**Protokollat**

1. [Microsoftin](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) tunnistetietoympäristö ja implisiittinen grant flow - Implisiittisen myöntämisen ominaisuuden määrittävä ominaisuus on se, että tunnukset (tunnustunnukset tai käyttöoikeustietueet) palautetaan suoraan /authorize-päätepisteistä /token-päätepisteen sijaan. Tätä käytetään usein osana valtuutuskoodin kulkua, jota kutsutaan yhdistelmävuoksi – tunnustietueen noutamisessa /authorize-pyynnöstä ja **valtuutuskoodista.** Tässä artikkelissa kerrotaan, miten voit ohjelmoida suoraan sovelluksesi protokollaa vastaan pyytääksesi tunnuksia Azure AD:ltä.
2. [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - The OAuth 2.0 authorization code grant can be used in apps that are installed on a device to gain to access to protected resources, such as web APIs. Käyttämällä Microsoftin tunnistetietoympäristön OAuth 2.0 -käyttöönottoa voit lisätä kirjautumis- ja **ohjelmointirajapinnan käyttöomme mobiili- ja työpöytäsovelluksiasi.** Tässä artikkelissa kerrotaan, miten voit ohjelmoida suoraan protokollaa vasten sovelluksessa millä tahansa kielellä.
3. [Microsoftin käyttäjätietoympäristö ja OpenID Connect -protokolla](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – Kun käytät Microsoftin käyttäjätietoympäristön OpenID Connectin käyttöönottoa, voit lisätä sovellusten kirjautumis- ja ohjelmointirajapinnan käyttöoikeudet. Tässä artikkelissa kerrotaan, miten voit tehdä tämän kielestä riippumatta ja miten HTTP-viestejä lähetetään ja vastaanotaan ilman microsoftin avoimen **lähdekoodin kirjastoja.**
4. Microsoftin tunnistetietoympäristö ja [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -asiakastietojen työnkulku – Voit käyttää verkossa isännöityjä resursseja käyttämällä RFC 6749:ssä määritettyä OAuth 2.0 -asiakastunnusten myöntämistä, jota kutsutaan joskus kaksikirjaimiseksi **OAuth-ohjelmaksi.** Tämäntyyppistä tukea käytetään yleisesti palvelinten välillä käytettynä vuorovaikutuksessa, joka on suoritettava taustalla ilman välitöntä vuorovaikutusta käyttäjän kanssa. Tällaisia sovelluksia kutsutaan usein **daemone- tai** **palvelutileille.** Tässä artikkelissa kerrotaan, miten voit ohjelmoida suoraan protokollaa vasten sovelluksessasi.
