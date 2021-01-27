---
title: Ehdollisen käytön ongelmat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014789"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="22d9e-102">Ehdollisen käytön ongelmat</span><span class="sxs-lookup"><span data-stu-id="22d9e-102">Conditional access issues</span></span>

<span data-ttu-id="22d9e-103">**Kirjautumisen vianmäärityksen ongelmien ratkaiseminen**</span><span class="sxs-lookup"><span data-stu-id="22d9e-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="22d9e-104">Kirjautumisen vianmäärityksen avulla voit selvittää nopeasti, mitä on tapahtunut tai diagnosoida käyttäjien [kirjautumisongelmia:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="22d9e-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="22d9e-105">Käynnistä kirjautumisen vianmääritys.</span><span class="sxs-lookup"><span data-stu-id="22d9e-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="22d9e-106">Etsi analysoitava tapahtuma kirjoittamalla tiedot käyttäjästä, sovelluksesta, kirjautumisajasta, pyyntötunnuksesta tai korrelaatiotunnuksesta.</span><span class="sxs-lookup"><span data-stu-id="22d9e-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="22d9e-107">Tarkista diagnostiikkatulokset, jotka näyttävät, mitä on tapahtunut ja mitä voit tehdä muutosten tekoon (jos muutoksia tarvitaan).</span><span class="sxs-lookup"><span data-stu-id="22d9e-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="22d9e-108">**Kirjautumisen vianmääritysvaiheet**</span><span class="sxs-lookup"><span data-stu-id="22d9e-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="22d9e-109">Siirry Azure AD:n kirjautumissivulle.</span><span class="sxs-lookup"><span data-stu-id="22d9e-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="22d9e-110">Voit suodattaa kirjautumiset käyttäjän, aika-alueen, sovelluksen, tilan, asiakassovelluksen ja niin edelleen.</span><span class="sxs-lookup"><span data-stu-id="22d9e-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="22d9e-111">Valitse kirjautumistapahtuma ja tarkastele Ehdollinen käyttöoikeus -välilehteä nähdäksesi, mitkä käytännöt on arvioitu.</span><span class="sxs-lookup"><span data-stu-id="22d9e-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="22d9e-112">Napsauta käytännön riviä, jotta näet käytännön tiedot ja ymmärrät, miksi sitä on käytetty.</span><span class="sxs-lookup"><span data-stu-id="22d9e-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="22d9e-113">**Työkalut ehdollisen käytön käytännön vianmääritykseen**</span><span class="sxs-lookup"><span data-stu-id="22d9e-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="22d9e-114">Vain raportti -tilassa voit arvioida käytäntöä vaikuttamatta käyttäjiin.</span><span class="sxs-lookup"><span data-stu-id="22d9e-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="22d9e-115">Entä jos -työkalun avulla voit jäljitellä kirjautumistapahtumia ja nähdä, mitä käytäntöjä sovelletaan.</span><span class="sxs-lookup"><span data-stu-id="22d9e-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="22d9e-116">Insights- ja Reporting-työkirja näyttää kunkin käytännön reaaliaikaisen vaikutuksen.</span><span class="sxs-lookup"><span data-stu-id="22d9e-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="22d9e-117">**Perusaikataulun suojauskäytännöt**</span><span class="sxs-lookup"><span data-stu-id="22d9e-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="22d9e-118">Perusaikataulun suojauskäytännöt on poistettu käytöstä.</span><span class="sxs-lookup"><span data-stu-id="22d9e-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="22d9e-119">Niitä ei enää pakoteta, ja ne poistetaan pian Azure-portaalista.</span><span class="sxs-lookup"><span data-stu-id="22d9e-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="22d9e-120">Suosittelemme, että otat [suojauksen oletusasetukset käyttöön.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="22d9e-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="22d9e-121">Lisätietoja ehdollisesta käyttöoikeussta on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="22d9e-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="22d9e-122">[Ehdollisen käyttöoikeuden parhaat käytännöt Azure Active Directoryssa](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ehdollisen käyttöoikeuden ehdot](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ehdollisen käyttöoikeuden ohjausobjektit](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Sijainnit ehdollisessa käyttöomme](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="22d9e-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
