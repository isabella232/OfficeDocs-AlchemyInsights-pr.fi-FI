---
title: Välityspalvelimen osoitevirhe jaetun postilaatikon luonnin aikana
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062905"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Välityspalvelimen osoitevirhe postilaatikon tai muun sähköpostia käyttävän objektin luonnin aikana

Jos yritit luoda sähköpostia käyttävän objektin (postilaatikko, jaettu postilaatikko jne.) ja sait virhesanoman "Välityspalvelimen osoite "SMTP:alias@domain.com" on jo käytössä...", valitsemaasi sähköpostiosoitetta käyttää jo toinen sähköpostia käyttävä objekti organisaatiossasi.
  
Sinun on etsittava käyttäjä, ryhmä, jaettu postilaatikko tai yleinen kansio, jolla on tämä sähköpostiosoite, ja poistettava se tai muutettava sen sähköpostiosoitetta. Sen jälkeen voit luoda uuden sähköpostia käyttävän objektin, jossa on vapaita sähköpostiosoitteita. Etsi se aloitussivun Haku-haun avulla. Voit myös hakea sitä Exchange Online PowerShell -komennolla:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Jos et halua poistaa olemassa olevaa sähköpostiosoitetta, valitse uusi sähköpostiosoite luomallesi uudelle objektille.
  