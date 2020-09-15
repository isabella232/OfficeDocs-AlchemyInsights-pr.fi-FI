---
title: Ohitus aula
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684947"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="9ae1d-102">Hallitse aulan asetuksia ja osallistumis tasoa tiimeihin</span><span class="sxs-lookup"><span data-stu-id="9ae1d-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="9ae1d-103">Jos haluat, että kaikki käyttäjät, kuten dial-in, External ja Anonymous, voivat **ohittaa odotus**tilan, käytä PowerShelliä tämän tehtävän suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="9ae1d-104">Seuraavassa on esimerkki organisaation yleisen Kokous käytäntöjen muokkaamisesta.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="9ae1d-105">Tämä cmdlet-toiminto edellyttää tällä hetkellä Skype for Business PowerShell-moduulin käyttöä.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="9ae1d-106">Jos haluat määrittää tämän cmdlet-toiminnon käyttö oikeuden, tutustu [käytäntöjen hallintaan PowerShellin avulla](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="9ae1d-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="9ae1d-107">Kun olet määrittänyt käytännöt, sinun on otettava se käyttöön käyttäjille. Jos olet muokannut yleistä käytäntöä, se on automaattisesti käytössä myös käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="9ae1d-108">Jos haluat muuttaa käytäntöä, sinun on odotettava vähintään **neljä tuntia** , ennen kuin käytännöt astuvat voimaan.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="9ae1d-109">Tarkista alla olevat ohjeet, ennen kuin teet nämä muutokset, jotta ymmärrät tarkalleen, mitä tämä sallii.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="9ae1d-110">Teamsin Kokous aulan käytäntöjen hallinta</span><span class="sxs-lookup"><span data-stu-id="9ae1d-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="9ae1d-111">Nämä asetukset ohjaavat sitä, mitkä koko uksen osallistujat odottavat odotus tilassa, ennen kuin heidät otetaan mukaan koko ukseen ja osallistumis aste on sallittu koko uksessa.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="9ae1d-112">Voit päivittää PowerShellin avulla Kokous käytäntöjen asetukset, joita ei ole vielä toteutettu (merkintä "tulossa pian") teamsin hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="9ae1d-113">Alla on esimerkki PowerShellin cmdlet-komentosovelmasta, jonka avulla kaikki käyttäjät voivat ohittaa aulan.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="9ae1d-114">Hyväksy [automaattisesti henkilöt](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) -vaihto ehto, joka määrittää, liittyvätkö ihmiset koko ukseen suoraan vai odottaako hän sitä, kunnes käyttäjä on myöntänyt sen oikeaksi.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="9ae1d-115">[Salli anonyymien henkilöiden aloittaa Kokous](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) on ohjaajakohtainen menettely tapa, joka määrittää, voivatko anonyymit henkilöt, mukaan lukien B2B ja liitetyt käyttäjät, liittyä käyttäjän koko ukseen ilman todennettua käyttäjää organisaation läsnäololistalla.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="9ae1d-116">[Salli Puhelin käyttäjät voivat ohittaa aulan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**tulossa pian**) on ohjaajakohtainen menettely tapa, joka määrittää, liittyvätkö käyttäjät, jotka ovat soittamassa koko ukseen suoraan tai odotus tilassa, huolimatta siitä, hyväksyykö se **automaattisesti ihmiset** -asetuksen.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="9ae1d-117">[Salli järjestäjien ohittaa aulan asetukset](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**tulossa pian**) on organisoija, joka määrittää, voiko koko uksen järjestäjä ohittaa asetukset, jotka järjestelmänvalvoja on määrittänyt **automaattisesti** , ja **Salli Puhelin käyttäjät voivat ohittaa aulan** , kun he ajoittavat uuden koko uksen.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="9ae1d-118">**Huomautus:** Lukemalla [Kokous käytäntöjen hallinta teamsissa](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) saat kattavan yleiskatsauksen Microsoft teamsin Kokous käytännöistä.</span><span class="sxs-lookup"><span data-stu-id="9ae1d-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
