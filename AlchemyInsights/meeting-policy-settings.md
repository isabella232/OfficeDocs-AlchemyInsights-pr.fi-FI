---
title: Koko uksen käytäntö asetukset
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627571"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="08b4f-102">Kokous käytäntöjen hallinta Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="08b4f-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="08b4f-103">Kokous käytäntöjä käytetään sellaisten toimintojen hallintaan, jotka ovat osallistujien organisaation käyttäjien aikatauluttamien kokousten osanottajien käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="08b4f-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="08b4f-104">Joitakin Kokous käytäntöjen ominaisuuksia ei ehkä ole vielä toteutettu teams-hallinta keskuksessa (nämä on merkitty "tulossa pian" dokumentaatiossa).</span><span class="sxs-lookup"><span data-stu-id="08b4f-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="08b4f-105">Tässä tapa uksessa tai jos saat virheen, kuten "emme voi päivittää käytäntöä juuri nyt, mutta kokeilet sitä myöhemmin" Microsoft teams-hallinta keskuksessa, suosittelemme, että luot tai muokkaat teamsin Kokous käytäntöjä PowerShellin avulla.</span><span class="sxs-lookup"><span data-stu-id="08b4f-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="08b4f-106">Lisä tietoja Kokous käytännöistä on seuraavissa resursseissa:</span><span class="sxs-lookup"><span data-stu-id="08b4f-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="08b4f-107">Lisä tietoja käytäntöjen luomisesta, muutosten tekemisestä ja käyttäjien määrittämisestä käytäntöön on kohdassa [Kokous käytäntöjen hallinta teamsissa](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="08b4f-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="08b4f-108">Jos haluat tehdä käytäntö muutoksia PowerShellin cmdlet-komentojen avulla, katso [teams PowerShell-yleiskatsaus](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="08b4f-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="08b4f-109">Sinun on käytettävä [Skype for Business PowerShell-moduulia](https://www.microsoft.com/download/details.aspx?id=39366) teams-Kokous käytäntöihin.</span><span class="sxs-lookup"><span data-stu-id="08b4f-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="08b4f-110">Lisä tietoja on [\*-csteamsmeetingpolicy cmdlet-ohjeissa](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="08b4f-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="08b4f-111">**Huom:** Käytännön muutosten vaikutus käyttäjiin voi kestää jopa 24 tuntia.</span><span class="sxs-lookup"><span data-stu-id="08b4f-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="08b4f-112">Et ehkä voi tehdä muutoksia äskettäin luotuihin käytäntöihin välittömästi. Odota 4 tuntia ja yritä muokata juuri luotua käytäntöä uudelleen.</span><span class="sxs-lookup"><span data-stu-id="08b4f-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="08b4f-113">Jos ongelmia ei vieläkään ole, kokeile PowerShelliä.</span><span class="sxs-lookup"><span data-stu-id="08b4f-113">If you're still having problems, try PowerShell.</span></span>  