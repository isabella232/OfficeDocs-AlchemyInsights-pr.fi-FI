---
title: Yksityinen kanava
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005435"
---
# <a name="private-channels-in-microsoft-teams"></a>Yksityiset kanavat Microsoft Teamsissa

Yksityiset kanavat ovat microsoft Teamsin uusi ominaisuus. Huomaa, että yksityisiä kanavia ei voi muuntaa vakiokanavista tai päinvastoin.

Lisätietoja yksityisistä kanavista, kuten [yksityiskanavien luomisesta ja jäsenyydestä](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) sekä [yksityisestä SharePoint-sivustoista](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), on kohdassa [Microsoft Teamsin yksityiset kanavat](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Huomautus:** Koska yksityisten kanavien viestien säilyttämisen määritystä ei vielä tueta, vuokraajat, joiden säilytyskäytännöt ovat käytössä, eivät oletusarvoisesti ota käyttöön yksityisiä kanavia. Yksityiset kanavat voidaan ottaa käyttöön Teams-hallintakeskuksessa. Huomaa myös, että vaikka yksityisten kanavien viestien säilyttämistä ei tueta, yksityisissä kanavissa jaettujen tiedostojen säilyttämistä tuetaan.

**Tarvitsetko uuden tiimin omistajan?**

Jos yksityinen kanavasi omistaja lähtee, voit lisätä uuden tiimin omistajan Teams Powershellin kautta.


- [Siirry tästä](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) asentaaKsesi Teams Powershellin.

Tässä on cmdlet tarvitset:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Lisätietoja Teams Powershellistä on kohdassa [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
