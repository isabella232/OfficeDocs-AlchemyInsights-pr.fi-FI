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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084343"
---
# <a name="sso-connection-issues"></a>SSO-yhteysongelmat

1. Määritä [sovellus seuraamalla pika-aloitustoimintoa: sovellusoppaan](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) ominaisuuksien määrittäminen.
2. Noudata seuraavia ohjeita [valitsemasi sovelluksen](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) ja kertakirjausvaihtoehdon mukaan:
    - Jos haluat **määrittää** paikallisen sovelluksen **SAML-pohjaista** kertakirjaamista varten, katso SAML-kertakirjaaminen paikallisille sovelluksille, joissa [on sovelluksen välityspalvelin.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Lisätietoja **pilvisovelluksen määrittämisestä** **salasanapohjaisia kertakirjaumista varten on** kohdassa Salasanan [kertakirjauksesi määrittäminen.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Lisätietoja paikallisen sovelluksen **määrittämisestä kertakirjaamista** varten sovelluksen välityspalvelimen kautta **on** kohdassa Kertakirjautuksen salasanasäilön määrittäminen [sovelluksen välityspalvelimen avulla.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Sovelluksen välityspalvelimen** ongelmien vianmääritys: on suositeltavaa aloittaa vianmäärityksen [kulku,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)sovelluksen välityspalvelimen yhdistimen ongelmien vianmääritys , jotta voit selvittää, onko sovelluksen välityspalvelimen yhdistimien määritykset oikein määritetty. Jos sinulla on edelleen ongelmia yhteyden muodostamisessa sovellukseen, noudata vianmääritystoimintoa, joka on ohjeen mukaan sovelluksen [välityspalvelimen ongelmien vianmäärityksessä.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Voit tunnistaa [CORS-ongelmia](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) selaimen virheenkorjaustyökalujen avulla:
    - Käynnistä selain ja selaa verkkosovellukseen.
    - Avaa **virheenkorjauskonsoli painamalla F12-näppäintä.**
    - Yritä toistaa tapahtuma uudelleen ja tarkista konsolin viesti. CORS-virhe aiheuttaa konsolivirheen alkuperästä.
    - Joitakin CORS-ongelmia ei voida ratkaista, esimerkiksi silloin, kun sovellus login.microsoft.com todennettavaksi, ja käyttöoikeustietue vanhenee. Cors-puhelu epäonnistuu. Vaihtoehtoinen menetelmä tälle skenaariolle on käyttöoikeustietueen elinkaaren pidentäminen, jotta se ei vanhene käyttäjän istunnon aikana. Lisätietoja tästä on kohdassa Määritettävissä [olevat](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)tunnusten elinkaaren Microsoftin käyttäjätietoympäristö.
4. **SAML-pohjaisen** kertakirjaustoiminnon vianmääritys: suosittelemme tarkistamaan [SAML-pohjaisiin](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)kertakirjaussovelluksiin kirjautumisongelmat , jotta löydät ratkaisuja ongelmiin, joita todennäköisimmin kohtaat.
5. **Salasanapohjaisen kertakirjaustoiminnon** vianmääritys: suosittelemme tarkistamaan Azure [AD:n](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)salasanapohjaisen kertakirjausongelman vianmäärityksen, jotta löydät ratkaisut todennäköisimmin kohtaamiin ongelmiin.
6. Lisätietoja VPN-yhteyden käytössä liittyvistä yhteysongelmista on kohdassa Kertakirjautumisen käyttäminen VPN-yhteyden ja [Wi-Fi kautta.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
