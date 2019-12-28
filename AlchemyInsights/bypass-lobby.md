---
title: Ohita aula
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889079"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="d510e-102">Hallitse aulan asetuksia ja tiimien osallistumis tasoa</span><span class="sxs-lookup"><span data-stu-id="d510e-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="d510e-103">Jos haluat sallia kaikkien, mukaan lukien Puhelin verkko-, ulkoiset ja anonyymit käyttäjät, **ohittaa aulan**, käytä PowerShelliä tämän tehtävän suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="d510e-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="d510e-104">Tässä on esimerkki organisaation maailmanlaajuisen Kokous käytännön muuttamisesta.</span><span class="sxs-lookup"><span data-stu-id="d510e-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="d510e-105">Tämä cmdlet-komento edellyttää tällä hetkellä Skype for Business PowerShell-moduulin käyttöä.</span><span class="sxs-lookup"><span data-stu-id="d510e-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="d510e-106">Jos haluat määrittää tämän cmdlet-komennolla, tutustu [käytäntöjen hallintaan PowerShellin kautta](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="d510e-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="d510e-107">Kun olet määrittänyt käytännön, sinun on sovellettava sitä käyttäjille; Jos olet muokannut yleistä käytäntöä, se koskee käyttäjiä automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="d510e-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="d510e-108">Jos haluat muuttaa käytäntöä, sinun on odotettava vähintään **4 tuntia 24 tuntiin** , jotta käytännöt tulevat voimaan.</span><span class="sxs-lookup"><span data-stu-id="d510e-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="d510e-109">Muista tarkistaa alla olevat ohjeet ennen muutosten tekemistä, jotta ymmärrät tarkalleen, mitä tämä sallii.</span><span class="sxs-lookup"><span data-stu-id="d510e-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="d510e-110">Tietoja tiimien koko uksen aulan käytännön valvonnasta</span><span class="sxs-lookup"><span data-stu-id="d510e-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="d510e-111">Nämä asetukset ohjaavat sitä, ketkä osallistujat odottavat aulassa ennen kuin heidät otetaan mukaan koko ukseen ja kuinka suuri osallistumis aste he saavat koko uksessa.</span><span class="sxs-lookup"><span data-stu-id="d510e-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="d510e-112">Voit käyttää PowerShelliä päivittämään Kokous käytäntö asetukset, joita ei ole vielä toteutettu (merkitty "tulossa pian") teams-hallinta keskukseen.</span><span class="sxs-lookup"><span data-stu-id="d510e-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="d510e-113">Katso alla esimerkki PowerShell cmdlet, jonka avulla kaikki käyttäjät voivat ohittaa aulan.</span><span class="sxs-lookup"><span data-stu-id="d510e-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="d510e-114">[Henkilöiden automaattinen myöntäjä](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) on järjestäjäkohtainen käytäntö, joka ohjaa sitä, liittytäänkö koko ukseen suoraan vai odotetaanko sitä aulassa, kunnes todennettu käyttäjä on myöntänyt heidät.</span><span class="sxs-lookup"><span data-stu-id="d510e-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="d510e-115">[Nimettömät henkilöt voivat aloittaa koko uksen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , on järjestäjäkohtainen käytäntö, joka ohjaa sitä, voivatko anonyymit henkilöt, mukaan lukien B2B-ja Federated-käyttäjät, liittyä käyttäjän koko ukseen ilman organisaation todennetun käyttäjän läsnäoloa.</span><span class="sxs-lookup"><span data-stu-id="d510e-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="d510e-116">[Salli dial-in-käyttäjien ohittaa aula](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**tulossa pian**) on järjestäjäkohtainen käytäntö, joka ohjaa sitä, liittääkö Puhelin puhelimitse suoraan koko ukseen vai odottaako se aulan automaattisesti, riippumatta siitä, sallitaanko **ihmiset** -asetus.</span><span class="sxs-lookup"><span data-stu-id="d510e-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="d510e-117">[Salli järjestäjien ohittaa aulan asetukset](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**tulossa pian**) on järjestelijä koskeva käytäntö, joka ohjaa sitä, voiko koko uksen järjestäjä ohittaa aulan asetukset, jotka järjestelmänvalvoja asettaa **automaattisesti myöntämään ihmisille** ja **sallia soiton käyttäjien ohittaa aulan** , kun he aikatauluttaa uuden koko uksen.</span><span class="sxs-lookup"><span data-stu-id="d510e-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="d510e-118">**Huom:** Lue [teams-Kokous käytäntöjen hallinta](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , niin saat yleiskatsauksen Microsoft teams-Kokous käytännöistä.</span><span class="sxs-lookup"><span data-stu-id="d510e-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
