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
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063618"
---
# <a name="configure-and-customize-applications"></a>Sovellusten määrittäminen ja mukauttaminen

**Sovellusten määrittäminen**

1. [Pika-aloitus: Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) -vuokraajan sovelluksen ominaisuuksien määrittäminen näyttää, miten voit määrittää joitakin sovelluksen ominaisuuksia.
2. Jotta sovellukset voidaan integroida Azure Active Directoryyn, olemme kehittäneet opetusohjelmakokoelman, [joka](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) opastaa sinua määrityksessä.
3. [Sovelluksen välityspalvelinsovelluksen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) määrittäminen auttaa ymmärtämään, miten voit määrittää sovelluksen välityspalvelinsovelluksen Azure AD:ssä, jotta voit näyttää paikallisen sovelluksen pilvessä.
4. [Lataa PingAccess ja määritä](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)sovellus: Noudata Azure *AD:n Configure PingAccess -sovelluksen* ohjeita, jotta voit suojata Microsoft Azure AD Application Proxy -välityspalvelimella ping-käyttäjätiedot -sivustossa julkaistuja sovelluksia ja ladata uusimman PingAccess-version.

**Virheelliset sovellusvirheet (AADSTS650056)**

1. Varmista, että käytät sovellusta sovelluksen omistajan kirjautumisosoitteesta. Muussa tapauksessa kirjaudu sovellukseen normaalin prosessin kautta. Useimmissa tapauksissa tämä ratkaisee automaattisesti luonnollisesti. Jos näin ei ole, tämä viesti voi auttaa vianmäärityksessä ja sen ratkaisemisessa.
2. **Jos organisaatiosi omistaa sovelluksen** (eli sovelluksen rekisteröinti on organisaatiossasi):
    - Microsoft suosittelee vähintään Microsoft `User.Read` `openid` **Graphin** valtuutettua käyttöoikeutta.
    - Varmista, että sovellus ja kaikki sen käyttöoikeudet ovat suostuneet. Voit tarkistaa tämän tarkastelemalla  sovelluksen rekisteröinnin Tila-saraketta **ohjelmointirajapinnan käyttöoikeuksissa.**
    - Joissakin tilanteissa sovellus saattaa olla kolmannen osapuolen, mutta se saattaa olla rekisteröity organisaatiossasi. Tarkista, näkyykö sovellus sovelluksen rekisteröinnissä (ei Enterprise-sovelluksissa).
    - Jos näet edelleen tämän virhesanoman. Sen jälkeen voit joutua rakentamaan vaiheessa 4 kuvatun **suostumuksen URL-osoitteen.**
3. **Jos organisaatiosi ei ole sovelluksen omistaja ja käytät sitä kolmannen osapuolen sovelluksena:**
    - Jos olet yleinen/yrityksen järjestelmänvalvoja, sinun pitäisi nähdä suostumusnäyttö. Varmista, että hyväksyt organisaation puolesta **-valintaruudun.**
    - Jos et näe suostumusnäyttöä, poista Enterprise-sovellus ja yritä uudelleen.
    - Jos näet edelleen tämän virhesanoman. Sen jälkeen voit joutua rakentamaan vaiheessa 4 kuvatun **suostumuksen URL-osoitteen.**
4. **Muodosta käytettävä** suostumuksen URL-osoite manuaalisesti: Jos sovellus on suunniteltu käyttämään tiettyä resurssia, et ehkä voi käyttää Azure-portaalin Suostumus-painikkeita, sinun on luotava oma suostumuksesi URL-osoite manuaalisesti ja käytettävä tätä.
    - Sinun täytyy saada sovelluksen `{App-Id}` omistaja `{App-Uri-Id}` ja sen henkilöltä. `{Tenant-Id}` on vuokraajan tunniste. Tämä on joko `yourdomain.onmicrosoft.com` hakemistotunnus tai hakemiston tunnus.
    - Jos sovellus käyttää resurssia itseensä, ja `{App-Id}` `{App-Uri-Id}` se on sama.
5. Lisätietoja on kohdassa [SAML-pohjaisiin kertakirjaussovelluksiin kirjautumisongelmat.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Sovellusten mukauttaminen**

- [Lisää brändi](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) organisaatiosi Azure Active Directory -kirjautumissivulle – Käytä organisaatiosi logoa ja mukautettuja värimalleja, jotta Azure Active Directory (Azure AD) -kirjautumissivut ovat yhdenmukaisia.
- [Lisää mukautettu toimialuenimesi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) -portaalissa – Jokaisella uudella Azure AD -vuokraajassa on alkuperäinen toimialuenimi. Et voi muuttaa tai poistaa alkuperäistä toimialuenimeä, mutta voit lisätä organisaatiosi nimet. Lisäämällä mukautettuja toimialuenimiä voit luoda käyttäjille tuttuja käyttäjänimiä.
