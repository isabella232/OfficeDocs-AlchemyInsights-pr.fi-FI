---
title: Exchange PowerShell ja perustodentamisen käytöstä poistuminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015686"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell ja perustodentamisen käytöstä poistuminen

Jos haluat lisätietoja yhteyden muodostamisesta Exchange Online PowerShelliin ilman perustodentamista, [siirry tänne](https://aka.ms/psbasicauth).

Ota huomioon, että asiakaskoneessa on yhä otettava käyttöön perustodennus.
Uusi PowerShell V2 -moduuli käyttää modernia todennusta yhteyden luomiseen, jotta kaikki REST-pohjaiset V2 cmdlet -komennot voidaan ottaa käyttöön. V2 cmdlet -komentojen lisäksi voit käyttää sen avulla vanhemman etä-PowerShellin (RPS) cmdlet-komentoja, jotka edellyttävät etä-PowerShell-istuntoa. RPS-istunnon luominen Windows-tietokoneessa edellyttää, että WinRM-perustodennus on käytössä asiakaskoneessa, vaikka moduuli käyttää modernia todennusmekanismia palvelun todentamiseen. WinRM-perustodennusjaksoa käytetään modernien todennustunnusten siirtämiseen. Jos WinRM-perustodennus ei ole käytössä asiakaskoneessa, uudet V2 cmdlet -komennot toimivat (mutta vanhemmat RPS cmdlet -komennot eivät).
