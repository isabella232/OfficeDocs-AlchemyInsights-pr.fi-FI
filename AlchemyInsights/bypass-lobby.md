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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Hallitse aulan asetuksia ja osallistumis tasoa tiimeihin

Jos haluat, että kaikki käyttäjät, kuten dial-in, External ja Anonymous, voivat **ohittaa odotus**tilan, käytä PowerShelliä tämän tehtävän suorittamiseen. Seuraavassa on esimerkki organisaation yleisen Kokous käytäntöjen muokkaamisesta.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Tämä cmdlet-toiminto edellyttää tällä hetkellä Skype for Business PowerShell-moduulin käyttöä. Jos haluat määrittää tämän cmdlet-toiminnon käyttö oikeuden, tutustu [käytäntöjen hallintaan PowerShellin avulla](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Kun olet määrittänyt käytännöt, sinun on otettava se käyttöön käyttäjille. Jos olet muokannut yleistä käytäntöä, se on automaattisesti käytössä myös käyttäjille. Jos haluat muuttaa käytäntöä, sinun on odotettava vähintään **neljä tuntia** , ennen kuin käytännöt astuvat voimaan. 

Tarkista alla olevat ohjeet, ennen kuin teet nämä muutokset, jotta ymmärrät tarkalleen, mitä tämä sallii.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Teamsin Kokous aulan käytäntöjen hallinta

Nämä asetukset ohjaavat sitä, mitkä koko uksen osallistujat odottavat odotus tilassa, ennen kuin heidät otetaan mukaan koko ukseen ja osallistumis aste on sallittu koko uksessa. Voit päivittää PowerShellin avulla Kokous käytäntöjen asetukset, joita ei ole vielä toteutettu (merkintä "tulossa pian") teamsin hallinta keskuksessa. Alla on esimerkki PowerShellin cmdlet-komentosovelmasta, jonka avulla kaikki käyttäjät voivat ohittaa aulan.

- Hyväksy [automaattisesti henkilöt](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) -vaihto ehto, joka määrittää, liittyvätkö ihmiset koko ukseen suoraan vai odottaako hän sitä, kunnes käyttäjä on myöntänyt sen oikeaksi.

- [Salli anonyymien henkilöiden aloittaa Kokous](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) on ohjaajakohtainen menettely tapa, joka määrittää, voivatko anonyymit henkilöt, mukaan lukien B2B ja liitetyt käyttäjät, liittyä käyttäjän koko ukseen ilman todennettua käyttäjää organisaation läsnäololistalla.

- [Salli Puhelin käyttäjät voivat ohittaa aulan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**tulossa pian**) on ohjaajakohtainen menettely tapa, joka määrittää, liittyvätkö käyttäjät, jotka ovat soittamassa koko ukseen suoraan tai odotus tilassa, huolimatta siitä, hyväksyykö se **automaattisesti ihmiset** -asetuksen.

- [Salli järjestäjien ohittaa aulan asetukset](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**tulossa pian**) on organisoija, joka määrittää, voiko koko uksen järjestäjä ohittaa asetukset, jotka järjestelmänvalvoja on määrittänyt **automaattisesti** , ja **Salli Puhelin käyttäjät voivat ohittaa aulan** , kun he ajoittavat uuden koko uksen.

**Huomautus:** Lukemalla [Kokous käytäntöjen hallinta teamsissa](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) saat kattavan yleiskatsauksen Microsoft teamsin Kokous käytännöistä.
