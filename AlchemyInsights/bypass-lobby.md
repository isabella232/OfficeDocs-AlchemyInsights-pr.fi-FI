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
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "37654253"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="4d8a6-102">Hallitse aulan asetuksia ja osallistumis tasoa</span><span class="sxs-lookup"><span data-stu-id="4d8a6-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="4d8a6-103">Jos haluat sallia kaikkien, mukaan lukien Puhelin verkko-, ulkoiset ja anonyymit käyttäjät, ohittaa aulan, voit tehdä sen PowerShellin avulla.</span><span class="sxs-lookup"><span data-stu-id="4d8a6-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="4d8a6-104">Tässä on esimerkki organisaation maailmanlaajuisen koko uksen käytännön muuttamisesta:</span><span class="sxs-lookup"><span data-stu-id="4d8a6-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="4d8a6-105">Tämä cmdlet-komento edellyttää tällä hetkellä Skype for Business PowerShell-moduulin käyttöä.</span><span class="sxs-lookup"><span data-stu-id="4d8a6-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="4d8a6-106">Jos haluat saada asennus ohjelman käyttämään tätä cmdlet-komentoa, tutustu [käytäntöjen hallintaan PowerShellin kautta](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="4d8a6-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="4d8a6-107">Voit määrittää uuden käytännön, jota sinun on sitten sovellettava käyttäjiin.</span><span class="sxs-lookup"><span data-stu-id="4d8a6-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="4d8a6-108">Jos muokkaat yleistä käytäntöä, se koskee käyttäjiä automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="4d8a6-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="4d8a6-109">Jos haluat muuttaa käytäntöä, sinun on odotettava vähintään 4 tuntia ja enintään 24 tuntia, jotta käytännöt tulevat voimaan.</span><span class="sxs-lookup"><span data-stu-id="4d8a6-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="4d8a6-110">Muista tarkistaa alla olevat ohjeet ennen muutosten tekemistä, jotta ymmärrät tarkalleen, mitä tämä sallii.</span><span class="sxs-lookup"><span data-stu-id="4d8a6-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="4d8a6-111">Tietoja tiimien koko uksen aulan käytännön valvonnasta</span><span class="sxs-lookup"><span data-stu-id="4d8a6-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="4d8a6-112">[Henkilöiden automaattinen myöntäjä](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) on järjestäjäkohtainen käytäntö, joka ohjaa sitä, liittytäänkö koko ukseen suoraan vai odotetaanko sitä aulassa, kunnes todennettu käyttäjä on myöntänyt heidät.</span><span class="sxs-lookup"><span data-stu-id="4d8a6-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="4d8a6-113">[Nimettömät henkilöt voivat aloittaa koko uksen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , on järjestäjäkohtainen käytäntö, joka ohjaa sitä, voivatko anonyymit henkilöt, mukaan lukien B2B-ja Federated-käyttäjät, liittyä käyttäjän koko ukseen ilman organisaation todennetun käyttäjän läsnäoloa.</span><span class="sxs-lookup"><span data-stu-id="4d8a6-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="4d8a6-114">[Salli dial-in-käyttäjien ohittaa aula](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**tulossa pian**) on järjestäjäkohtainen käytäntö, joka ohjaa sitä, liittääkö Puhelin puhelimitse suoraan koko ukseen vai odottaako se aulan automaattisesti, riippumatta siitä, sallitaanko **ihmiset** -asetus.</span><span class="sxs-lookup"><span data-stu-id="4d8a6-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="4d8a6-115">[Salli järjestäjien ohittaa aulan asetukset](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**tulossa pian**) on järjestäjäkohtainen käytäntö, joka määrittää, voiko koko uksen järjestäjä ohittaa aulan asetukset, jotka järjestelmänvalvoja asettaa **automaattisesti myöntämään ihmisiä** ja **sallimaan soiton käyttäjiä ohittamaan aulan** , kun he aikatauluttaa uuden koko uksen.</span><span class="sxs-lookup"><span data-stu-id="4d8a6-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="4d8a6-116">**Huom:** Lue [teams-Kokous käytäntöjen hallinta](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , niin saat yleiskatsauksen Microsoft teams-Kokous käytännöistä.</span><span class="sxs-lookup"><span data-stu-id="4d8a6-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
