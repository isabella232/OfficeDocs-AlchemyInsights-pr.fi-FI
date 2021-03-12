---
title: DKIM:n ottaminen käyttöön tietyssä toimialueella Exchange Online PowerShellin avulla
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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746278"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>DKIM:n ottaminen käyttöön tietyssä toimialueella Exchange Online PowerShellin avulla

Jos et voi luoda DKIM DNS -tietueita hallintakeskuksessa, kokeile Exchange Online PowerShelliä. 

Voit luoda DKIM DNS -tietueen Exchange Online PowerShellin avulla seuraavasti:

1. Avaa Windows PowerShell järjestelmänvalvojana ja suorita seuraavat komennot seuraavassa järjestyksessä:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Jos sinulla on ongelmia yhteyden muodostamisessa Exchange Online PowerShelliin, katso [kohta Yhteyden muodostaminen Exchange Online PowerShelliin.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Kun olet muodostanut yhteyden Exchange Online PowerShelliin, suorita seuraava komento:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Kun yllä oleva komento on suoritettu onnistuneesti, lopeta Exchange Online PowerShell -istunto suorittamalla seuraava komento:

    `Remove-PSSession $Session` 



