---
title: SharePoint Online PowerShell
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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770836"
---
# <a name="sharepoint-online-powershell"></a>SharePoint Online PowerShell

Työskenteleminen PowerShellin tai komento sarjojen kanssa SharePoint Onlinessa? Saat lisä tietoja alla olevista linkeistä.
- [SharePoint Online-hallinta liittymän käytön aloittaminen](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Yhteyden muodostaminen SPO PowerShelliin multifactor-todennuksella (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint-mallit ja-käytännöt (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisältää PowerShell-komentoja sisältävän kirjaston, jonka avulla voit suorittaa monimutkaisia hallinta toimia SPO:n hallintaan.

> [!NOTE]
> - Jos sinulla on ongelmia SPO-hallinta liittymän kanssa, varmista, että olet päivittänyt uusimpaan versioon, ja yritä [tuoda moduuli uudelleen](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) *"Import-Module Microsoft. online. SharePoint. PowerShell"* -toiminnolla.
> - Jos yrität suorittaa asiakas puolen objekti malli komento sarjoja, sinulla on oltava [SharePoint Online client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) asennettuna paikalliseen tieto koneeseesi.
> - Jos sinulla on ongelmia komento sarjojen suorittamisessa PowerShellissä, kannattaa ehkä harkita PowerShellin suorittamista järjestelmänvalvojana ja [suoritus käytäntöjen](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)vaihtamista.