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
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974278"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Arkistopostilaatikkosi on lähes täynnä

Jos käyttäjä saa varoituksen; **Arkistopostilaatikkosi on lähes** täynnä tai sinun on lisättävä arkistopostilaatikon kokoa, seuraavassa on joitain vinkkejä:

1. Jos käyttäjälle on määritetty Exchange Online -palvelupaketti 1, päivitä **Exchange Online -palvelupaketti 2** -käyttöoikeuteen ja suurenna kokoa 50 Gt:stä 100 Gt:ksi.
1. Jos käyttäjälle on jo määritetty jompikumpi seuraavista: Exchange Online -palvelupaketti **2** tai Exchange Online -palvelupaketti 1 ja Exchange Online Archiving -lisäosa, ota automaattinen arkistointi käyttöön alla olevia ohjeita noudattamalla:.
 
    1. [Muodosta yhteys Exchange Online PowerShelliin.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Suorita käyttäjälle seuraava komento:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Varmista, että komento on otettu käyttöön käyttäjälle, toimimalla seuraavasti:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Lisätietoja on kohdassa:

- [ Rajoittamattoman arkistoinnin ottaminen käyttöön – järjestelmänvalvojan ohje – Microsoft 365 :n | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Onlinen rajoitukset – palvelukuvaukset | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Toiseen liiketoimintasuunnitelmaan päivittäminen | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

