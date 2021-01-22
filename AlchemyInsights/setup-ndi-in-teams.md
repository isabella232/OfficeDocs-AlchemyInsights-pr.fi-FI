---
title: NDI-tekniikan käyttöönottaaminen
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935100"
---
# <a name="turn-on-ndi-technology"></a>NDI-tekniikan käyttöönottaaminen

NDI-tekniikka edellyttää, että käyttäjä ottaa käyttöön kaksi vaihetta:

1. Vuokraajan järjestelmänvalvojan on otettava AllowNDIStreaming-ominaisuus käyttöön CsTeamsMeetingPolicyssa.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Kun tämä muutos on täytetty, käyttäjän on otettava NDI®-tekniikka käyttöön tietyssä asiakasohjelmassa **Asetukset-> käyttöoikeudet -kohdassa.**

Lisätietoja on kohdassa [NDI-tekniikan käyttö Microsoft Teamsissa.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
