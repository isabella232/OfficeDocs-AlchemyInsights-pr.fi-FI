---
title: Isännöidyn vastaajan ottaminen käyttöön
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055551"
---
# <a name="how-to-enable-hosted-voicemail"></a>Isännöidyn vastaajan ottaminen käyttöön

Jos haluat ottaa vastaajan käyttöön, **HostedVoicemail-asetuksena** on oltava $true.

Käyttäjän **HostedVoicemail-ominaisuus,** joka käyttää Etä-PowerShelliä (RPS).

Lisätietoja yhteyden muodostamisesta RPS-palveluntarjoajaan on [Microsoft Teams PowerShellin yleiskatsauksen](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) avulla.

1. Järjestelmänvalvojan Teams oltava kirjautuneena PowerShell-etäistuntoon Teams.
1. PowerShellin kehotteesta Teams Järjestelmänvalvoja voi suorittaa **set-csuser-user@contoso.com -HostedVoiceMail-$true** jossa sip uri on kyseiseltä käyttäjältä.

> [!NOTE]
> Käytäntöihin tehdyt muutokset voivat replikoida jopa 24 tuntia.