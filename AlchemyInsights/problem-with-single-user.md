---
title: Ongelma yksittäisen käyttäjän kanssa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429712"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="c8abf-102">Ongelma yksittäisen käyttäjän kanssa</span><span class="sxs-lookup"><span data-stu-id="c8abf-102">Problem with single user</span></span>

- <span data-ttu-id="c8abf-103">Käyttäjää ei ehkä ole valmistettu, koska palvelussa ei ole vielä ollut mahdollisuutta arvioida käyttäjää.</span><span class="sxs-lookup"><span data-stu-id="c8abf-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="c8abf-104">Tutustu valmistelun määrityssivun ohjeisiin sekä edistymispalkkiin.</span><span class="sxs-lookup"><span data-stu-id="c8abf-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="c8abf-105">Jos lisätiedot-osassa määritetty tasainen tila on ennen käyttäjän luonti-, päivitys- tai poistamispäivää, se tarkoittaa, että käyttäjää ei ole vielä arvioitu.</span><span class="sxs-lookup"><span data-stu-id="c8abf-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="c8abf-106">Tässä skenaariossa on parasta odottaa valmistelupalvelun valmistumista.</span><span class="sxs-lookup"><span data-stu-id="c8abf-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="c8abf-107">Huomaa, että palvelumme on tietoinen vain lähdejärjestelmän (Cloud HR) käyttäjälle muutoksista.</span><span class="sxs-lookup"><span data-stu-id="c8abf-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="c8abf-108">Azure AD:n lähdejärjestelmässä on oltava kelvollinen muutos, jotta se voidaan tunnistaa ja se voidaan sitten työnkulun jälkeen käyttää Active Directorya.</span><span class="sxs-lookup"><span data-stu-id="c8abf-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="c8abf-109">Valmistelupalvelu on arvioinut käyttäjän ja todennut, ettei sitä tule valmistella:</span><span class="sxs-lookup"><span data-stu-id="c8abf-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="c8abf-110">Jos olet määrittänyt määritepohjaisen rajaussuodattimen, varmista, että käyttäjä täyttää määrittämäsi ehdot.</span><span class="sxs-lookup"><span data-stu-id="c8abf-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="c8abf-111">Jos käyttäjät ovat jo kohdejärjestelmässä ja käyttäjän tila lähde- ja kohde vastineissa, emme tee mitään lisätoimia.</span><span class="sxs-lookup"><span data-stu-id="c8abf-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="c8abf-112">Valmistelupalvelu yritti valmistella käyttäjää, ja se epäonnistui.</span><span class="sxs-lookup"><span data-stu-id="c8abf-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="c8abf-113">Tutustu näissä tilanteissa valmistelulokien vianmääritys- ja suositukset-välilehteen:</span><span class="sxs-lookup"><span data-stu-id="c8abf-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="c8abf-114">Käyttäjän pakollinen määrite saattaa puuttua paikallisesta Active Directorysta tai Azure AD:stä.</span><span class="sxs-lookup"><span data-stu-id="c8abf-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="c8abf-115">Esimerkiksi userPrincipalName- tai sAMAccountName-luontisäännöt eivät luo oikeaa arvoa.</span><span class="sxs-lookup"><span data-stu-id="c8abf-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="c8abf-116">Vastaava määrite (yleensä employeeId) ei ratkaise yksilöllistä käyttäjää paikalliselle Active Directorylle tai Azure AD:lle.</span><span class="sxs-lookup"><span data-stu-id="c8abf-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="c8abf-117">Esimerkiksi kahdella käyttäjällä on sama työntekijätunnus AD:ssä, ja palvelu palauttaa virhekoodin, joka osoittaa saman lähdemerkinnän kohdemerkintöjen kaksoiskappaleet.</span><span class="sxs-lookup"><span data-stu-id="c8abf-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="c8abf-118">Jos haluat tarkastella yksittäisen käyttäjän ja ryhmän lokeja, tutustu tietyn käyttäjän ongelmaan tutustumalla [valmistelulokeja.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="c8abf-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
