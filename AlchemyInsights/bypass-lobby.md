---
title: Ohitusaula
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820031"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="788e5-102">Hallita aula-asetuksia ja osallistumisen tasoa Teamsissa</span><span class="sxs-lookup"><span data-stu-id="788e5-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="788e5-103">Jos haluat, että kaikki, kuten puhelinneuvottelut, ulkoiset ja anonyymit käyttäjät, voivat ohittaa aulan **,** käytä PowerShelliä tämän tehtävän suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="788e5-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="788e5-104">Seuraavassa on esimerkki organisaation yleisen kokouskäytännön muokkaamisesta.</span><span class="sxs-lookup"><span data-stu-id="788e5-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="788e5-105">Tämä cmdlet-komento edellyttää tällä hetkellä Skype for Business PowerShell -moduulin käyttöä.</span><span class="sxs-lookup"><span data-stu-id="788e5-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="788e5-106">Jos haluat määrittää tämän cmdlet-komennon käyttöön, lue kohta Policies [via PowerShell (Hallitse käytäntöjä PowerShellin kautta).](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="788e5-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="788e5-107">Kun olet määrittänyt käytännön, sinun on sovellettava sitä käyttäjiin. tai jos olet muokannut global-käytäntöä, se koskee automaattisesti käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="788e5-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="788e5-108">Jos käytäntö muuttuu, sinun on odotettava vähintään 4 tuntia **ja 24** tuntia, ennen kuin käytännöt tulevat voimaan.</span><span class="sxs-lookup"><span data-stu-id="788e5-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="788e5-109">Muista tarkistaa alla olevat ohjeet ennen muutosten tekeminen, jotta ymmärrät tarkalleen, mitä tämä sallii.</span><span class="sxs-lookup"><span data-stu-id="788e5-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="788e5-110">Teamsin kokouksen aulakäytännön hallinta</span><span class="sxs-lookup"><span data-stu-id="788e5-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="788e5-111">Näillä asetuksilla voit määrittää, mitkä kokouksen osallistujat odottavat odotustilassa, ennen kuin heidät hyväksytään kokoukseen, ja osallistujat voivat osallistua kokoukseen.</span><span class="sxs-lookup"><span data-stu-id="788e5-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="788e5-112">PowerShellin avulla voit päivittää kokouskäytäntöasetuksia, joita ei ole vielä otettu käyttöön (tulossa pian) Teams-hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="788e5-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="788e5-113">Alla on esimerkki PowerShell-cmdlet-komennosta, jonka avulla kaikki käyttäjät voivat ohittaa aulan.</span><span class="sxs-lookup"><span data-stu-id="788e5-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="788e5-114">[Hyväksy henkilöt automaattisesti](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) järjestäjän mukaan -käytäntö, joka määrittää, liittyvätkö henkilöt kokoukseen suoraan vai odottavat odotustilassa, kunnes todennettu käyttäjä on myöntänyt heidät sisään.</span><span class="sxs-lookup"><span data-stu-id="788e5-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="788e5-115">[Salli anonyymien](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) käyttäjien aloittaa kokous on järjestäjäkohtainen käytäntö, joka määrittää, voivatko anonyymit henkilöt, mukaan lukien B2B- ja liitetyt käyttäjät, liittyä käyttäjän kokoukseen ilman organisaation todennettua käyttäjää.</span><span class="sxs-lookup"><span data-stu-id="788e5-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="788e5-116">[Salli puhelinkäyttäjien](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) ohittaa odotustila **(tulossa** pian) on järjestäjäkohtainen käytäntö, joka määrittää, liittyvätkö puhelinyhteyden kautta soittavat henkilöt kokoukseen suoraan vai odottavat odotustilassa Hyväksy henkilöt automaattisesti **-asetuksen** välittämisen väliltä.</span><span class="sxs-lookup"><span data-stu-id="788e5-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="788e5-117">[Salli järjestäjien](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) ohittaa aula-asetukset **(tulossa** pian) on järjestäjäkohtainen käytäntö, joka määrittää, voiko  kokouksen järjestäjä  ohittaa aula-asetukset, jotka järjestelmänvalvoja on määrittänyt asetuksissa Hyväksy käyttäjät automaattisesti ja Salli puhelinkäyttäjien ohittaa aula, kun he ajoittavat uuden kokouksen.</span><span class="sxs-lookup"><span data-stu-id="788e5-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="788e5-118">**Huomautus:** Lue [kokouskäytäntöjen hallinta Teamsissa,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) niin saat täydellisen yleiskatsauksen Microsoft Teams -kokouskäytännöistä.</span><span class="sxs-lookup"><span data-stu-id="788e5-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
