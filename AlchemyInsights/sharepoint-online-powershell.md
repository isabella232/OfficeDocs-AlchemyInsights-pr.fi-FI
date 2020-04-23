---
title: Sharepoint Online -PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764258"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online -PowerShell

PowerShellin tai Komentosarjojen käyttäminen Sharepoint Onlinessa? Lisätietoja on alla olevissa linkeissä.
- [SharePoint Online -hallintaliittymän käytön aloittaminen](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Yhteyden muodostaminen SPO PowerShelliin monitekijätodennuksen (MFA) avulla](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisältää PowerShell-komentojen kirjaston, jonka avulla voit suorittaa monimutkaisia hallintatoimintoja spo:ta kohtaan.

> [!NOTE]
> - Jos sinulla on ongelmia yhteyden muodostamisessa SPO:n hallintaliittymän kanssa, varmista, että olet päivittänyt uusimpaan versioon, ja yritä [tuoda moduuli uudelleen](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) *"Import-Module Microsoft.Online.SharePoint.PowerShell" -toiminnon avulla.*
> - Jos yrität suorittaa asiakaspuolen objektimallikomentosarjoja, [sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) on oltava asennettuna paikalliseen tietokoneeseen.
> - Jos sinulla on ongelmia komentosarjojen suorittamisessa PowerShellistä, kannattaa harkita PowerShellin suorittamista järjestelmänvalvojana ja [suorituskäytännön](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)muuttamista.