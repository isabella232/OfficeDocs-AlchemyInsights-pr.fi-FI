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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318645"
---
# <a name="how-to-enable-hosted-voicemail"></a>Isännöidyn vastaajan ottaminen käyttöön

Jos haluat ottaa vastaajan käyttöön, **HostedVoicemail-asetuksena** on oltava $true.

Käyttäjän **HostedVoicemail-ominaisuus,** joka käyttää Etä-PowerShelliä (RPS).

Lisätietoja yhteyden muodostamisesta RPS:iin on [Microsoft Teams PowerShellin](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) yleiskatsauksesta.

1. Järjestelmänvalvojan Teams kirjauduttava PowerShell-etäistuntoon Teams.
1. PowerShellin kehotteesta Teams Järjestelmänvalvoja voi suorittaa **set-csuser-user@contoso.com -HostedVoiceMail$true** jossa sip uri on kyseiseltä käyttäjältä.

**Huomautus:** toimintakäytäntöjen replikointi voi kestää jopa 24 tuntia.