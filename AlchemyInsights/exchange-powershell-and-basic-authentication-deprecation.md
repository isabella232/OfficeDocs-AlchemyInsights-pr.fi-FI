---
title: Exchange PowerShell ja perustodentamisen käytöstä poistuminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069241"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell ja perustodentamisen käytöstä poistuminen

Jos haluat lisätietoja yhteyden muodostamisesta Exchange Online PowerShelliin ilman perustodentamista, [siirry tänne](https://aka.ms/exops-docs). PowerShell V2 -moduuli ei käytä perustodennusta.

Ota huomioon, että asiakaskoneessa on yhä otettava käyttöön perustodennus.
Uusi PowerShell V2 -moduuli käyttää modernia todennusta yhteyden luomiseen, jotta kaikki REST-pohjaiset V2 cmdlet -komennot voidaan ottaa käyttöön. V2 cmdlet -komentojen lisäksi voit käyttää sen avulla vanhemman etä-PowerShellin (RPS) cmdlet-komentoja, jotka edellyttävät etä-PowerShell-istuntoa. RPS-istunnon luominen Windows-tietokoneessa edellyttää, että WinRM-perustodennus on käytössä asiakaskoneessa, vaikka moduuli käyttää modernia todennusmekanismia palvelun todentamiseen. WinRM-perustodennusjaksoa käytetään modernien todennustunnusten siirtämiseen. Jos WinRM-perustodennus ei ole käytössä asiakaskoneessa, uudet V2 cmdlet -komennot toimivat (mutta vanhemmat RPS cmdlet -komennot eivät).
