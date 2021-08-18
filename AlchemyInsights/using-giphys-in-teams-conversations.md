---
title: Giphyjen käyttäminen Teams keskusteluissa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323517"
---
# <a name="using-giphys-in-teams-conversations"></a>Giphyjen käyttäminen Teams keskusteluissa

Giphyjen käyttö Teams on oletusarvoisesti käytössä. Järjestelmänvalvojana voit hallita, ovatko Giphyt käyttäjien [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) käytettävissä, määrittämällä viestikäytännön ja varmistamalla, että **Giphyjen** käyttö keskusteluissa **on käytössä.**

Jos GIF-tiedostot eivät toimi odotetulla Teams keskusteluissa, tarkista seuraavat:

Viestintäkäytännön [on sallittava](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) Giphyt. Tarkistaminen PowerShellin cmdlet-komentojen avulla:

- Varmista, että voit [hallita Teams PowerShellin avulla.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Suorita PowerShell-komento [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ja varmista, että **AllowGiphy-asetuksena** on **TOSI.**
- Jos **AllowGiphy-asetuksena** on **EPÄTOSI**, suorita seuraava [PowerShell-komento Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[Valinnaiset yhdistetyt](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) käyttökokemukset on otettava käyttöön, jotta Giphy-URL-osoitteen käyttö sallitaan.

**Huomautus:** Jos vuokraajalle on määritetty useita Teams-viestikäytäntöjä, voit määrittää käyttäjälle määritetyn käytännön käyttäjätiedot Käyttämällä [PowerShell-komentoa Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Valitse TeamsMessagingPolicy.
