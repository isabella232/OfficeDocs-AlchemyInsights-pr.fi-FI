---
title: Ehdollisen käytön valvominen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366425"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="22b4e-102">Ehdollisen Exchange-yhteyden valvonta</span><span class="sxs-lookup"><span data-stu-id="22b4e-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="22b4e-103">Ehdolliseen käyttöön kohdistetut käyttäjät saavat ilmoitus Sähkö posti viestin, jos he eivät täytä organisaatiosi käyttö oikeus vaatimuksia.</span><span class="sxs-lookup"><span data-stu-id="22b4e-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="22b4e-104">Ratkaisu on suositeltava vähintään yksi seuraavista ratkaisuista:</span><span class="sxs-lookup"><span data-stu-id="22b4e-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="22b4e-105">Jos laitteen oletetaan olevan rekisteröity, kehota käyttäjää siirtymään yritys portaali-sovellukseen ja vahvistamaan, että se näkyy yritys portaalissa.</span><span class="sxs-lookup"><span data-stu-id="22b4e-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="22b4e-106">Jos näin ei tapahdu, käyttäjän on rekisteröitävä laite.</span><span class="sxs-lookup"><span data-stu-id="22b4e-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="22b4e-107">Valitse Azure-portaalissa Intune-> laite yhteensopivuus.</span><span class="sxs-lookup"><span data-stu-id="22b4e-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="22b4e-108">Valitse näyttö-kohdassa laitteen yhteensopivuus.</span><span class="sxs-lookup"><span data-stu-id="22b4e-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="22b4e-109">Tarkastele laitteesi yhteensopivuus raporttia varmistaaksesi, että käyttäjän laite on merkitty yhteensopivaksi.</span><span class="sxs-lookup"><span data-stu-id="22b4e-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="22b4e-110">Valitse Azure-portaalissa Intune-> laite yhteensopivuus.</span><span class="sxs-lookup"><span data-stu-id="22b4e-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="22b4e-111">Valitse hallinta-kohdassa käytännöt.</span><span class="sxs-lookup"><span data-stu-id="22b4e-111">Under Manage, click Policies.</span></span> <span data-ttu-id="22b4e-112">Varmista yhteensopivuus käytäntöjen luettelosta, että profiili on määritetty käyttäjän laitteelle.</span><span class="sxs-lookup"><span data-stu-id="22b4e-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="22b4e-113">Jos profiilia ei ole määritetty, Intune ei pysty vahvistamaan laitteen yhteensopivuus tilaa.</span><span class="sxs-lookup"><span data-stu-id="22b4e-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="22b4e-114">Muokkaa käyttäjän ehdollisen käytön määritystä.</span><span class="sxs-lookup"><span data-stu-id="22b4e-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="22b4e-115">Valitse Azure-portaalissa **Intune**-  >  **ehdollisen käytön**  >  **käytännöt**.</span><span class="sxs-lookup"><span data-stu-id="22b4e-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="22b4e-116">Valitse luettelosta haluamasi käytännöt.</span><span class="sxs-lookup"><span data-stu-id="22b4e-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="22b4e-117">Valitse käyttäjät ja ryhmät.</span><span class="sxs-lookup"><span data-stu-id="22b4e-117">Click Users and groups.</span></span>
4. <span data-ttu-id="22b4e-118">Jos haluat kohdentaa tiettyyn käytäntöön jollekulle, lisää ne Sisällytä-luetteloon.</span><span class="sxs-lookup"><span data-stu-id="22b4e-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="22b4e-119">Jos haluat varmistaa, että henkilö jätetään pois käytännöstä, Lisää hänet jätä pois-luetteloon.</span><span class="sxs-lookup"><span data-stu-id="22b4e-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="22b4e-120">Hyödyllisiä linkkejä:</span><span class="sxs-lookup"><span data-stu-id="22b4e-120">Helpful links:</span></span>

[<span data-ttu-id="22b4e-121">Laitteen yhteensopivuuden yleiskatsaus</span><span class="sxs-lookup"><span data-stu-id="22b4e-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="22b4e-122">Varmenteiden myöntäjän vian määritys</span><span class="sxs-lookup"><span data-stu-id="22b4e-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="22b4e-123">Vian määritys käytännöt</span><span class="sxs-lookup"><span data-stu-id="22b4e-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="22b4e-124">Intune-laitteen yhteensopivuuden valvonta</span><span class="sxs-lookup"><span data-stu-id="22b4e-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="22b4e-125">Huomautus: näistä vaiheista on hyötyä vain Azure Active Directory-ominaisuus ehdollisen käytön vian määrityksessä.</span><span class="sxs-lookup"><span data-stu-id="22b4e-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="22b4e-126">On myös mahdollista eristää laite, joka estää sähkö postin käytön Exchange-käytännöllä.</span><span class="sxs-lookup"><span data-stu-id="22b4e-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="22b4e-127">Lisä tietoja Exchange Device managementä on [täällä](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="22b4e-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
