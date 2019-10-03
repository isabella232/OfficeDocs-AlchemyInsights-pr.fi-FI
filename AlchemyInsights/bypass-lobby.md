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
# <a name="control-lobby-settings-and-level-of-participation"></a>Hallitse aulan asetuksia ja osallistumis tasoa

Nämä asetukset ohjaavat sitä, ketkä osallistujat odottavat aulassa ennen kuin heidät otetaan mukaan koko ukseen ja kuinka suuri osallistumis aste he saavat koko uksessa. Voit käyttää PowerShelliä päivittämään Kokous käytäntö asetukset, joita ei ole vielä toteutettu (merkitty "tulossa pian") teams-hallinta keskukseen.  Katso alla esimerkki PowerShell cmdlet, jonka avulla kaikki käyttäjät voivat ohittaa aulan.  

- [Henkilöiden automaattinen myöntäjä](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) on järjestäjäkohtainen käytäntö, joka ohjaa sitä, liittytäänkö koko ukseen suoraan vai odotetaanko sitä aulassa, kunnes todennettu käyttäjä on myöntänyt heidät.

- [Nimettömät henkilöt voivat aloittaa koko uksen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , on järjestäjäkohtainen käytäntö, joka ohjaa sitä, voivatko anonyymit henkilöt, mukaan lukien B2B-ja Federated-käyttäjät, liittyä käyttäjän koko ukseen ilman organisaation todennetun käyttäjän läsnäoloa.

- [Salli dial-in-käyttäjien ohittaa aula](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**tulossa pian**) on järjestäjäkohtainen käytäntö, joka ohjaa sitä, liittääkö Puhelin puhelimitse suoraan koko ukseen vai odottaako se aulan automaattisesti, riippumatta siitä, sallitaanko **ihmiset** -asetus.

- [Salli järjestäjien ohittaa aulan asetukset](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**tulossa pian**) on järjestäjäkohtainen käytäntö, joka määrittää, voiko koko uksen järjestäjä ohittaa aulan asetukset, jotka järjestelmänvalvoja asettaa **automaattisesti myöntämään ihmisiä** ja **sallimaan soiton käyttäjiä ohittamaan aulan** , kun he aikatauluttaa uuden koko uksen.

**Huom:** Lue [teams-Kokous käytäntöjen hallinta](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , niin saat yleiskatsauksen Microsoft teams-Kokous käytännöistä. 


**PowerShell-esimerkki**

Jos haluat sallia kaikkien, myös ulkoisten tai anonyymien käyttäjien, ohittaa aulan, voit myös käyttää PowerShelliä tämän tehtävän suorittamiseen.  Tässä on esimerkki organisaation maailmanlaajuisen Kokous käytännön muuttamisesta.   

(Muista tarkistaa edellä mainitut ohjeet ennen muutosten tekemistä, jotta ymmärrät tarkalleen, mitä tämä sallii.)

Set-CsTeamsMeetingPolicy-identiteetti Global-Autosisääntulokäyttäjät "kaikki"-AllowPSTNUsersToBypassLobby $True

Lisä tietoja on kohdassa [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
