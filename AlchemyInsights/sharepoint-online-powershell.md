---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709067"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

PowerShellin tai komentosarjojen käyttäminen SharePoint Onlinessa Saat lisätietoja alla olevista linkeistä.
- [SharePoint Online -hallintaliittymän käytön aloittaminen](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Yhteyden muodostaminen SPO PowerShelliin monimenetelmäisen todentamisen (MFA) avulla](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisältää PowerShell-komentokirjaston, jonka avulla voit suorittaa monimutkaisia hallintatoimintoja SPO:ssa.

> [!NOTE]
> - Jos sinulla on ongelmia yhteyden muodostamisessa SPO-hallintaliittymään, varmista, että olet [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) päivittänyt uusimpaan versioon, ja yritä tuoda moduuli uudelleen käyttäen *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Jos yrität suorittaa asiakaspuolen objektimallikomentosarjoja, [SharePoint Onlinen](https://www.microsoft.com/download/details.aspx?id=42038) asiakaskomponenttien SDK on oltava asennettuna paikallisessa koneessa.
> - Jos sinulla on ongelmia komentosarjojen suorittamisessa PowerShellistä, voit harkita PowerShellin suorittamista järjestelmänvalvojana ja [suorituskäytännön vaihtamista.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)