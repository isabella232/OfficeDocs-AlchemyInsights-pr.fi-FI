---
title: Sovellusten määrittäminen ja mukauttaminen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004334"
- "7733"
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044985"
---
# <a name="configure-and-customize-applications"></a>Sovellusten määrittäminen ja mukauttaminen

**Sovellusten määrittäminen**

1. [Pika-aloitus: Sovelluksen ominaisuuksien määrittäminen Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) -vuokraajassa näyttää, miten voit määrittää joitakin sovelluksen ominaisuuksia.
2. Jotta sovellukset voidaan integroida Azure Active Directory, olemme kehittäneet kokoelman opetusohjelmia, [jotka](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) opastavat sinua määrityksessä.
3. [Sovelluksen välityspalvelimen sovelluksen määrittäminen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) auttaa ymmärtämään, miten voit määrittää sovelluksen välityspalvelinsovelluksen Azure AD:ssä niin, että se näyttää paikallisen sovelluksen pilvipalvelussa.
4. [Lataa PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)ja määritä sovellus: Noudata ohjeita, jotka ovat ohjeessa *PingAccessin* määrittäminen Azure AD:lle, jotta voit suojata ping-käyttäjätiedot Microsoft Azure AD-sivuston Microsoft Azure AD Application Proxy -sovelluksella julkaistut sovellukset ja ladata uusimman PingAccess-version.

**Virheelliset sovellusmääritykset (AADSTS650056) -virheet**

1. Varmista, että käytät sovellusta sovelluksen omistajan kirjautumisosoitteesta. Muussa tapauksessa kirjaudu sovellukseen normaalin prosessin kautta. Useimmissa tapauksissa tämä ratkaisee automaattisesti luonnollisesti. Jos näin ei ole, tämä viesti voi auttaa vianmäärityksessä ja sen ratkaisemisessa.
2. **Jos organisaatiosi omistaa sovelluksen** (eli sovelluksen rekisteröinti on organisaatiossasi):
    - Microsoft suosittelee vähintään Microsoftilta lupaa `User.Read` tai `openid` delegoitua Graph lisätään. 
    - Varmista, että sovellus ja kaikki sen käyttöoikeudet ovat suostuneet. Voit tarkistaa tämän sovelluksen  rekisteröinnin Tila-sarakkeesta **API-käyttöoikeuksissa.**
    - Joissakin tilanteissa sovellus saattaa olla kolmas osapuoli, mutta se saattaa olla rekisteröity organisaatiossasi. Varmista, että sovellus näkyy sovelluksen rekisteröitymisissä (ei Enterprise-sovelluksissa).
    - Jos tämä virhesanoma tulee edelleen näkyviin. Tämän jälkeen sinun on ehkä muodosnnettava vaiheessa 4 kuvattu **suostumus-URL-osoite.**
3. **Jos organisaatiosi ei ole sovelluksen omistaja ja käytät sitä kolmannen osapuolen sovelluksena:**
    - Jos olet yleinen tai yrityksen järjestelmänvalvoja, sinun pitäisi nähdä suostumusnäyttö. Varmista, että valintaruutu **"Suostumus organisaatiosi puolesta" on valintaruutu.**
    - Jos et näe suostumusnäyttöä, poista Enterprise-sovellus ja yritä uudelleen.
    - Jos tämä virhesanoma tulee edelleen näkyviin. Tämän jälkeen sinun on ehkä muodosnnettava vaiheessa 4 kuvattu **suostumus-URL-osoite.**
4. **Muodosta manuaalisesti** käytettävä url-osoite: Jos sovellus on suunniteltu käyttämään tiettyä resurssia, et ehkä voi käyttää Azure-portaalin Suostumus-painikkeita, sinun on luotava oma suostumuksesi URL-osoite manuaalisesti ja käytettävä sitä.
    - Sinun täytyy saada sovelluksen `{App-Id}` omistaja `{App-Uri-Id}` ja henkilöltä. `{Tenant-Id}` on vuokraajasi tunniste. Tämä on joko `yourdomain.onmicrosoft.com` hakemistotunnus tai hakemiston tunnus.
    - Jos sovellus käyttää resurssia itseensä, ja `{App-Id}` `{App-Uri-Id}` se on sama.
5. Lisätietoja on kohdassa [SAML-pohjaisiin kertakirjaussovelluksiin kirjautumisongelmat.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Sovellusten mukauttaminen**

- [Lisää brändi](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) organisaation Azure Active Directory -kirjautumissivulle – Organisaation logon ja mukautettujen värimallien avulla voit luoda yhtenäisen ulkoasun Azure Active Directory (Azure AD) -kirjautumissivuille.
- [Mukautetun toimialuenimen lisääminen Azure Active Directory portaalissa](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – Jokaisella uudella Azure AD -vuokraajassa on alkuperäinen toimialuenimi. Et voi muuttaa tai poistaa alkuperäistä toimialuenimeä, mutta voit lisätä organisaatiosi nimet. Lisäämällä mukautettuja toimialuenimiä voit luoda käyttäjille tuttuja käyttäjänimiä.
