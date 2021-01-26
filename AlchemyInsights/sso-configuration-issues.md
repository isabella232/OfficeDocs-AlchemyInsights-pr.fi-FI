---
title: SSO-määritysongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7760"
- "9004346"
ms.openlocfilehash: 5ab56ec1eda10ea059e600e8933ce85bb143b76e
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901049"
---
# <a name="sso-configuration-issues"></a>SSO-määritysongelmat

1. Seuraa [pika-aloitustoimintoa: Määritä sovelluksen asetukset sovellusoppaan](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) avulla.
2. Noudata seuraavia ohjeita [](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) valitsemasi sovelluksen ja kertakirjausvaihtoehdon mukaan: a. Jos haluat **määrittää** paikallisen sovelluksen SAML-pohjaista kertakirjautumista **(SSO)** varten, katso SAML-kertakirjautuminen paikallisille sovelluksille, joissa [on sovelluksen välityspalvelin.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    b. Lisätietoja **pilvisovelluksen määrittämisestä** **salasanapohjaiselle** kertakirjautumista varten on kohdassa [Salasanan kertakirjautumisen määrittäminen.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    c. Jos haluat määrittää **paikallisen sovelluksen kertakirjautumista** varten sovelluksen **välityspalvelimen** kautta, katso kertakirjautumisen salasanasäilöä sovelluksen [välityspalvelimen avulla.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Sovelluksen välityspalvelimen** ongelmien vianmääritys: Suosittelemme, että tarkistat [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors) vianmäärityksen vianmäärityksen ( Sovelluksen välityspalvelimen yhdistimen vianmäärityksen ongelmat) sen määrittämiseksi, onko sovelluksen välityspalvelimen yhdistimiä määritetty oikein. Jos sinulla on edelleen ongelmia yhteyden muodostamisessa sovellukseen, noudata vianmääritysohjeita sovelluksen välityspalvelimen [ongelmien vianmäärityksessä.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Voit tunnistaa [CORS-ongelmia](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) suorittamalla seuraavat selaimen virheenkorjausvaiheet: a. Käynnistä selain ja siirry verkkosovellukseen.
    b. Avaa **virheenkorjauskonsoli painamalla F12-näppäintä.**
    c. Yritä toistaa tapahtuma ja tarkista konsolin viesti. KORS-rikkomus aiheuttaa konsolivirheen alkuperästä.
    d. Joitakin CORS-ongelmia ei voida ratkaista, kuten käyttöoikeustietueen vanhenemista, kun sovellus ohjaa login.microsoftonline.com todennusta varten. Käyttöoikeustietueen vanhentumisen vuoksi CORS-kutsu epäonnistuu. Vaihtoehtoinen menetelmä tähän skenaarioon on käyttöoikeustietueen elinkaaren pidentäminen, jotta se ei vanhene käyttäjän istunnon aikana. Lisätietoja tästä on kohdassa Määritettävissä olevat tunnusten elinkaarit [Microsoftin käyttäjätietoympäristössä.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **SAML-pohjaisen** kertakirjautumisen vianmääritys: Suosittelemme tarkistamaan [SAML-pohjaisiin](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) kertakirjautumissovelluksiin kirjautumisongelmat, jotta löydät ratkaisuja ongelmiin, joita todennäköisimmin kohtaat.
5. **Salasanapohjaisen** kertakirjautumisen vianmääritys: Suosittelemme tarkistamaan salasanapohjaisen kertakirjautumisen vianmäärityksen Azure AD:ssä, jotta löydät ratkaisuja ongelmiin, joita todennäköisimmin kohtaat. [](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
6. **Sain määritysvirheen:** Määritysvirheiden vianmäärityksessä on suositeltavaa tarkistaa seuraavat artikkelit: a. [SAML-pohjaisiin kertakirjaussovelluksiin](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) b kirjautumisongelmat. [Tunnistetiedot täytetään, mutta laajennus ei lähetä niitä](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso#credentials-are-filled-in-but-the-extension-does-not-submit-them) c. [Tunnistetiedot täytetään ja lähetetään, mutta sivu osoittaa, että tunnistetiedot ovat virheellisiä](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) d. [Sovellussivulla näkyy virhesanoma, kun käyttäjä kirjautuu sisään](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
7. **Minulla on ongelmia Seamless SSO:n** integroinnissa paikallisiin sovelluksiin: Saumattoman SSO:n integrointiin paikallisiin sovelluksiin koskevien ongelmien vianmäärityksessä on suositeltavaa tarkistaa seuraavat artikkelit: a. [Kertakirjauksesi määrittäminen sovelluksen välityspalvelinsovellukseen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to) b. [SAML-kertakirjaus paikallisille sovelluksille, joissa on sovelluksen välityspalvelin](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps) c. [Azure Active Directory -sovelluksen välityspalvelimen CORS-ongelmien ymmärtäminen ja ratkaiseminen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues) d. [Sovelluksen välityspalvelimen Kerberos-rajoitettujen delegointimääritysten vianmääritys](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
8. **Haluan korjata vaateet tai pidentää tunnuksen elinkaaria. Istuntoa on muutettava:** Tätä varten kannattaa tarkistaa seuraavat artikkelit: a. [Mukauta sovellukselle b lähetettyjä SAML-vaateita.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) [Claims-aware apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) c. [Määritettävissä olevat tunnusten elinkaarit Microsoftin käyttäjätietoympäristössä](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) d. [Todennusistunnon hallinnan määrittäminen ehdollisen käyttöoikeuden e:n](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) avulla. [Evästeasetukset paikallisiin sovelluksiin pääsyä varten](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings)
9. Tarvitsen apua käyttäjän ja vieraskäyttäjien **(B2B)** käyttöoikeuksien hallinnassa: Lisätietoja käyttäjän ja vieraskäyttäjän käyttöoikeuksien hallinnasta on seuraavissa artikkeleissa: a. [Sovellusten b käyttöoikeuksien](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-access-management) hallinta [Hallitse sovelluksen käyttäjämääritystä Azure Active Directory c:ssä.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) [Määritä SaaS-sovellukset B2B-yhteistyötä](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) varten d. [Myönnä Azure AD:n B2B-käyttäjille käyttöoikeudet paikallisiin sovelluksiin](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) e. [Paikallisesti hallittujen kumppanitilien käyttöoikeuden myöntäminen pilviresursseihin Azure AD B2B -yhteistyön avulla](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)
10. **Haluan mukauttaa sovelluksia: Jos** haluat lisätietoja sovellusten mukauttamisesta, suosittelemme tarkistamaan seuraavat artikkelit: a. [Mukautettujen toimialueiden määrittäminen Azure AD -sovelluksen välityspalvelimen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain) b avulla. [Mukautetun aloitussivun luominen julkaistuille sovelluksille](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page) c. [Yleismerkkisovellukset](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard)
11. **Minulla on ongelmia sovelluksen** siirrossa AD FS:stä Azureen: Jotta voin ratkaista ongelmia, joita ilmeni, kun sovellus siirretään AD FS:stä Azureen, suosittelemme tarkistamaan seuraavat artikkelit: a. [Sovellustodennuksen siirtäminen Active Directory -liittoutumispalveluista Azure Active Directory b:een.](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-apps-to-azure) [Resursseja sovellusten azure Active Directoryyn](https://docs.microsoft.com/azure/active-directory/manage-apps/migration-resources)
