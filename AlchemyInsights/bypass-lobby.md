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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Hallitse aulan asetuksia ja tiimien osallistumis tasoa

Jos haluat sallia kaikkien, mukaan lukien Puhelin verkko-, ulkoiset ja anonyymit käyttäjät, **ohittaa aulan**, käytä PowerShelliä tämän tehtävän suorittamiseen. Tässä on esimerkki organisaation maailmanlaajuisen Kokous käytännön muuttamisesta.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Tämä cmdlet-komento edellyttää tällä hetkellä Skype for Business PowerShell-moduulin käyttöä. Jos haluat määrittää tämän cmdlet-komennolla, tutustu [käytäntöjen hallintaan PowerShellin kautta](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Kun olet määrittänyt käytännön, sinun on sovellettava sitä käyttäjille; Jos olet muokannut yleistä käytäntöä, se koskee käyttäjiä automaattisesti. Jos haluat muuttaa käytäntöä, sinun on odotettava vähintään **4 tuntia 24 tuntiin** , jotta käytännöt tulevat voimaan. 

Muista tarkistaa alla olevat ohjeet ennen muutosten tekemistä, jotta ymmärrät tarkalleen, mitä tämä sallii.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Tietoja tiimien koko uksen aulan käytännön valvonnasta

Nämä asetukset ohjaavat sitä, ketkä osallistujat odottavat aulassa ennen kuin heidät otetaan mukaan koko ukseen ja kuinka suuri osallistumis aste he saavat koko uksessa. Voit käyttää PowerShelliä päivittämään Kokous käytäntö asetukset, joita ei ole vielä toteutettu (merkitty "tulossa pian") teams-hallinta keskukseen. Katso alla esimerkki PowerShell cmdlet, jonka avulla kaikki käyttäjät voivat ohittaa aulan.

- [Henkilöiden automaattinen myöntäjä](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) on järjestäjäkohtainen käytäntö, joka ohjaa sitä, liittytäänkö koko ukseen suoraan vai odotetaanko sitä aulassa, kunnes todennettu käyttäjä on myöntänyt heidät.

- [Nimettömät henkilöt voivat aloittaa koko uksen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , on järjestäjäkohtainen käytäntö, joka ohjaa sitä, voivatko anonyymit henkilöt, mukaan lukien B2B-ja Federated-käyttäjät, liittyä käyttäjän koko ukseen ilman organisaation todennetun käyttäjän läsnäoloa.

- [Salli dial-in-käyttäjien ohittaa aula](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**tulossa pian**) on järjestäjäkohtainen käytäntö, joka ohjaa sitä, liittääkö Puhelin puhelimitse suoraan koko ukseen vai odottaako se aulan automaattisesti, riippumatta siitä, sallitaanko **ihmiset** -asetus.

- [Salli järjestäjien ohittaa aulan asetukset](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**tulossa pian**) on järjestelijä koskeva käytäntö, joka ohjaa sitä, voiko koko uksen järjestäjä ohittaa aulan asetukset, jotka järjestelmänvalvoja asettaa **automaattisesti myöntämään ihmisille** ja **sallia soiton käyttäjien ohittaa aulan** , kun he aikatauluttaa uuden koko uksen.

**Huom:** Lue [teams-Kokous käytäntöjen hallinta](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , niin saat yleiskatsauksen Microsoft teams-Kokous käytännöistä.
