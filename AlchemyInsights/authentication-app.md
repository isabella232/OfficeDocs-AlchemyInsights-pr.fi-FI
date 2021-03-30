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
# <a name="authentication-app"></a><span data-ttu-id="24de4-102">Todennussovellus</span><span class="sxs-lookup"><span data-stu-id="24de4-102">Authentication app</span></span>

<span data-ttu-id="24de4-103">Jos olet yleinen järjestelmänvalvoja, voit selvittää nopeasti, mitä on tapahtunut tai diagnosoida käyttäjän sisäänkirjautumisongelmia kirjautumisen [vianmäärityksen avulla.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="24de4-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="24de4-104">Käynnistä vianmääritys napsauttamalla[Käynnistä](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)diagnostiikka -painiketta.</span><span class="sxs-lookup"><span data-stu-id="24de4-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="24de4-105">Etsi analysoitava tapahtuma kirjoittamalla tiedot käyttäjästä, sovelluksesta, kirjautumisajasta, pyyntötunnuksesta tai korrelaatiotunnuksesta.</span><span class="sxs-lookup"><span data-stu-id="24de4-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="24de4-106">Tarkista diagnostiikkatulokset, jotka näyttävät, mitä on tapahtunut ja mitä voit tehdä muutosten tekoon, jos muutoksia tarvitaan.</span><span class="sxs-lookup"><span data-stu-id="24de4-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="24de4-107">**Tarkista soveltuva skenaario:**</span><span class="sxs-lookup"><span data-stu-id="24de4-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="24de4-108">Jos käyttäjä ei saa push-ilmoitusta Microsoft Authenticator -sovelluksessa, varmista, että häntä ei näy MFA:n estettyjen käyttäjien alla kohdassa Käyttäjien estäminen ja eston [poistaminen kuvatulla tavalla.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="24de4-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="24de4-109">Jos käyttäjää ei estetä MFA-todentamista varten, mutta hän ei saa push-ilmoitusta, hän voi avata Microsoft Authenticator -sovelluksen, joka pyytää odottavia hyväksyntäpyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="24de4-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="24de4-110">Vaihtoehtoisena kirjautumismenetelmänä käyttäjä voi myös napsauttaa Kirjaudu sisään muulla tavalla ja valita käyttää vahvistuskoodia mobiilisovelluksestani.</span><span class="sxs-lookup"><span data-stu-id="24de4-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="24de4-111">Microsoft Authenticator -sovellus on ainoa käytettävissä oleva menetelmä monille käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="24de4-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="24de4-112">[Lue lisää suojauksen oletusasetuksista,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)tarkista [Authenticator-sovelluksen usein](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) kysytyt kysymykset usein kysytyistä kysymyksistä ja niiden ratkaisemisesta.</span><span class="sxs-lookup"><span data-stu-id="24de4-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="24de4-113">**Suositellut videot**</span><span class="sxs-lookup"><span data-stu-id="24de4-113">**Recommended Videos**</span></span>

<span data-ttu-id="24de4-114">[Authenticator-sovelluksen asentaminen uuteen puhelimeen (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="24de4-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
