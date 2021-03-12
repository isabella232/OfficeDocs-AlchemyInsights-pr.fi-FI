---
title: Ehdollisen käyttöoikeuden valvonta
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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708671"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="32603-102">Ehdollisen käyttöoikeuden valvonta Exchangessa</span><span class="sxs-lookup"><span data-stu-id="32603-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="32603-103">Käyttäjät, joilla on ehdollinen käyttöoikeus, saavat sähköposti-ilmoituksen, jos he eivät täytä organisaatiosi käyttöoikeusvaatimuksia.</span><span class="sxs-lookup"><span data-stu-id="32603-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="32603-104">Ratkaisua varten suosittelemme vähintään yhtä seuraavista ratkaisuista:</span><span class="sxs-lookup"><span data-stu-id="32603-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="32603-105">Jos laitteen oletetaan olevan rekisteröity, kehota käyttäjää menemään Yritysportaali-sovellukseen ja tarkistamaan, että se näkyy yritysportaalissa.</span><span class="sxs-lookup"><span data-stu-id="32603-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="32603-106">Jos näin ei ole, käyttäjän tulisi rekisteröidä laite.</span><span class="sxs-lookup"><span data-stu-id="32603-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="32603-107">Valitse Azure-portaalissa Intune > laitteen yhteensopivuus.</span><span class="sxs-lookup"><span data-stu-id="32603-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="32603-108">Valitse Näyttö-kohdassa Laitteen yhteensopivuus.</span><span class="sxs-lookup"><span data-stu-id="32603-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="32603-109">Tarkista laitteen yhteensopivuusraportista, että käyttäjän laite on merkitty yhteensopivaksi.</span><span class="sxs-lookup"><span data-stu-id="32603-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="32603-110">Valitse Azure-portaalissa Intune > laitteen yhteensopivuus.</span><span class="sxs-lookup"><span data-stu-id="32603-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="32603-111">Valitse Hallinta-kohdassa Käytännöt.</span><span class="sxs-lookup"><span data-stu-id="32603-111">Under Manage, click Policies.</span></span> <span data-ttu-id="32603-112">Tarkista yhteensopivuuskäytäntöjen luettelosta, että profiili on määritetty käyttäjän laitteelle.</span><span class="sxs-lookup"><span data-stu-id="32603-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="32603-113">Jos profiilia ei ole määritetty, Intune ei voi vahvistaa laitteen yhteensopivuustilaa.</span><span class="sxs-lookup"><span data-stu-id="32603-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="32603-114">Muokkaa käyttäjän ehdollisen käyttöoikeuden määritystä.</span><span class="sxs-lookup"><span data-stu-id="32603-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="32603-115">Valitse Azure-portaalissa   >  **Intune-ehdollisen käytön**  >  **käytännöt.**</span><span class="sxs-lookup"><span data-stu-id="32603-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="32603-116">Valitse käytäntö luettelosta.</span><span class="sxs-lookup"><span data-stu-id="32603-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="32603-117">Valitse Käyttäjät ja ryhmät.</span><span class="sxs-lookup"><span data-stu-id="32603-117">Click Users and groups.</span></span>
4. <span data-ttu-id="32603-118">Jos haluat kohdistaa tietyn käytännön jollekulle, lisää hänet Sisällytä-luetteloon.</span><span class="sxs-lookup"><span data-stu-id="32603-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="32603-119">Jos haluat varmistaa, että henkilö jätetään pois käytännön ulkopuolelle, lisää hänet Poissulkeminen-luetteloon.</span><span class="sxs-lookup"><span data-stu-id="32603-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="32603-120">Hyödyllisiä linkkejä:</span><span class="sxs-lookup"><span data-stu-id="32603-120">Helpful links:</span></span>

[<span data-ttu-id="32603-121">Laitteen yhteensopivuuden yleiskatsaus</span><span class="sxs-lookup"><span data-stu-id="32603-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="32603-122">Varmenteiden myöntäjän vianmääritys</span><span class="sxs-lookup"><span data-stu-id="32603-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="32603-123">Vianmäärityskäytäntö</span><span class="sxs-lookup"><span data-stu-id="32603-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="32603-124">Intune-laitteen yhteensopivuuden valvonta</span><span class="sxs-lookup"><span data-stu-id="32603-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="32603-125">Huomautus: näistä ohjeista on hyötyä vain Azure Active Directory -ominaisuuden ehdollisen käyttöoikeuden vianmäärityksessä.</span><span class="sxs-lookup"><span data-stu-id="32603-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="32603-126">On myös mahdollista asettaa karanteeniin laite, joka estää sähköpostin käytön Exchange-käytännön avulla.</span><span class="sxs-lookup"><span data-stu-id="32603-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="32603-127">Lisätietoja Exchange-laitehallinnasta on [täällä]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="32603-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
