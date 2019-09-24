---
title: SharePoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/23/2019
ms.locfileid: "37122996"
---
# <a name="sharepoint-online-powershell"></a>SharePoint Online PowerShell

Työskentelen PowerShellin tai komento sarjojen kanssa SharePoint Onlinessa? Lisä tietoja on alla olevissa linkeissä.
- [SharePointin online-hallinta liittymän käytön aloittaminen](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Yhdistä SPO PowerShelliin monivaiheisen todennuksen avulla (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint-mallit ja-käytännöt (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisältää PowerShell-komentojen kirjaston, jonka avulla voit suorittaa monimutkaisia hallinta toimia SPO: tä kohti.

> [!NOTE]
> - Jos sinulla on ongelmia yhteyden muodostamisessa SPO-hallinta liittymään, varmista, että olet päivittänyt uusimpaan versioon ja yritä [tuoda moduuli uudelleen](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) käyttämällä *"Import-moduuli Microsoft. online. SharePoint. PowerShell"* -moduulia.
> - Jos yrität suorittaa asiakas puolen objekti mallin komento sarjoja, [SharePoint Online-asiakas komponenttien SDK](https://www.microsoft.com/download/details.aspx?id=42038) on asennettava paikalliseen tieto koneeseen.
> - Jos sinulla on ongelmia PowerShell-komento sarjojen suorittamisen kanssa, sinun kannattaa harkita PowerShellin suorittamista järjestelmänvalvojana ja [suoritus käytännön](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)muuttamista.