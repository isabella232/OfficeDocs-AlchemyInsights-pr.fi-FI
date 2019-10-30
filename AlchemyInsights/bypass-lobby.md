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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768437"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Hallitse aulan asetuksia ja osallistumis tasoa

Jos haluat sallia kaikkien, mukaan lukien Puhelin verkko-, ulkoiset ja anonyymit käyttäjät, ohittaa aulan Microsoft Teamsissa, voit tehdä sen PowerShellin avulla. Tässä on esimerkki organisaation maailmanlaajuisen koko uksen käytännön muuttamisesta:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Tämä cmdlet-komento edellyttää tällä hetkellä Skype for Business PowerShell-moduulin käyttöä. Jos haluat saada asennus ohjelman käyttämään tätä cmdlet-komentoa, tutustu [käytäntöjen hallintaan PowerShellin kautta](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Voit määrittää uuden käytännön, jota sinun on sitten sovellettava käyttäjiin. Jos muokkaat yleistä käytäntöä, se koskee käyttäjiä automaattisesti. Jos haluat muuttaa käytäntöä, sinun on odotettava vähintään 4 tuntia ja enintään 24 tuntia, jotta käytännöt tulevat voimaan.

Muista tarkistaa alla olevat ohjeet ennen muutosten tekemistä, jotta ymmärrät tarkalleen, mitä tämä sallii.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Tietoja tiimien koko uksen aulan käytännön valvonnasta

- [Henkilöiden automaattinen myöntäjä](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) on järjestäjäkohtainen käytäntö, joka ohjaa sitä, liittytäänkö koko ukseen suoraan vai odotetaanko sitä aulassa, kunnes todennettu käyttäjä on myöntänyt heidät.

- [Nimettömät henkilöt voivat aloittaa koko uksen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , on järjestäjäkohtainen käytäntö, joka ohjaa sitä, voivatko anonyymit henkilöt, mukaan lukien B2B-ja Federated-käyttäjät, liittyä käyttäjän koko ukseen ilman organisaation todennetun käyttäjän läsnäoloa.

- [Salli dial-in-käyttäjien ohittaa aula](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**tulossa pian**) on järjestäjäkohtainen käytäntö, joka ohjaa sitä, liittääkö Puhelin puhelimitse suoraan koko ukseen vai odottaako se aulan automaattisesti, riippumatta siitä, sallitaanko **ihmiset** -asetus.

- [Salli järjestäjien ohittaa aulan asetukset](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**tulossa pian**) on järjestäjäkohtainen käytäntö, joka määrittää, voiko koko uksen järjestäjä ohittaa aulan asetukset, jotka järjestelmänvalvoja asettaa **automaattisesti myöntämään ihmisiä** ja **sallimaan soiton käyttäjiä ohittamaan aulan** , kun he aikatauluttaa uuden koko uksen.

**Huom:** Lue [teams-Kokous käytäntöjen hallinta](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , niin saat yleiskatsauksen Microsoft teams-Kokous käytännöistä.
