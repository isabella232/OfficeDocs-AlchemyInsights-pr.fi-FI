---
title: SSO-yhteysongelmat
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
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935112"
---
# <a name="sso-connection-issues"></a>SSO-yhteysongelmat

1. Seuraa [pika-aloitustoimintoa: Määritä sovelluksen asetukset sovellusoppaan](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) avulla.
2. Noudata seuraavia ohjeita valitsemasi [sovelluksen ja](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) kertakirjausvaihtoehdon mukaan:
    - Jos haluat **määrittää** paikallisen sovelluksen **SAML-pohjaista** kertakirjaamista varten, katso SAML-kertakirjaaminen paikallisille sovelluksille, joissa [on sovelluksen välityspalvelin.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Lisätietoja **pilvisovelluksen määrittämisestä** **salasanapohjaisia kertakirjaumista varten on** ohjeaiheessa Salasanan [kertakirjaaminen -asetuksen määrittäminen.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Jos haluat määrittää **paikallisen sovelluksen** kertakirjaamista varten sovelluksen välityspalvelimen **kautta,** katso kertakirjautuksen salasanasäilöä sovelluksen [välityspalvelimen avulla.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Sovelluksen välityspalvelimen** ongelmien vianmääritys: suosittelemme käynnistämään vianmäärityksen, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)sovelluksen välityspalvelimen yhdistinongelmien vianmäärityksen tarkistamisen ja määrittämään, onko sovelluksen välityspalvelimen yhdistimiä määritetty oikein. Jos sinulla on edelleen ongelmia yhteyden muodostamisessa sovellukseen, noudata vianmäärityksen kulkua sovelluksen välityspalvelimen [ongelmien vianmäärityksessä.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Voit tunnistaa [CORS-ongelmia](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) selaimen virheenkorjaustyökalujen avulla:
    - Käynnistä selain ja siirry verkkosovellukseen.
    - Avaa **virheenkorjauskonsoli painamalla F12-näppäintä.**
    - Yritä tehdä tapahtuma uudelleen ja tarkista konsolin viesti. KORS-rikkomus aiheuttaa konsolivirheen alkuperästä.
    - Joitakin CORS-ongelmia ei voi ratkaista, esimerkiksi silloin, kun sovellus ohjaa login.microsoft.com todennuksia varten ja käyttöoikeustietue vanhenee. Sen jälkeen CORS-puhelu epäonnistuu. Vaihtoehtoinen menetelmä tähän skenaarioon on käyttöoikeustietueen elinkaaren pidentäminen, jotta se ei vanhene käyttäjän istunnon aikana. Lisätietoja tästä on kohdassa Määritettävissä olevat tunnusten elinkaarit [Microsoftin käyttäjätietoympäristössä.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **SAML-pohjaisen** kertakirjaumisen vianmääritys: suosittelemme tarkistamaan [SAML-pohjaisiin](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)kertakirjaussovelluksiin kirjautumisongelmat, jotta löydät ratkaisuja ongelmiin, joita todennäköisimmin kohtaat.
5. **Salasanapohjaisen** kertakirjaumisen vianmääritys: suosittelemme tarkistamaan salasanapohjaisen kertakirjaumisen vianmäärityksen Azure AD:ssä, jotta löydät ratkaisuja ongelmiin, joita todennäköisimmin kohtaat. [](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
6. Lisätietoja VPN-yhteyden käytössä liittyvistä yhteysongelmista on ohjeaiheessa Kertakirjautumisen [(SSO)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)käyttäminen VPN-yhteyden ja Wi-Fi kautta.
