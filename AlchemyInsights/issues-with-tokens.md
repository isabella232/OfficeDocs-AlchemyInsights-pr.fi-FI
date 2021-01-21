---
title: Tunnuksiin liittyvät ongelmat
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
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916844"
---
# <a name="issues-with-tokens"></a>Tunnuksiin liittyvät ongelmat

Voit hallita tunnuksiin liittyviä ongelmia seuraavasti:

1. Voit määrittää Microsoftin tunnistetietoympäristön myöntämän käyttö-, tunnus- tai SAML-tunnuksen elinkaaren. Voit määrittää tunnuksen elinkaaren kaikille organisaation sovelluksille, usean vuokraajan (usean organisaation) sovellukselle tai tietylle organisaation palvelun päätasolle. Lisätietoja on kohdassa Määritettävissä [olevat tunnusten elinkaarit Microsoftin käyttäjätietoympäristössä (esikatselu).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
2. Käyttöoikeustietueiden avulla asiakasohjelmat voivat soittaa suojatuille verkkorajapinnoille turvallisesti, ja verkkorajapinnat käyttävät niitä todennuksen ja valtuutuksen suorittamiseen. OAuth-määrityksen mukaisesti käyttöoikeustietueet ovat läpinäkymättömiä merkkijonoja, joissa ei ole määritettyä muotoa. Jotkin tunnistetietojen toimittajat käyttävät GUID-tunnuksia ja toiset salattuja blob-koodeja. Microsoftin tunnistetietoympäristö käyttää erilaisia käyttöoikeustietueen muotoja sen mukaan, mikä ohjelmointirajapinta on määrityksessä, joka hyväksyy tunnuksen. Lisätietoja siitä, miten ohjelmointirajapinta voi vahvistaa ja käyttää käyttöoikeustietueen vaatimuksia, on [Microsoftin käyttäjätietoympäristön käyttöoikeustietueissa.](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint)
3. Microsoftin todentamiskirjasto (MSAL) tukee useita todennusvirtoja käytettäväksi eri sovellusskenaarioissa. Lisätietoja on kohdassa [Todennusvirrat.](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes)
4. OAuth 2.0 -valtuutuskoodia voidaan käyttää sovelluksiin, jotka on asennettu laitteeseen, jotta he voivat käyttää suojattuja resursseja, kuten verkkorajapinnuksia. Käyttämällä Microsoftin tunnistetietoympäristön OAuth 2.0 -käyttöönottoa voit lisätä kirjautumis- ja ohjelmointirajapinnan käyttöomme mobiili- ja työpöytäsovelluksiasi. Katso [Microsoftin käyttäjätietoympäristöstä ja OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) :n valtuutuskoodivirrasta, miten voit ohjelmoida suoraan sovelluksesi protokollaa vastaan millä tahansa kielellä.
5. OpenID Connect (OIDC) on OAuth 2.0:een luotu todennusprotokolla, jonka avulla voit kirjautua turvallisesti sovellukseen. Kun käytät Microsoftin tunnistetietoympäristön päätepisteen OpenID Connectin käyttöönottoa, voit lisätä sovellusten kirjautumis- ja ohjelmointirajapinnan käyttöoikeudet. [Microsoftin käyttäjätietoympäristö ja OpenID Connect -protokolla](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) osoittavat, miten tämä voidaan tehdä kielestä riippumatta ja miten HTTP-viestejä lähetetään ja vastaanotaan ilman microsoftin avoimen lähdekoodin kirjastoja.
    - UserInfo-päätepiste on osa OIDC-standardia, jonka tarkoituksena on palauttaa todennutta käyttäjää koskevat vaateet. Lisätietoja on kohdassa [Microsoftin käyttäjätietoympäristön UserInfo-päätepiste.](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead)
    - Verkkorajapinnan kutsuminen verkkosovelluksessa Azure AD:n ja [OpenID Connectin](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) avulla näyttää, miten voit luoda Azure AD:tä käyttävän MVC-verkkosovelluksen OpenID Connect -protokollan avulla ja soittaa sitten verkkorajapintaan kirjautuneen käyttäjän tunnistetietojen alle käyttämällä OAuth 2.0:n kautta hankittuja tunnuksia. Tässä esimerkissä käytetään OpenID Connect ASP .Net OWIN -keskiohjelmistoa ja ADAL .Net -yhteyttä.
6. [Määritä sovellus, joka näyttää verkkorajapinnan](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) . Tässä pika-aloitussovelluksessa rekisteröit verkkorajapinnan Microsoftin käyttäjätietoympäristöön ja paljastat sen asiakassovelluksissa lisäämällä esimerkkialueen. Rekisteröimällä verkkorajapintasi ja altistamalla sen laajuuden kautta voit antaa käyttöoikeuspohjaisen käyttöoikeuden sen resursseihin valtuutetuille käyttäjille ja asiakassovelluksissa, jotka voivat käyttää ohjelmointirajapintaasi.
7. Azure Active Directory B2C:ssä (Azure AD B2C) resurssin omistajan salasanan tunnistetiedot (ROPC) ovat OAuth-vakiotodennusmenetelmä. Tässä työnkulussa sovellus, joka tunnetaan myös nimellä luotettava osapuoli, vaihtaa kelvollisia tunnistetietoja tunnuksille. Tunnistetiedot sisältävät käyttäjätunnuksen ja salasanan. Palautetut tunnukset ovat tunnustietue, käyttötunnus ja päivitystunnus. Lisätietoja on kohdassa Resurssin omistajan salasanan tunnistetietojen [työnkulun määrittäminen Azure Active Directory B2C:ssä.](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow) 

