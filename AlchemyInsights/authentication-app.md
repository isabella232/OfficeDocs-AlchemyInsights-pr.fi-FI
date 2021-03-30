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
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404600"
---
# <a name="authentication-app"></a>Todennussovellus

Jos olet yleinen järjestelmänvalvoja, voit selvittää nopeasti, mitä on tapahtunut tai diagnosoida käyttäjän sisäänkirjautumisongelmia kirjautumisen [vianmäärityksen avulla.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Käynnistä vianmääritys napsauttamalla[Käynnistä](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)diagnostiikka -painiketta. 
1. Etsi analysoitava tapahtuma kirjoittamalla tiedot käyttäjästä, sovelluksesta, kirjautumisajasta, pyyntötunnuksesta tai korrelaatiotunnuksesta.
1. Tarkista diagnostiikkatulokset, jotka näyttävät, mitä on tapahtunut ja mitä voit tehdä muutosten tekoon, jos muutoksia tarvitaan.

**Tarkista soveltuva skenaario:**

1. Jos käyttäjä ei saa push-ilmoitusta Microsoft Authenticator -sovelluksessa, varmista, että häntä ei näy MFA:n estettyjen käyttäjien alla kohdassa Käyttäjien estäminen ja eston [poistaminen kuvatulla tavalla.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Jos käyttäjää ei estetä MFA-todentamista varten, mutta hän ei saa push-ilmoitusta, hän voi avata Microsoft Authenticator -sovelluksen, joka pyytää odottavia hyväksyntäpyyntöjä.
1. Vaihtoehtoisena kirjautumismenetelmänä käyttäjä voi myös napsauttaa Kirjaudu sisään muulla tavalla ja valita käyttää vahvistuskoodia mobiilisovelluksestani.
1. Microsoft Authenticator -sovellus on ainoa käytettävissä oleva menetelmä monille käyttäjille. [Lue lisää suojauksen oletusasetuksista,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)tarkista [Authenticator-sovelluksen usein](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) kysytyt kysymykset usein kysytyistä kysymyksistä ja niiden ratkaisemisesta.
 
**Suositellut videot**

[Authenticator-sovelluksen asentaminen uuteen puhelimeen (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
