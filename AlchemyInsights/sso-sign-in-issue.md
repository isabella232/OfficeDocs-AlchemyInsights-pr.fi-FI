---
title: Saumaton SSO-käyttäjän kirjautumisongelmat
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
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935122"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Saumaton SSO-käyttäjän kirjautumisongelmat

Kun käyttäjä on todennettu, selain tallentaa käyttäjän tunnistetiedot välimuistiin, jotta sama selain kirjautuu automaattisesti sisään samalla tilillä. Tämä voi vaikeuttaa toisen käyttäjän tai yksittäisen käyttäjän kirjautumista useisiin tileihin yhdellä laitteella. Voit ratkaista ongelman 1. Yritä kirjautua sisään toisella selaimella. 2. Tyhjennä selaimen välimuisti ja/tai evästeet ja yritä kirjautua sisään uudelleen.

Jos sinulla on edelleen kirjautumisongelmia, suosittelemme, että diagnosoit ja automatisoit ratkaisuvaiheet seuraavasti:

1. Asenna [Omat sovellukset -selainlaajennus,](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) jotta Azure Active Directory (Azure AD) voi tarjota paremman vianmääritys- ja ratkaisukokemuksen, kun käytät Azure-portaalin testauskokemusta.
2. Voit kopioida virheen käyttämällä Azure-portaalin sovelluksen määrityssivun testauskokemusta. Lisätietoja on ohjeaiheessa [SAML-pohjaisten kertakirjainsovelluksissa virheenkorjaus.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Jos käytät Azure-portaalin testauskokemusta My Apps Secure Browser Extension -laajennuksen kanssa, voit **ohittaa vaiheen 4.**
4. SAML-pohjaisen kertakirjausmäärityssivun avaaminen:
    - Avaa [Azure-portaali ja](https://portal.azure.com/) kirjaudu sisään yleisenä **järjestelmänvalvojana tai** **Coadmin-järjestelmänvalvojana.**
    - Avaa **Azure Active Directory -laajennus** valitsemalla kaikki **palvelut** vasemman reunan siirtymisvalikon yläreunassa.
    - Kirjoita suodatinhakuruutuun "Azure Active Directory" ja valitse **Azure Active Directory -kohde.**
    - Valitse **Yrityssovellukset** Azure Active Directoryn vasemmanpuoleinen siirtymisvalikko.
    - Valitsemalla **Kaikki sovellukset** voit tarkastella kaikkien sovellusten luetteloa. Jos haluamasi sovellus ei näy tässä, käytä  Suodata-ohjausobjektia  Kaikki sovellukset -luettelon  yläreunassa ja määritä Näytä-vaihtoehdoksi **Kaikki sovellukset.**
    - Valitse sovellus, jonka haluat määrittää kertakirjauksesi.
    - Kun sovellus on latautunut, valitse **Sovelluksen** vasemmanpuoleinen siirtymisvalikko kertakirjaus.
    - Valitse **SAML-pohjainen SSO.**
5. Virheen perusteella saat lisätietoja suositelluista vaiheista, jotka on annettu [SAML-pohjaisiin](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)kertakirjaussovelluksiin kirjautumisessa.
6. Jos haluat tehdä vianmäärityksen muiden käyttäjien kirjautumisongelmien kanssa, tutustu seuraaviin ohjeisiin:
    - [YKSI-Sign-On SAML-protokolla](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Kirjautumisvirheiden vianmääritys Azure Active Directory -raporttien avulla](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Odottamaton suostumuskehote](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Käyttäjän suostumusvirhe](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Omat sovellukset -sovelluksesta kirjautumisongelmat](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Virhe sovelluksen kirjautumissivulla](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Ongelma microsoft-sovellukseen kirjautumisessa](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
