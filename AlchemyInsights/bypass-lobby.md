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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376621"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="9f73b-102">Hallitse aulan asetuksia ja osallistumis tasoa</span><span class="sxs-lookup"><span data-stu-id="9f73b-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="9f73b-103">Nämä asetukset ohjaavat sitä, ketkä osallistujat odottavat aulassa ennen kuin heidät otetaan mukaan koko ukseen ja kuinka suuri osallistumis aste he saavat koko uksessa.</span><span class="sxs-lookup"><span data-stu-id="9f73b-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="9f73b-104">Voit käyttää PowerShelliä päivittämään Kokous käytäntö asetukset, joita ei ole vielä toteutettu (merkitty "tulossa pian") teams-hallinta keskukseen.</span><span class="sxs-lookup"><span data-stu-id="9f73b-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="9f73b-105">Katso alla esimerkki PowerShell cmdlet, jonka avulla kaikki käyttäjät voivat ohittaa aulan.</span><span class="sxs-lookup"><span data-stu-id="9f73b-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="9f73b-106">[Henkilöiden automaattinen myöntäjä](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) on järjestäjäkohtainen käytäntö, joka ohjaa sitä, liittytäänkö koko ukseen suoraan vai odotetaanko sitä aulassa, kunnes todennettu käyttäjä on myöntänyt heidät.</span><span class="sxs-lookup"><span data-stu-id="9f73b-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="9f73b-107">[Nimettömät henkilöt voivat aloittaa koko uksen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , on järjestäjäkohtainen käytäntö, joka ohjaa sitä, voivatko anonyymit henkilöt, mukaan lukien B2B-ja Federated-käyttäjät, liittyä käyttäjän koko ukseen ilman organisaation todennetun käyttäjän läsnäoloa.</span><span class="sxs-lookup"><span data-stu-id="9f73b-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="9f73b-108">[Salli dial-in-käyttäjien ohittaa aula](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**tulossa pian**) on järjestäjäkohtainen käytäntö, joka ohjaa sitä, liittääkö Puhelin puhelimitse suoraan koko ukseen vai odottaako se aulan automaattisesti, riippumatta siitä, sallitaanko **ihmiset** -asetus.</span><span class="sxs-lookup"><span data-stu-id="9f73b-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="9f73b-109">[Salli järjestäjien ohittaa aulan asetukset](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**tulossa pian**) on järjestäjäkohtainen käytäntö, joka määrittää, voiko koko uksen järjestäjä ohittaa aulan asetukset, jotka järjestelmänvalvoja asettaa **automaattisesti myöntämään ihmisiä** ja **sallimaan soiton käyttäjiä ohittamaan aulan** , kun he aikatauluttaa uuden koko uksen.</span><span class="sxs-lookup"><span data-stu-id="9f73b-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="9f73b-110">**Huom:** Lue [teams-Kokous käytäntöjen hallinta](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , niin saat yleiskatsauksen Microsoft teams-Kokous käytännöistä.</span><span class="sxs-lookup"><span data-stu-id="9f73b-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="9f73b-111">**PowerShell-esimerkki**</span><span class="sxs-lookup"><span data-stu-id="9f73b-111">**PowerShell example**</span></span>

<span data-ttu-id="9f73b-112">Jos haluat sallia kaikkien, myös ulkoisten tai anonyymien käyttäjien, ohittaa aulan, voit myös käyttää PowerShelliä tämän tehtävän suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="9f73b-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="9f73b-113">Tässä on esimerkki organisaation maailmanlaajuisen Kokous käytännön muuttamisesta.</span><span class="sxs-lookup"><span data-stu-id="9f73b-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="9f73b-114">(Muista tarkistaa edellä mainitut ohjeet ennen muutosten tekemistä, jotta ymmärrät tarkalleen, mitä tämä sallii.)</span><span class="sxs-lookup"><span data-stu-id="9f73b-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="9f73b-115">Set-CsTeamsMeetingPolicy-identiteetti Global-Autosisääntulokäyttäjät "kaikki"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="9f73b-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="9f73b-116">Lisä tietoja on kohdassa [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="9f73b-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
