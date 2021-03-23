---
title: OAuth 2.0- ja OpenID Connect -protokollien vianmääritys
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036401"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>OAuth 2.0- ja OpenID Connect -protokollien vianmääritys

Voit ratkaista OAuth 2.0: n ja OpenID Connectin ongelmat seuraavasti:

Tutustu seuraaviin artikkeleihin, jotka liittyvät OAuth 2.0- ja OpenID Connect -protokollien määritykseen ja vianmääritykseen:

- [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - This article describes how to program directly against the **code grant (PKCE) flow** in your application, using any language.
- [Microsoftin tunnistetietoympäristö ja OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -asiakasohjelman tunnistetiedot työnkulku  – tässä artikkelissa kerrotaan, miten ohjelma voidaan ohjelmoida suoraan sovelluksen asiakastunnusten perusteella.
- [Microsoftin käyttäjätietojen käyttöympäristö ja OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) -resurssin omistajan salasanan tunnistetiedot – tässä artikkelissa kerrotaan, miten voit ohjelmoida suoraan **ropc-työnkulkuun** sovelluksessa.
    - Microsoftin käyttäjätietoympäristö tukee vain Azure AD -vuokralaisten ropc-tallennustilaa, ei henkilökohtaisia tilejä. Tämä tarkoittaa, että sinun on käytettävä vuokraajakohtaista päätepistettä **(tai https://login.microsoftonline.com/{TenantId_or_Name})** **organisaatioiden päätepistettä).**
    - Henkilökohtaiset tilit, jotka on kutsuttu Azure AD -vuokraajaan, eivät voi käyttää ROPC:tä.
    - Tilit, joissa ei ole salasanoja, eivät voi kirjautua ropc:n kautta. Tässä skenaariossa suosittelemme, että käytät eri työnkulkua sovellukselle.
    - Jos käyttäjien on kirjauduttava sovellukseen monimenetelmäisen todentamisen [(MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) avulla, ne estetään.
    - RoPC:tä ei tueta [yhdistelmämallien](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) liittämisskenaarioissa (esimerkiksi Azure AD ja ADFS, joita käytetään paikallisen tilin todentamisessa). Jos käyttäjät ohjataan koko sivun koko sivun paikalliseen tunnistetietojen toimittajaan, Azure AD ei voi testata käyttäjänimeä ja salasanaa palveluntarjoajalta. [Läpitunnistus on](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) kuitenkin tuettu ROPC:ssä.
    - Poikkeus yhdistelmäkäyttäjätietojen liittämisskenaarioon olisi seuraava: Home Realm Discovery -käytäntö, jonka **AllowCloudPasswordValidation-asetuksena** on **TOSI,** mahdollistaa ROPC-työnkulun toimimisen organisaation ulkopuolisia käyttäjiä varten, kun paikallinen salasana synkronoidaan pilvipalveluun. Lisätietoja on ohjeaiheessa Liitettyjen käyttäjien suoran [ROPC-todennuksen ottaminen käyttöön vanhoissa sovelluksissa](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- Microsoftin käyttäjätietoympäristö ja [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) Työnkulun puolesta – tässä artikkelissa kerrotaan, miten voit ohjelman suoraan vastaan sovelluksen **(OBO)** puolesta.
- [Microsoftin käyttäjätietoympäristö](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) ja OpenID Connect -protokolla – Tässä artikkelissa kerrotaan, miten OpenID Connect -protokolla voidaan ottaa käyttöön kielestä riippumatta ja miten HTTP-viestejä lähetetään ja vastaanotaan ilman Microsoftin avoimen lähdekoodin kirjastoja.

**Access-tunnukset**

[Microsoftin käyttäjätietoympäristön käyttöoikeustietueet](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Lue, miten ohjelmointirajapintasi voi vahvistaa ja käyttää käyttöoikeustietueen sisällä tavia vaateita. Kaikki tämän artikkelin ohjeet, paitsi jos ne on mainittu, koskevat vain rekisteröityjen ohjelmointirajapintojen tunnuksia. Se ei koske Microsoftin omistamien ohjelmointirajapintojen tunnuksia eikä tunnuksia, joilla vahvistetaan, miten Microsoftin tunnistetietoympäristö myöntää tunnuksia luomaasi ohjelmointirajapintaan.

**Sovelluksen määritykset**

[Redirect URI (reply URL) restrictions and limitations](https://docs.microsoft.com/azure/active-directory/develop/reply-url) - Learn how to configure your Redirect URI (reply URL). Uudelleenohjauksen URI eli vastauksen URL-osoite on sijainti, johon valtuutuspalvelin lähettää käyttäjän, kun sovellus on onnistuneesti valtuutettu ja hänelle on myönnetty valtuutuskoodi tai käyttöoikeustunnus. Valtuutuspalvelin lähettää koodin tai tunnuksen uudelleenohjauksen URI-tunnukseen. siksi on tärkeää, että rekisteröit oikean sijainnin osana sovelluksen rekisteröintiprosessia.

**Sovelluksen valmistelu**

[Opetusohjelma: SCIM-päätepisteen](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) valmistelun kehittäminen ja suunnitteleminen – Tässä artikkelissa kerrotaan, miten VOIT LUODA SCIM-päätepisteen ja integroida sen AAD-valmistelupalveluun.


