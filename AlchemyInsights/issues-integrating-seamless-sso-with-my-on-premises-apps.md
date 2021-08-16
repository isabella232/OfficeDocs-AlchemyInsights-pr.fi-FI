---
title: Saumattoman SSO:n integrointiin paikallisiin sovelluksiin liittyvät ongelmat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028289"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Saumattoman SSO:n integrointiin paikallisiin sovelluksiin liittyvät ongelmat

Jos haluat tehdä vianmäärityksen Seamless SSO -integroinnissa paikallisiin sovelluksiin, toimi seuraavasti:

**Suositellut vaiheet**

1. Lisätietoja paikallisen sovelluksen **määrittämisestä kertakirjaamista** varten sovelluksen välityspalvelimen kautta **on** kohdassa Kertakirjautuksen salasanasäilön määrittäminen [sovelluksen välityspalvelimen avulla.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Sovelluksen välityspalvelimen** ongelmien vianmääritys: suosittelemme, että aloitat vianmäärityksen [ja](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)sovelluksen välityspalvelimen yhdistinongelmien vianmäärityksen tarkistamisen sen määrittämiseksi, onko sovelluksen välityspalvelimen yhdistimiin määritetty oikein. Jos sinulla on edelleen ongelmia yhteyden muodostamisessa sovellukseen, noudata vianmääritysohjeita, jotka on annettu ohjeena sovelluksen [välityspalvelimen ongelmien vianmäärityksessä.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Voit tunnistaa [CORS-ongelmia](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) käyttämällä seuraavia selaimen virheenkorjaustyökaluja:
    1. Käynnistä selain ja selaa verkkosovellukseen.
    1. Avaa **virheenkorjauskonsoli painamalla F12-näppäintä.**
    1. Yritä toistaa tapahtuma uudelleen ja tarkista konsolin viesti. CORS-virhe aiheuttaa konsolivirheen alkuperästä.
    1. Joitakin CORS-ongelmia ei voida ratkaista, esimerkiksi silloin, kun sovellus ohjaa login.microsoftonline.com todennettavaksi, ja käyttöoikeustietue vanhenee. Cors-puhelu epäonnistuu. Vaihtoehtoinen menetelmä tälle skenaariolle on käyttöoikeustietueen elinkaaren pidentäminen, jotta se ei vanhene käyttäjän istunnon aikana. Lisätietoja tästä on kohdassa Määritettävissä [olevat](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)tunnusten elinkaaren Microsoftin käyttäjätietoympäristö.

**Suositellut asiakirjat**

- [Kertakirjauksesi määrittäminen sovelluksen välityspalvelimen sovellukseen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML-kertakirjaminen paikallisille sovelluksille sovelluksen välityspalvelimen avulla](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Sovelluksen välityspalvelimen AZURE ACTIVE DIRECTORY ongelmien ymmärtäminen ja ratkaiseminen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Kerberos-välityspalvelimen rajoitettujen delegointimääritysten vianmääritys](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)