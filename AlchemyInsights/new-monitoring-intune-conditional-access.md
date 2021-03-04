---
title: Intunen ehdollisen käyttöoikeuden valvonta
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427426"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="41e72-102">Intunen ehdollisen käyttöoikeuden valvonta</span><span class="sxs-lookup"><span data-stu-id="41e72-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="41e72-103">Käyttäjät, joilla on ehdollinen käyttöoikeus, saavat sähköposti-ilmoituksen, jos he eivät täytä organisaatiosi käyttöoikeusvaatimuksia.</span><span class="sxs-lookup"><span data-stu-id="41e72-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="41e72-104">Ratkaisua varten suosittelemme vähintään yhtä seuraavista ratkaisuista:</span><span class="sxs-lookup"><span data-stu-id="41e72-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="41e72-105">Jos laitteen oletetaan olevan rekisteröity, kehota käyttäjää menemään Yritysportaali-sovellukseen ja tarkistamaan, että se näkyy yritysportaalissa.</span><span class="sxs-lookup"><span data-stu-id="41e72-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="41e72-106">Jos näin ei ole, käyttäjän on rekisteröittävä laite.</span><span class="sxs-lookup"><span data-stu-id="41e72-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="41e72-107">Valitse Azure-portaalissa **Intune-laitteen**  >  **yhteensopivuus.**</span><span class="sxs-lookup"><span data-stu-id="41e72-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="41e72-108">Voit tarkastella laitteen yhteensopivuusraporttia sen varmistamiseksi, että käyttäjän laite on merkitty **yhteensopivaksi,** valitsemalla Seuraa-kohdassa Laitteen yhteensopivuus.</span><span class="sxs-lookup"><span data-stu-id="41e72-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="41e72-109">Valitse Azure-portaalissa **Intune-laitteen**  >  **yhteensopivuus.**</span><span class="sxs-lookup"><span data-stu-id="41e72-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="41e72-110">Valitse **Hallinta-kohdassa** **Käytännöt.**</span><span class="sxs-lookup"><span data-stu-id="41e72-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="41e72-111">Tarkista yhteensopivuuskäytäntöjen luettelosta, että profiili on määritetty käyttäjän laitteelle.</span><span class="sxs-lookup"><span data-stu-id="41e72-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="41e72-112">Jos profiilia ei ole määritetty, Intune ei voi vahvistaa laitteen yhteensopivuustilaa.</span><span class="sxs-lookup"><span data-stu-id="41e72-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="41e72-113">Muokkaa käyttäjän ehdollisen käyttöoikeuden määritystä.</span><span class="sxs-lookup"><span data-stu-id="41e72-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="41e72-114">Siirry Azure-portaalissa **Intune-ehdollisen** käytön käytäntöihin, valitse käytäntö luettelosta ja valitse Käyttäjät  >    >   **ja ryhmät.**</span><span class="sxs-lookup"><span data-stu-id="41e72-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="41e72-115">Jos haluat kohdistaa tietyn käytännön jollekulle, lisää hänet **Sisällytä-luetteloon.**</span><span class="sxs-lookup"><span data-stu-id="41e72-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="41e72-116">Jos haluat varmistaa, että henkilö jätetään pois käytännön ulkopuolelle, lisää hänet **Poissulkeminen-luetteloon.**</span><span class="sxs-lookup"><span data-stu-id="41e72-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="41e72-117">**Hyödyllisiä linkkejä:**</span><span class="sxs-lookup"><span data-stu-id="41e72-117">**Helpful links:**</span></span>

- [<span data-ttu-id="41e72-118">Laitteen yhteensopivuuden yleiskatsaus</span><span class="sxs-lookup"><span data-stu-id="41e72-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="41e72-119">Varmenteiden myöntäjän vianmääritys</span><span class="sxs-lookup"><span data-stu-id="41e72-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="41e72-120">Vianmäärityskäytäntö</span><span class="sxs-lookup"><span data-stu-id="41e72-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="41e72-121">Intune-laitteen yhteensopivuuden valvonta</span><span class="sxs-lookup"><span data-stu-id="41e72-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="41e72-122">Näistä ohjeista on hyötyä vain Azure Active Directory -ominaisuuden ehdollisen käyttöoikeuden vianmäärityksessä.</span><span class="sxs-lookup"><span data-stu-id="41e72-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="41e72-123">On myös mahdollista asettaa karanteeniin laite, joka estää sähköpostin käytön Exchange-käytännön avulla.</span><span class="sxs-lookup"><span data-stu-id="41e72-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="41e72-124">Lisätietoja Exchange-laitehallinnasta on [**täällä.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="41e72-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
