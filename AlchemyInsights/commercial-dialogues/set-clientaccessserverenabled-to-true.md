---
title: Aseta ClientAccessServerEnabled-arvoksi Tosi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994862"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Aseta ClientAccessServerEnabled-arvoksi Tosi

Jos et voi avata salattua sähköpostiviestiä ja nähdä sen sijaan **rpmsg-liitteen,** toimi seuraavasti:

1. Näyttöyhteys PowerShellin Exchange Online avulla.

> [!NOTE]
> Jos haluat muodostaa Exchange Online PowerShelliin, sinun on kirjauduttava sisään yleisen järjestelmänvalvojan tai Exchange järjestelmänvalvojan tilillä.

   a. Avaa Windows PowerShell ja suorita sitten seuraava komento:`$UserCredential = Get-Credential`
b. Kirjoita **Windows PowerShell tunnistetietopyyntö** -valintaikkunaan työ- tai koulutilisi ja salasanasi, c. Napsauta **OK**. 

2. Luo uusi istunto suoritamalla seuraava komento:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Suorita seuraava komento:
    
    `Import-PSSession $Session -DisableNameChecking`

3. `Get-IRMConfiguration`Suorita-komento.

4. Tarkista **ClientAccessServerEnabled -asetus.** 

    a. Jos **ClientAccessServerEnabled-asetuksena** on **Epätosi**, suorita seuraava cmdlet-komento: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Sulje PowerShell-istunto aina seuraavalla komennolla: `Remove-PSSession $Session`

Lisätietoja on kohdassa Exchange Online [käyttäminen.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

