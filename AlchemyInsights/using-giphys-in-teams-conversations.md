---
title: Giphys-käyttö teamsin keskusteluissa
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982458"
---
# <a name="using-giphys-in-teams-conversations"></a>Giphys-käyttö teamsin keskusteluissa

Giphys-käyttö oikeus teamsin keskustelussa on oletusarvoisesti käytössä. Järjestelmänvalvojana voit hallita sitä, voivatko käyttäjät käyttää käyttäjiä asettamalla [viestintä käytäntöä](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) ja **varmistamalla, että** **keskustelujen käyttö** on käytössä.

Jos GIF ei toimi oikein teamsin keskusteluissa, tarkista seuraavat asiat:

[Viestintä käytäntöjen](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) on sallittava giphys. Varmentamaan PowerShell-cmdlet-komennolla:

- Varmista, että voit [hallita Teamsia PowerShellin avulla](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Suorita PowerShell-komento [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ja varmista, että **Allowgiphy** -asetuksena on **True**.
- Jos **Allowgiphy-parametrin** arvo on **false** , suorita seuraava PowerShell [-komento joukko-CsTeamsMessagingPolicy-Identity Global-allowgiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

Jos haluat käyttää Giphy-URL-osoitetta, [valinnaisten yhdistettyjen kokemusten](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) on oltava käytössä.

> [!NOTE]
> Jos sinulla on useita teamsin viestintä käytäntöjä, voit määrittää käyttäjälle, jolle ongelma on määritetty, PowerShell [-komennolla Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Valitse TeamsMessagingPolicy.
