---
title: Arkistopostilaatikkosi on lähes täynnä
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046749"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Arkistopostilaatikkosi on lähes täynnä

Jos käyttäjä saa varoituksen; **Arkistopostilaatikkosi on lähes** täynnä tai sinun on lisättävä arkistopostilaatikon kokoa, seuraavassa on joitain vinkkejä:

1. Jos käyttäjälle on määritetty Exchange Online 1, päivitä **Exchange Online 2** -käyttöoikeuteen, jotta voit suurentaa koon 50 gt:stä 100 gt:ksi.
1. Jos käyttäjälle on jo määritetty jompikumpi seuraavista: **Exchange Online Plan 2** tai Exchange Online Plan 1 ja Exchange Online Archiving-lisäosa, ota automaattinen laajentaminen käyttöön alla olevia ohjeita noudattamalla:.
 
    1. [Näyttöyhteys Powershellin Exchange Online avulla.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Suorita käyttäjälle seuraava komento:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Suorita seuraava komento, kun haluat varmistaa, että se on otettu käyttöön käyttäjällä:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Lisätietoja on ohjeaiheessa:

- [Rajoittamattoman arkistoinnin ottaminen käyttöön – järjestelmänvalvojan Microsoft 365 yhteensopivuus | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online - Palvelukuvaukset-| Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Toiseen Business-| Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

