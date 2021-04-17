---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830579"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

PowerShellin tai komentosarjojen käyttäminen SharePoint Onlinessa Saat lisätietoja alla olevista linkeistä.
- [SharePoint Online -hallintaliittymän käytön aloittaminen](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Yhteyden muodostaminen SPO PowerShelliin monimenetelmäisen todentamisen (MFA) avulla](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisältää PowerShell-komentokirjaston, jonka avulla voit suorittaa monimutkaisia hallintatoimintoja SPO:ta varten.

> [!NOTE]
> - Jos sinulla on ongelmia yhteyden muodostamisessa SPO-hallintaliittymään, varmista, että olet [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) päivittänyt uusimpaan versioon ja yritä tuoda moduuli uudelleen käyttäen *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Jos yrität suorittaa asiakaspuolen objektimallikomentosarjoja, [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) on oltava asennettuna paikallisessa koneessa.
> - Jos sinulla on ongelmia komentosarjojen suorittamisessa PowerShellistä, voit harkita PowerShellin suorittamista järjestelmänvalvojana ja [suorituskäytännön vaihtamista.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)