---
title: Koko uksen käytäntö asetukset
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376616"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Kokous käytäntöjen hallinta Microsoft Teamsissa

Kokous käytäntöjä käytetään sellaisten toimintojen hallintaan, jotka ovat osallistujien organisaation käyttäjien aikatauluttamien kokousten osanottajien käytettävissä. Joitakin Kokous käytäntöjen ominaisuuksia ei ehkä ole vielä toteutettu teams-hallinta keskuksessa (nämä on merkitty "tulossa pian" dokumentaatiossa). Tässä tapa uksessa tai jos saat virheen, kuten "emme voi päivittää käytäntöä juuri nyt, mutta kokeilet sitä myöhemmin" Microsoft teams-hallinta keskuksessa, suosittelemme, että luot tai muokkaat teamsin Kokous käytäntöjä PowerShellin avulla. 

Lisä tietoja Kokous käytännöistä on seuraavissa resursseissa:

- Lisä tietoja käytäntöjen luomisesta, muutosten tekemisestä ja käyttäjien määrittämisestä käytäntöön on kohdassa [Kokous käytäntöjen hallinta teamsissa](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Jos haluat tehdä käytäntö muutoksia PowerShellin cmdlet-komentojen avulla, katso [teams PowerShell-yleiskatsaus](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Sinun on käytettävä [Skype for Business PowerShell-moduulia](https://www.microsoft.com/download/details.aspx?id=39366) teams-Kokous käytäntöihin. 
    - Lisä tietoja on [*-csteamsmeetingpolicy cmdlet-ohjeissa](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .

**Huom:** Käytännön muutosten vaikutus käyttäjiin voi kestää jopa 24 tuntia. Et ehkä voi tehdä muutoksia äskettäin luotuihin käytäntöihin välittömästi. Odota 4 tuntia ja yritä muokata juuri luotua käytäntöä uudelleen. Jos ongelmia ei vieläkään ole, kokeile PowerShelliä.  