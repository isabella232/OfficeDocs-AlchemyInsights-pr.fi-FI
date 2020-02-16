---
title: Kokouskäytännön asetukset
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042841"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="2bdbe-102">Kokouskäytäntöjen hallinta Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="2bdbe-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="2bdbe-103">**Huomautus: Käytäntömuutosten voimaantulo käyttäjille voi kestää jopa 24 tuntia.**</span><span class="sxs-lookup"><span data-stu-id="2bdbe-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="2bdbe-104">Et ehkä voi tehdä muutoksia uusiin käytäntöihin välittömästi. odota 4 tuntia ja yritä muokata juuri luotua käytäntöä uudelleen.</span><span class="sxs-lookup"><span data-stu-id="2bdbe-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="2bdbe-105">Kokouskäytäntöjen avulla hallitaan ominaisuuksia, jotka ovat kokouksen osallistujien käytettävissä organisaation käyttäjien ajoittamien kokousten aikana.</span><span class="sxs-lookup"><span data-stu-id="2bdbe-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="2bdbe-106">Joitakin kokouskäytäntöjen ominaisuuksia ei ehkä ole vielä otettu käyttöön Teams-hallintakeskuksessa (niiden dokumentaatiossa lukee "tulossa pian").</span><span class="sxs-lookup"><span data-stu-id="2bdbe-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="2bdbe-107">Tässä tapauksessa tai jos saat Microsoft Teams -hallintakeskuksen virheen, kuten "Emme voi päivittää käytäntöä juuri nyt, mutta yritä sitä myöhemmin uudelleen", microsoft suosittelee, että luot tai muokkaat Teamsin kokouskäytäntöjä PowerShellin avulla.</span><span class="sxs-lookup"><span data-stu-id="2bdbe-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="2bdbe-108">Lisätietoja kokouskäytännöistä on seuraavissa resursseissa:</span><span class="sxs-lookup"><span data-stu-id="2bdbe-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="2bdbe-109">Lisätietoja käytäntöjen luomisesta, muutosten tekemisestä ja käyttäjien määrittämisestä käytäntöön on kohdassa [Kokouskäytäntöjen hallinta Teamsissa](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="2bdbe-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="2bdbe-110">Lisätietoja käytäntömuutoksista PowerShellin cmdlet-komennoilla on artikkelissa [Teams PowerShellin yleiskatsaus](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="2bdbe-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="2bdbe-111">Sinun on käytettävä Teamsin kokouskäytäntöjen [Skype for Business PowerShell -moduulia.](https://www.microsoft.com/download/details.aspx?id=39366)</span><span class="sxs-lookup"><span data-stu-id="2bdbe-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="2bdbe-112">Lisätietoja on [\*-CsTeamsMeetingPolicy-cmdlet-komentojen ohjeissa.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="2bdbe-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

