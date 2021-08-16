---
title: DKIM Exchange Online ottaminen käyttöön tietyssä toimialueella PowerShellin avulla
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070295"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>DKIM Exchange Online ottaminen käyttöön tietyssä toimialueella PowerShellin avulla

Jos et voi luoda DKIM DNS -tietueita hallintakeskuksessa, kokeile käyttää PowerShelliä Exchange Online avulla. 

Voit luoda DKIM DNS -tietueen PowerShellin Exchange Online avulla seuraavasti:

1. Avaa Windows PowerShell järjestelmänvalvojana ja suorita seuraavat komennot seuraavassa järjestyksessä:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Jos yhteyden muodostaminen PowerShelliin Exchange Online on Näyttöyhteys [PowerShellin Exchange Online avulla.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Kun olet muodostanut yhteyden Exchange Online, suorita seuraava komento:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Kun edellä kuvattu komento on suoritettu onnistuneesti, lopeta PowerShell-istunto suorittamalla Exchange Online komento:

    `Remove-PSSession $Session` 



