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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Hallita aula-asetuksia ja osallistumisen tasoa Teamsissa

Jos haluat, että kaikki, kuten puhelinneuvottelut, ulkoiset ja anonyymit käyttäjät, voivat ohittaa aulan **,** käytä PowerShelliä tämän tehtävän suorittamiseen. Seuraavassa on esimerkki organisaation yleisen kokouskäytännön muokkaamisesta.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Tämä cmdlet-komento edellyttää tällä hetkellä Skype for Business PowerShell -moduulin käyttöä. Jos haluat määrittää tämän cmdlet-komennon käyttöön, lue kohta Policies [via PowerShell (Hallitse käytäntöjä PowerShellin kautta).](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Kun olet määrittänyt käytännön, sinun on sovellettava sitä käyttäjiin. tai jos olet muokannut global-käytäntöä, se koskee automaattisesti käyttäjiä. Jos käytäntö muuttuu, sinun on odotettava vähintään 4 tuntia **ja 24** tuntia, ennen kuin käytännöt tulevat voimaan. 

Muista tarkistaa alla olevat ohjeet ennen muutosten tekeminen, jotta ymmärrät tarkalleen, mitä tämä sallii.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Teamsin kokouksen aulakäytännön hallinta

Näillä asetuksilla voit määrittää, mitkä kokouksen osallistujat odottavat odotustilassa, ennen kuin heidät hyväksytään kokoukseen, ja osallistujat voivat osallistua kokoukseen. PowerShellin avulla voit päivittää kokouskäytäntöasetuksia, joita ei ole vielä otettu käyttöön (tulossa pian) Teams-hallintakeskuksessa. Alla on esimerkki PowerShell-cmdlet-komennosta, jonka avulla kaikki käyttäjät voivat ohittaa aulan.

- [Hyväksy henkilöt automaattisesti](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) järjestäjän mukaan -käytäntö, joka määrittää, liittyvätkö henkilöt kokoukseen suoraan vai odottavat odotustilassa, kunnes todennettu käyttäjä on myöntänyt heidät sisään.

- [Salli anonyymien](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) käyttäjien aloittaa kokous on järjestäjäkohtainen käytäntö, joka määrittää, voivatko anonyymit henkilöt, mukaan lukien B2B- ja liitetyt käyttäjät, liittyä käyttäjän kokoukseen ilman organisaation todennettua käyttäjää.

- [Salli puhelinkäyttäjien](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) ohittaa odotustila **(tulossa** pian) on järjestäjäkohtainen käytäntö, joka määrittää, liittyvätkö puhelinyhteyden kautta soittavat henkilöt kokoukseen suoraan vai odottavat odotustilassa Hyväksy henkilöt automaattisesti **-asetuksen** välittämisen väliltä.

- [Salli järjestäjien](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) ohittaa aula-asetukset **(tulossa** pian) on järjestäjäkohtainen käytäntö, joka määrittää, voiko  kokouksen järjestäjä  ohittaa aula-asetukset, jotka järjestelmänvalvoja on määrittänyt asetuksissa Hyväksy käyttäjät automaattisesti ja Salli puhelinkäyttäjien ohittaa aula, kun he ajoittavat uuden kokouksen.

**Huomautus:** Lue [kokouskäytäntöjen hallinta Teamsissa,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) niin saat täydellisen yleiskatsauksen Microsoft Teams -kokouskäytännöistä.
