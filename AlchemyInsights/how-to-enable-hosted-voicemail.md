---
title: Hosted Voicemailin käyttöönotto
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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/09/2020
ms.locfileid: "49678001"
---
# <a name="how-to-enable-hosted-voicemail"></a>Hosted Voicemailin käyttöönotto

Jos haluat ottaa vasta ajan käyttöön, **Hostedvoicemail** -asetuksena on oltava $TRUE.

**Hostedvoicemail** -ominaisuus käyttäjän etäpowershellin (RPS) avulla.

Lisä tietoja yhteyden muodostamisesta RPS-palveluun on [Microsoft teamsin PowerShellin yleiskatsaus](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) -kohdassa, jossa on lisä tietoja yhteyden MUODOSTAMISESTA RPS-palveluun.

1. Teamsin järjestelmänvalvojan tulee olla kirjautuneena teamsin PowerShell-etäpalvelimeen.
1. PowerShell-kehotteesta teamsin järjestelmänvalvoja voi suorittaa **joukko-csuser user@contoso.com-Hostedvoicemailin $True** , jossa SIP URI on kyseisessä käyttäjä.

> [!NOTE]
> Käytäntöjen muutokset voivat kestää jopa 24 tuntia, ennen kuin ne replikoidaan.