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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023519"
---
# <a name="turn-on-ndi-technology"></a>NDI-tekniikan käyttöönottaaminen

NDI-tekniikka edellyttää, että käyttäjällä on kaksi vaihetta:

1. Vuokraajan järjestelmänvalvojan on otettava käyttöön AllowNDIStreaming-ominaisuus CsTeamsMeetingPolicyssa.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Kun tämä muutos on täytetty, käyttäjän on otettava NDI®-tekniikka käyttöön tietyssä asiakasohjelmassa **Asetukset > käyttöoikeudet.**

Lisätietoja on kohdassa [NDI-tekniikan käyttö Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
