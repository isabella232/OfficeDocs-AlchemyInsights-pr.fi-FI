---
title: Saumaton SSO-integraattiin paikallisiin sovelluksiin liittyvät ongelmat
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868676"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Saumaton SSO-integraattiin paikallisiin sovelluksiin liittyvät ongelmat

Jos haluat tehdä vianmäärityksen Seamless SSO -integroinnissa paikallisiin sovelluksiin, toimi seuraavasti:

**Suositellut vaiheet**

1. Jos haluat määrittää **paikallisen sovelluksen** kertakirjaamista varten sovelluksen välityspalvelimen **kautta,** katso kertakirjautuksen salasanasäilöä sovelluksen [välityspalvelimen avulla.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Sovelluksen välityspalvelimen** ongelmien vianmääritys: suosittelemme käynnistämään vianmäärityksen, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)sovelluksen välityspalvelimen yhdistinongelmien vianmäärityksen tarkistamisen ja määrittämään, onko sovelluksen välityspalvelimen yhdistimiä määritetty oikein. Jos sinulla on edelleen ongelmia yhteyden muodostamisessa sovellukseen, noudata vianmääritysohjeita sovelluksen välityspalvelimen [ongelmien vianmäärityksessä.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Voit tunnistaa [CORS-ongelmia](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) käyttämällä seuraavia selaimen virheenkorjaustyökaluja:
    1. Käynnistä selain ja siirry verkkosovellukseen.
    1. Avaa **virheenkorjauskonsoli painamalla F12-näppäintä.**
    1. Yritä tehdä tapahtuma uudelleen ja tarkista konsolin viesti. KORS-rikkomus aiheuttaa konsolivirheen alkuperästä.
    1. Joitakin CORS-ongelmia ei voi ratkaista, esimerkiksi silloin, kun sovellus ohjaa login.microsoftonline.com todennuksia varten ja käyttöoikeustietue vanhenee. Sen jälkeen CORS-puhelu epäonnistuu. Vaihtoehtoinen menetelmä tähän skenaarioon on käyttöoikeustietueen elinkaaren pidentäminen, jotta se ei vanhene käyttäjän istunnon aikana. Lisätietoja tästä on kohdassa Määritettävissä olevat tunnusten elinkaarit [Microsoftin käyttäjätietoympäristössä.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Suositellut asiakirjat**

- [Kertakirjauksesi määrittäminen sovelluksen välityspalvelinsovellukseen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML-kertakirjaminen paikallisille sovelluksille sovelluksen välityspalvelimen avulla](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Azure Active Directory -sovelluksen välityspalvelimen CORS-ongelmien ymmärtäminen ja ratkaiseminen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Sovelluksen välityspalvelimen Kerberos-rajoitettujen delegointimääritysten vianmääritys](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)