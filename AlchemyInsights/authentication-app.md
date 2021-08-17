---
title: Todennussovellus
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082939"
---
# <a name="authentication-app"></a>Todennussovellus

Jos olet yleinen järjestelmänvalvoja, voit selvittää nopeasti, mitä on tapahtunut tai diagnosoida käyttäjän sisäänkirjautumisongelmia kirjautumisen [vianmäärityksen avulla.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Käynnistä vianmääritys napsauttamalla Käynnistä diagnostiikka[-painiketta.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Etsi analysoitava tapahtuma kirjoittamalla tiedot käyttäjästä, sovelluksesta, kirjautumisajasta, pyynnön tunnuksesta tai korrelaatiotunnuksesta.
1. Tarkista diagnostiikkatulokset, jotka näyttävät tiedot siitä, mitä on tapahtunut ja mitä voit tehdä muutosten tekoon, jos muutoksia tarvitaan.

**Tarkista soveltuva skenaario:**

1. Jos käyttäjä ei saa push-ilmoitusta Microsoft Authenticator-sovelluksessa, varmista, että häntä ei näy MFA:n estettyjen käyttäjien alla artikkelissa Käyttäjien estäminen ja salliminen [kuvatulla tavalla.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Jos MFA ei estä käyttäjää, mutta hän ei saa push-ilmoitusta, hän voi avata Microsoft Authenticator-sovelluksen, joka pyytää odottavat hyväksyntäpyynnöt.
1. Vaihtoehtoisen kirjautumismenetelmän avulla käyttäjä voi myös napsauttaa Kirjaudu sisään muulla tavalla ja valita käyttää mobiilisovelluksessa olevaa vahvistuskoodia.
1. The Microsoft Authenticator App is the only available method for many users. [Lisätietoja suojauksen oletusasetuksista](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)on usein [kysytyissä Authenticator usein](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) kysytyissä kysymyksissä ja niiden ratkaisemisessa.
 
**Suositellut videot**

[Ohjeet Authenticator sovelluksesi asentaminen uuteen puhelimeen (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
