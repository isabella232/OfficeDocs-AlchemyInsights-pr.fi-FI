---
title: Sovellusten suojauskäytäntö
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423601"
---
# <a name="application-protection-policy"></a><span data-ttu-id="5386b-102">Sovellusten suojauskäytäntö</span><span class="sxs-lookup"><span data-stu-id="5386b-102">Application protection policy</span></span>

<span data-ttu-id="5386b-103">Jos et ole uusi sovellussuojauskäytännössä (APP), tutustu [sovelluksen suojauskäytäntöjen yleiskatsaukseen](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="5386b-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="5386b-104">Lisätietoja APP:n käyttämisestä on ohjeaiheessa [Sovellusten suojauskäytäntöjen luominen ja määrittäminen](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="5386b-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="5386b-105">Sovellusten suojauskäytännöt:</span><span class="sxs-lookup"><span data-stu-id="5386b-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="5386b-106">Käyttäjällä on Intune- tai EMS-lisenssi.</span><span class="sxs-lookup"><span data-stu-id="5386b-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="5386b-107">Käyttäjä kuuluu sovellussuojauskäytäntöjen kohteena oleviin ryhmään.</span><span class="sxs-lookup"><span data-stu-id="5386b-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="5386b-108">Vain yksi yrityksen käyttäjä on kirjautunut suojattuihin sovelluksiin laitteessa.</span><span class="sxs-lookup"><span data-stu-id="5386b-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="5386b-109">Sovellus on toteuttanut [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="5386b-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="5386b-110">Luettelo SDK:ta tukemista sovelluksista on [ohjeaiheessa Microsoft Intune -suojatut sovellukset](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="5386b-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="5386b-111">Käytännöt ovat voimassa sen jälkeen, kun käyttäjä, joka täyttää edellä mainitut vaatimukset, kirjautuu Intune SDK -yhteensopivaan sovellukseen.</span><span class="sxs-lookup"><span data-stu-id="5386b-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="5386b-112">Helpoin tapa määrittää, käytetäänkö käytäntöä, on se, että käyttäjä asettaa käytännössä nastan.</span><span class="sxs-lookup"><span data-stu-id="5386b-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="5386b-113">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="5386b-113">For more information, see:</span></span>

[<span data-ttu-id="5386b-114">APP/MAM-vianmäärityksen usein kysytyt kysymykset</span><span class="sxs-lookup"><span data-stu-id="5386b-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="5386b-115">Sovelluksen suojauskäytännön asetusten vahvistaminen</span><span class="sxs-lookup"><span data-stu-id="5386b-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="5386b-116">Tietoja sovellusten suojauskäytännön toimitusajoistimista</span><span class="sxs-lookup"><span data-stu-id="5386b-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="5386b-117">Sovellusten suojauskäytäntöjen valvonta</span><span class="sxs-lookup"><span data-stu-id="5386b-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)