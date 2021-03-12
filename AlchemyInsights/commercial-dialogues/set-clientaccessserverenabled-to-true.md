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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746417"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Aseta ClientAccessServerEnabled-arvoksi Tosi

Jos et voi avata salattua sähköpostiviestiä ja nähdä sen sijaan **rpmsg-liitteen,** toimi seuraavasti:

1. Muodosta yhteys Exchange Online PowerShelliin.

> [!NOTE]
> Jos haluat muodostaa yhteyden Exchange Online PowerShelliin, sinun on kirjauduttava sisään yleisen järjestelmänvalvojan tai Exchange-järjestelmänvalvojan tilillä.

   a. Avaa Windows PowerShell ja suorita sitten seuraava komento: `$UserCredential = Get-Credential`
b. Kirjoita **Windows PowerShellin tunnistetietopyyntö** -valintaikkunaan työ- tai koulutilisi ja salasanasi, c. Valitse **OK**. 

2. Luo uusi istunto suoritamalla seuraava komento:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Suorita seuraava komento:
    
    `Import-PSSession $Session -DisableNameChecking`

3. `Get-IRMConfiguration`Suorita-komento.

4. Tarkista **ClientAccessServerEnabled-asetus.** 

    a. Jos **ClientAccessServerEnabled-asetuksena** on **Epätosi,** suorita seuraava cmdlet-komento: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Sulje powershell-istunto aina seuraavalla komennolla: `Remove-PSSession $Session`

Lisätietoja on Exchange [Online PowerShellissä.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

