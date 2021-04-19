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
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813469"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell ja perustodentamisen käytöstä poistuminen

Jos haluat lisätietoja yhteyden muodostamisesta Exchange Online PowerShelliin ilman perustodentamista, [siirry tänne](https://aka.ms/exops-docs). PowerShell V2 -moduuli ei käytä perustodennusta.

Ota huomioon, että asiakaskoneessa on yhä otettava käyttöön perustodennus.
Uusi PowerShell V2 -moduuli käyttää modernia todennusta yhteyden luomiseen, jotta kaikki REST-pohjaiset V2 cmdlet -komennot voidaan ottaa käyttöön. V2 cmdlet -komentojen lisäksi voit käyttää sen avulla vanhemman etä-PowerShellin (RPS) cmdlet-komentoja, jotka edellyttävät etä-PowerShell-istuntoa. RPS-istunnon luominen Windows-tietokoneessa edellyttää, että WinRM-perustodennus on käytössä asiakaskoneessa, vaikka moduuli käyttää modernia todennusmekanismia palvelun todentamiseen. WinRM-perustodennusjaksoa käytetään modernien todennustunnusten siirtämiseen. Jos WinRM-perustodennus ei ole käytössä asiakaskoneessa, uudet V2 cmdlet -komennot toimivat (mutta vanhemmat RPS cmdlet -komennot eivät).
