---
title: Ilmaisimet eivät toimi Edge-selaimessa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676240"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="1bb03-102">Ilmaisimet eivät toimi Edge-selaimessa</span><span class="sxs-lookup"><span data-stu-id="1bb03-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="1bb03-103">Kun olet luonut ilmaisimen, Edge (Smartscreen) ei ota sitä mukaan.</span><span class="sxs-lookup"><span data-stu-id="1bb03-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="1bb03-104">Lisätietoja on kohdassa ILMAISIMIEN [LUOMINEN IP-osoitteille ja URL-osoitteille/toimialueille.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="1bb03-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="1bb03-105">Vaihe 1: Varmista seuraavat asiat</span><span class="sxs-lookup"><span data-stu-id="1bb03-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="1bb03-106">Varmista, että ilmaisin on oikein (IP-/URL-osoitteessa ei ole kirjoitusvirheitä, oikea toiminto, oikeat RBAC-ryhmät).</span><span class="sxs-lookup"><span data-stu-id="1bb03-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="1bb03-107">Odota vähintään 2 tuntia ilmaisimen luomisen jälkeen, jotta mahdolliset viiveet otetaan huomioon.</span><span class="sxs-lookup"><span data-stu-id="1bb03-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="1bb03-108">Varmista, että järjestelmät onboarded Microsoft Defender for Endpointiin.</span><span class="sxs-lookup"><span data-stu-id="1bb03-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="1bb03-109">Varmista, että järjestelmät voivat viestiä pilvipalvelun kanssa.</span><span class="sxs-lookup"><span data-stu-id="1bb03-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="1bb03-110">Varmista testisivustosta, että Smartscreen on otettu käyttöön ja [tavoitettavissa.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="1bb03-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="1bb03-111">Vaihe 2: Mahdollisen ongelman vianmääritys</span><span class="sxs-lookup"><span data-stu-id="1bb03-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="1bb03-112">Varmista, että asiakas täyttää vaatimukset.</span><span class="sxs-lookup"><span data-stu-id="1bb03-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="1bb03-113">Lisätietoja on kohdassa [ILMAISIMIEN LUOMINEN IP-osoitteille ja URL-osoitteille/toimialueille.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="1bb03-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="1bb03-114">Varmista, että käytössäsi on Edge-selaimen uusin versio.</span><span class="sxs-lookup"><span data-stu-id="1bb03-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="1bb03-115">Lisätietoja uusimmasta versiosta on kohdassa [Käytössäsi Microsoft Edge version selvitäminen.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="1bb03-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="1bb03-116">Käynnistä Edge-selain uudelleen.</span><span class="sxs-lookup"><span data-stu-id="1bb03-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="1bb03-117">Siirry sivustoon, johon olet lisännyt ilmaisimen.</span><span class="sxs-lookup"><span data-stu-id="1bb03-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="1bb03-118">Jos sivusto ei näy odotetulla tavalla, jatka vaiheeseen 3.</span><span class="sxs-lookup"><span data-stu-id="1bb03-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="1bb03-119">Vaihe 3: Tietojen kerääminen</span><span class="sxs-lookup"><span data-stu-id="1bb03-119">Step 3: Collect data</span></span>

- <span data-ttu-id="1bb03-120">Kerää **MDEClientAnalyzerin** diagnostiikkatietoja.</span><span class="sxs-lookup"><span data-stu-id="1bb03-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="1bb03-121">Katso ohjeet ohjeista [Onboarding machines to Microsoft Defender for Endpoint (Onboarding Machinesin ja Microsoft Defender for Endpointin ongelmat).](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="1bb03-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="1bb03-122">Jos olet tutustunut Fiddler-seurantatietojen asentamiseen ja keräämiseen, katso [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="1bb03-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="1bb03-123">Jos haluat ohjeita Microsoft-tuesta, avaa tukipyyntö valitsemalla alla oleva Tuki-kuvake.</span><span class="sxs-lookup"><span data-stu-id="1bb03-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
