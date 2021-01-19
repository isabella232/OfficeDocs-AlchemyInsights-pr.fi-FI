---
title: Sovelluksiin kirjautumisongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901035"
---
# <a name="issues-signing-in-to-applications"></a>Sovelluksiin kirjautumisongelmat

Voit tunnistaa käyttäjän sisäänkirjautumisongelmien syyn tai vianmäärityksen seuraavasti:

1. Käynnistä [kirjautumisen vianmääritys.](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
2. Etsi analysoitava tapahtuma kirjoittamalla tiedot käyttäjästä, sovelluksesta, kirjautumisajasta, pyyntötunnuksesta tai korrelaatiotunnuksesta.
3. Tarkista diagnostiikkatulokset, jotka näyttävät, mitä on tapahtunut ja mitä voit tehdä muutosten tekoon, jos muutoksia tarvitaan.

Seuraavassa on joitakin yleisiä ongelmia, joita voi i kokea, kun kirjaudut sisään sovelluksiin:

1. Sinä tai käyttäjä on suorittanut Azure AD -kirjautumisen, mutta näyttöön tulee odottamaton kehote – Tutustu artikkeleihin Odottamaton suostumuskehote, kun kirjaudut sovellukseen ja odottamaton virhe, kun suoritat [sovelluksen suostumuksen.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)  [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
2. Sinä tai käyttäjä olette kirjautuneet sovellukseen **suoraan,** mutta ette voi kirjautua sovellukseen mukautetun portaalin tai käyttöpaneelin syvälinkin kautta: Katso Azure AD My Apps -sovellukseen kirjautumisongelmien [vianmääritys.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
3. Sinä tai käyttäjä on suorittanut **Azure AD**-kirjautumisen, mutta sovellus näyttää virhesanoman eikä anna käyttäjän suorittaa kirjautumista loppuun: Ongelma on siinä, että sovellus ei hyväksynyt Azure AD:n antamaa vastausta. Voit [tehdä vianmäärityksen](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) seuraavasti.
4. Sinä tai käyttäjä ette voi kirjautua sisään **ei-valikoimaan** määritettyyn sovellukseen, joka on määritetty kertakirjaamista varten: Suorita vianmääritys [seuraavien](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) ohjeiden mukaisesti.
5. Sinä tai käyttäjä ette **voi kirjautua Azure AD Gallery**-sovellukseen, joka on määritetty kertakirjaumista varten: Suorita vianmääritys seuraavasti. [](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
6. Sinä tai käyttäjä **ette voi kirjautua sisään Microsoft-sovellukseen:** Suorita vianmääritys [seuraavasti.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
7. Sinä tai käyttäjä ette voi kirjautua sisään ei-valikoimaan liitettyä kertakirjainta varten määritettyyn **ei-valikoimaan määritettyyn sovellukseen:** Suorita vianmääritys [seuraavasti.](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery)
8. Sinä tai käyttäjä ette voi kirjautua azure AD -valikoimasovellukseen, joka on määritetty liittoutettua kertakirjainta **varten:** Suorita vianmääritys [seuraavasti.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)
9. Sinä tai käyttäjä **ette voi kirjautua sisään mukautettuun sovellukseen:** Suorita vianmääritys [seuraavasti.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)
10. Sinä tai käyttäjä **ette voi kirjautua paikalliseen** sovellukseen Azure AD -sovelluksen välityspalvelimen avulla: Suorita vianmääritys [seuraavasti.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy)

