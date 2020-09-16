---
title: Kokous käytäntöjen asetukset
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794331"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="dabe6-102">Kokous käytäntöjen hallinta Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="dabe6-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="dabe6-103">**Huomautus: käytäntöjen muutokset voivat kestää jopa 24 tuntia, ennen kuin käyttäjät astuvat voimaan.**</span><span class="sxs-lookup"><span data-stu-id="dabe6-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="dabe6-104">Et ehkä voi tehdä muutoksia juuri luotuihin käytäntöihin välittömästi. Odota neljä tuntia ja yritä muokata juuri luotua käytäntöä uudelleen.</span><span class="sxs-lookup"><span data-stu-id="dabe6-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="dabe6-105">Kokous käytäntöjen avulla voit hallita koko uksen osallistujien käytettävissä olevia koko uksia, jotka organisaation käyttäjät ovat ajoittanut.</span><span class="sxs-lookup"><span data-stu-id="dabe6-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="dabe6-106">Joitain Kokous käytäntöjen ominaisuuksia ei ehkä ole vielä toteutettu teamsin hallinta keskuksessa (ne on merkitty asia kirjoihin "tulossa pian").</span><span class="sxs-lookup"><span data-stu-id="dabe6-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="dabe6-107">Tässä tapa uksessa tai jos saat virhe ilmoituksen, kuten "emme voi päivittää käytäntöä juuri nyt, mutta yritä myöhemmin uudelleen" Microsoft teamsin hallinta keskuksessa, suosittelemme, että käytät PowerShellin avulla teamsin Kokous käytäntöjen luomista tai muokkaamista.</span><span class="sxs-lookup"><span data-stu-id="dabe6-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="dabe6-108">Lisä tietoja Kokous käytännöistä on seuraavissa resursseissa:</span><span class="sxs-lookup"><span data-stu-id="dabe6-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="dabe6-109">Lisä tietoja käytäntöjen luomisesta, muutosten tekemiseen ja käyttäjien määrittämisestä käytäntöön on artikkelissa [Kokous käytäntöjen hallinta tiimeissä](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="dabe6-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="dabe6-110">Jos haluat muuttaa käytäntöjen muutoksia PowerShellin cmdlet-komennolla, tutustu [teamsin PowerShellin yleiskatsaukseen](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="dabe6-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="dabe6-111">Sinun on käytettävä teamsin Kokous käytäntöjen [Skype for Business PowerShell-moduulia](https://www.microsoft.com/download/details.aspx?id=39366) .</span><span class="sxs-lookup"><span data-stu-id="dabe6-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="dabe6-112">Lisä tietoja on [\*-csteamsmeetingpolicy-cmdlet-ohjeissa](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="dabe6-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

